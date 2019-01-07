To run the Dockerized version of the question generator 2 it's necessary to have Docker installed in your machine.

# Install Docker:

## Instructions on macOS:

Docker for Mac offers a Mac native application that installs in /Applications. It creates symlinks (symbolic links) in /usr/local/bin for docker and docker-compose to the Mac versions of the commands in the application bundle.

The Docker for Mac bundle installs:

Docker Engine
Docker CLI Client
Docker Compose
Docker Machine

## Mac Requirements


The Mac has to be from 2010 or newer, with Intel’s hardware Memory Management Unit (MMU).
OS X 10.10.3 Yosemite or newer (or macOS).
At least 4 GB of RAM.
You must not have a VirtualBox installation earlier than version 4.3.30 on your system. If you do, you’ll need to uninstall it.

## Installation:

Download Docker from https://download.docker.com/mac/beta/Docker.dmg.
Double-click the DMG file, and drag-and-drop Docker into your Applications folder.
You need to authorize the installation with your system password.
Double-click Docker.app to start Docker.
The whale in your status bar indicates Docker is running and accessible.
Docker presents some information on completing common tasks and links to the documentation.
You can access settings and other options from the whale in the status bar. a. Select About Docker to make sure you have the latest version.

Verify your versions:

$ docker --version
$ docker-compose --version
$ docker-machine --version

Run a Dockerized web server to make sure everything works:


$ docker run -d -p 80:80 --name webserver nginx

If you are presented with an nginx page your Docker install was successful.








# Running the deep learning algorithm

1. docker build -t algorithmsbilstm . (Remember to include the . at the end)
2. docker run algorithmsbilstm
