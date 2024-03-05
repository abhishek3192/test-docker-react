## to build dockerfile

DOCKER_BUILDKIT=0 docker build -f Dockerfile.dev -t abhishek/docker:frontend-webapp .

## to run dockerfile

DOCKER_BUILDKIT=0 docker run -it -p 3000:3000 -v /home/node/app/node_modules -v /home/abhishek/docker/frontend-webapp:/home/node/app abhishek/docker:frontend-webapp
