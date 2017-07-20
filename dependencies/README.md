# Installed packages 

## DHCP and DNS

 * `sudo apt-get install isc-dhcp-server bind9` 

## FFMPEG/FFPLAY/FFSERVER
RPi uses a ARM CPU this means the software must be optimized "IN ORDER TO BE PROPERLY USED"

follow the walkthrough until you are ready to install ffmpeg:
 
* `https://trac.ffmpeg.org/wiki/CompilationGuide/RaspberryPi`

In the Raspberry , open a terminal and type this:

```
cd /usr/src
git clone git://source.ffmpeg.org/ffmpeg.git

cd ffmpeg
./configure
make && make install
```

##Install NGINX 

We need a webserver to serve the video on a Html page . To do so we use NGINX 
 * `sudo apt-get install ngnix`

#Python Dependencies
Use Python 2.7 

##Install Python-pip

We need to install pip to use  external libraries such as requests. We can do this by running:
 * `sudo apt-get install python2-pip`


###Install packages using pip

We need to install some packages for further use in python . We can do it by running :

 * `sudo pip2 install -r requirements.txt`