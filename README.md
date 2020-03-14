# Docker-golang-dev-env
Easy golang development setup with docker
###
## Setup guide
* Create src pkg bin folders at root
  * `mkdir src pkg bin` 
* Start-up go container
  * `docker-compose run golang bash`
###
The reason to use a docker container for the golang enviroment is because setting up the enviroments variables could be hard for begginers.

You can still use your IDE of choice, edit the files as you would normally do. It mounts the root folder to the working directory of the container, which is `/go` so any changes made in the root folder would be automatically updated to the container and viceversa.

To exit the container just type `exit` and it would kill the container and kick you back to your normal terminal.

It is intended to be used in a linux enviroment. However, it still can be used in an windows system, but you may need to read about cross-compiling and how you may need to set it up [here](https://hub.docker.com/_/golang) in the cross-compile section. Read throu the docs and choose your OS and architecture.
