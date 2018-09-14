# DEPRECATED - DOCKER REGISTRY IS NOW HOSTED ON AZURE!!!!!!

# docker-registry

docker-compose and systemd scripts for running a private docker registry as a linux service

## Install

### Git clone to the root directory 

    $ git clone git@gitlab.engr.atlas:devOps/docker-registry.git /docker-registry
    
### Install the systemd unit file

    $ cd /docker-registry
    $ cp docker-registry@.service /etc/systemd/system/
    
### Re-load the systemctl daemon & start the service

    $ systemctl daemon-reload
    $ systemctl start docker-registry@.service