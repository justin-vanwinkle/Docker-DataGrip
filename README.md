# Container for Housing a Development Environment
[![Build Status](https://travis-ci.org/justin-vanwinkle/Docker-DataGrip.svg?branch=master)](https://travis-ci.org/justin-vanwinkle/Docker-DataGrip)
 
__THIS CONTAINER IS NOT FOR PRODUCTION USE BUT FOR LOCAL DEVELOPMENT__

## Docker Run Scripts
Under `./bin` there is a simple bash script that  will build and execute
`docker run` commands for this container. You may either copy this script into
a location that is on your _PATH_ or you may add the `./bin` folder to your path.

Running a command like `./bin/datagrip.sh` would open the graphical portion of DataGrip on your desktop while its processes will be running in the container.

## Container information
This container extends the justinvanwinkle/dev-base image.
It is a complete container for using DataGrip.

This container is set up to have access to your local file system, so everything you do will persist.

## Know Issues:

- Your working directory must be with-in your host user's home directory.  Attempting run any of the containers outside of this will result in failure.
