# The content and configuration of Nginx is simplistic, and can be invoked with:

$ docker container run --rm -d -p 80:80 -e COLOR=blue sauravsrivastav/fluxcd:v1

# To add the hostname of the Docker host to the served content, set the NODE_NAME environment variable for the container:

$ docker container run --rm -d -p 80:80 -e NODENAME=$(hostname) sauravsrivastav/fluxcd:v1