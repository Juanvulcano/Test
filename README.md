To run the Dockerized version of the question generator 2 it's necessary to have Docker installed in your machine.

# Installing Docker:

## Instructions on macOS:

Docker for Mac offers a Mac native application that installs in /Applications. It creates symlinks (symbolic links) in /usr/local/bin for docker and docker-compose to the Mac versions of the commands in the application bundle.

The Docker for Mac bundle installs:

Docker Engine

Docker CLI Client

Docker Compose

Docker Machine

### Requirements


The Mac has to be from 2010 or newer, with Intel’s hardware Memory Management Unit (MMU).

OS X 10.10.3 Yosemite or newer (or macOS).

At least 4 GB of RAM.

You must not have a VirtualBox installation earlier than version 4.3.30 on your system. If you do, you’ll need to uninstall it.

### Installation:

Download Docker from https://download.docker.com/mac/beta/Docker.dmg.
Double-click the DMG file, and drag-and-drop Docker into your Applications folder.
You need to authorize the installation with your system password.
Double-click Docker.app to start Docker.
The whale in your status bar indicates Docker is running and accessible.
Docker presents some information on completing common tasks and links to the documentation.
You can access settings and other options from the whale in the status bar. a. Select About Docker to make sure you have the latest version.

Verify that your versions match below:

$ docker --version
Docker version 18.09.0, build 4d60db4

$ docker-compose --version
docker-compose version 1.23.2, build 1110ad01

$ docker-machine --version
docker-machine version 0.16.0, build 702c267f

Run a Dockerized web server to make sure everything works:

$ docker run -d -p 80:80 --name webserver nginx

If you are presented with an nginx page your Docker install was successful.


## Installing on Windows10:

### Requirements
Docker for Windows runs on 64-bit Windows 10 Pro, Enterprise, and Education; 1511 November update, Build 10586 or later. Docker plans to support more versions of Windows 10 in the future.

### Installation
Download Docker from https://download.docker.com/win/beta/InstallDocker.msi.
Double-click InstallDocker.msi to run the installer.
Follow the Install Wizard: accept the license, authorize the installer, and proceed with the install.
Click Finish to launch Docker.
Docker starts automatically.
Docker loads a “Welcome” window giving you tips and access to the Docker documentation.


# Running the deep learning algorithm

1. docker build -t algorithmsbilstm . (Remember to include the . at the end)
2. docker run algorithmsbilstm
