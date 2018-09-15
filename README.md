# Using docker install LNMP

* Installation environment

  - [Docker](https://docs.docker.com/install/)
  - [Docker Compose](https://docs.docker.com/compose/install/#install-compose)

* Git clone repository
    ```
    $ git clone https://github.com/bellawu0902/Docker-LNMP.git
    ```
    
* Run container
    
    Enter the project path and input instruction.

    
    ```
    $ docker-compose up -d
    ```

* Check container was run up

    ```
    $ docker ps
    ```
    
    You can see the result.
    
    ![docker ps](https://i.imgur.com/WWR4xiM.png)
    
* Check web service

    Open your browser and input http://localhost/index.php
    

* Delete all container

    If you want to delete all container, you can input the instruction.
    
    ```
    $ docker rm $(docker ps -a -q) -f
    ```
    
* Reference information
    
    - [Docker Hub](https://hub.docker.com/explore/)
    - [Docker Documentation](https://docs.docker.com/)
