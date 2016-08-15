docker-gitkraken
How it works
Get the install of gitkraken from the web and run it on docker container. Forked from myparkfolio (https://hub.docker.com/r/myparkfolio/docker-gitkraken/) and ported to debian:sid.

What's new
Just a container to run gitkraken on it.

How to use it
 docker run --name gitkraken -ti --rm \
   -v /tmp/.X11-unix:/tmp/.X11-unix \
   -e DISPLAY=$DISPLAY \
   -v $(pwd):/home/developer/data/ \
   -e UID=`id -u` -e GID=`id -g` \
   liftedkilt/docker-gitkraken
