# Development Status

Done
* docker images on github - https://hub.docker.com/u/klipperondocker
* klipper multi-platform build
* trigger klipper build on github master commit - one image per platform per commit
* klipper exposes serial port over ser2net
* octoprint multi-platform build
* trigger klipper build on github master commit - one image per platform per release
* octoprint uses socat to connect to serial port over network
* basic installation instructions - https://github.com/klipperondocker/docs
* basic dockerfile - https://github.com/klipperondocker/stack/blob/master/standard.yml

Being worked on
* automatically tag latest klipper image with ":latest"
* automatically tag latest octoprint stable release with ":latest"
* cleanup and publish dockerfile for octoprint
* cleanup and publish dockerfile for klipper
* web editor for configuration file(s) - visual studio code running in a docker image

To do list
* container with only ser2net to be able to run the stack via a network connection to printer ( klipper image will use socat to connect to generate a printer serial port )
* modify socat/ser2net to get over the 115200 bps limit or implement something else over the network
* upgrade to traefik 2 and add middleware to secure all web interface with the same octoprint user/passwords
* bash install script
* dwc docker image as alternate to octoprint

