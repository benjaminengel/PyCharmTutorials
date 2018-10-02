# README
This is a skeleton project for working with a remote interpreter in PyCharm.

All dependencies are handeld in the requirement.txt which will be used during the docker build process.
The chosen base image provies a workin jupyter notebook enviorment. 

All files under src will be copied to the image during build time and be present under /home/jovyan/work later on.

It is suggested to bind mount the src folder during development to the directory /home/jovyan/work for convinience.

In PyCharm it is needed to mount the port 8888 to a local port for the connection to the jupyter notebook server.