Install Compose
sudo curl -L "https://github.com/docker/compose/releases/download/1.22.0/docker-compose-$(uname -s)-$(uname -m)" -o /usr/local/bin/docker-compose
sudo chmod +x /usr/local/bin/docker-compose


How to run
inside, compose-docker file run "docker-compose up --force-recreate &"
to stop "docker-compose down"
Curl <IP address>:5000 , to see the number of times this page is accessed. The value is saved in the Redis Server

build – The build option is used to build images for services for which build is defined.
$ docker-compose build             ## Build all services
$ docker-compose build web         ## Build single service


up – Use to create docker containers with available services in docker-compose.yml file in current directory. Use -d switch to launch containers in daemon mode.
$ docker-compose up -d            ## Create all containers
$ docker-compose up -d web        ## Create single container


down – This will stop and delete all containers, network and associated images for the services defined in a config file
$ docker-compose down           ## Restart all containers
$ docker-compose down web       ## Restart single container


ps – This will list all containers created for the services defined in a config file with there status, port bindings and command.
$ docker-compose ps 


exec – This will execute a command to the running container. For example list files in container associated with web service.
$ docker-compose exec web ls -l


start – This will start stopped containers of the services defined in config file
$ docker-compose start            ## Start all containers
$ docker-compose start web        ## Start single container


stop – This will stop running containers for the services defined in config file
$ docker-compose stop             ## Stop all containers
$ docker-compose stop web         ## Stop single container


restart – This will restart containers of the services defined in config file
$ docker-compose restart           ## Restart all containers
$ docker-compose restart web       ## Restart single container


pause – This will pause running containers for the services defined in config file.
$ docker-compose pause            ## Pause all containers
$ docker-compose pause web        ## Pause single container


unpause – This will start paused containers for the services defined in config file.
$ docker-compose pause            ## Start all paused containers
$ docker-compose pause web        ## Start single paused container


rm –
This will remove stopped containers for the services defined in config file.
$ docker-compose rm               ## Start all paused containers
$ docker-compose pause web        ## Start single paused container


