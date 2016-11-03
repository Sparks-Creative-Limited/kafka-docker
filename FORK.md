kafka-docker (fork)
===================

This fork, modifies the wurstmeister image by integrating and configuring zookeeper.  
The base image is replaced with the official Zookeper image and the command is replaced with `supervisord`.  
Configuration is added to the image for `supervisord` to launch the usual commands from the Zookeeper and Wurstmeister
images.

All environment settings that can be applied to the upstream images may also be applied here.  
An example `docker-compose-cluster.yml` file is included to demonstrate the deployment of a 3 node cluster.