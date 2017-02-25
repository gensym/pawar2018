# Welcome to Pawar 2018 Repo

## Getting started (Mac)
1. Install Docker (www.docker.com)
2. Clone the repo
````
    git clone git@github.com:pawar-2018/pawar2018.git
````    
3. Start the docker container
````
    docker-compose up -d
````    
4. Go to http://localhost:8000

## Getting started (Windows)
1. Install Docker Toolbox on Windows (https://docs.docker.com/toolbox/toolbox_install_windows/)
2. Clone the repo
````
    git clone git@github.com:pawar-2018/pawar2018.git
````
3. Start the docker container
  1. You might need to change the volumes for Wordpress to:
       ```- /wp-content/themes/pawar2018:/var/www/html/wp-content/themes/pawar2018```
````
    docker-compose up -d
````
4. Open Oracle VM and look for your Docker VM(default)
5. Right click docker VM(default) and select Settings > Shared Folders
6. Mount the location where you clone the repo into by adding a shared folder
    Folder Path EX: C:\github\username\pawar2018\wp-content
    Folder Name EX: wp-content
7. You might need to restart the VM if it doesn't mount the folder path
8. Once you see the files in the VM console(double click the VM for console), fetch your IP in the Docker terminal
with docker-machine ip
9. Go to http://docker-machine-ip-here:8000

## URLS

* Production (master) http://ameyapawar2018.wpengine.com
* Staging (dev) http://ameyapawar2018.staging.wpengine.com
* Localhost http://localhost:8000

## README TODOS

* Update dev setup instructions
* Add coding standards
* Add integration standards
* Add git strategy