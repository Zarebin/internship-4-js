## For using this reopsitory after you cloned you must build image:
docker build -t docker-react
Instead of docker-react you can name whatever you want as your  image name

## After building our image now you are ready for to run your image:
docker run -d -p 8080:80 docker-react
Instead of docker-react you must use whatever you named your image
The -d option specifies that the container runs in detached mode: the container continues to run until stopped but does not respond to commands run on the command line
The -p option tells Docker to map the ports exposed in the container by the NGINX image (port 80) to the specified port on the Docker host. The first parameter specifies the port in the Docker host, the second parameter is mapped to the port exposed in the container
