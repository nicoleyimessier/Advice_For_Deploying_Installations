# Advice for Deploying Installations

## Checking your builds

### Test your software beforehand both with users and automated testing

There will always be bugs in your code at some point during the development process. You should try and catch these before getting onsite to install. Some bugs will only come up after many hours of use, so it’s good practice to run long form, automated testing. If you’re using xCode, run your applications using serialize and an automated test mode for as long as possible before install. 

### Test rebuilding your installation from zero before getting onsite

Learning how to rebuild your project before getting onsite will ensure you know the ins and outs of the equipment, as well as allow you to test all your equipment. Get together all the computers, wires, sensors, etc.c that you will be using and try building your setup. This will help you ensure all the cables and equipment are working, and you can debug the build process quickly.  

### Get to site as early as possible 

Things are always different then expected onsite -- get there early, so you can learn what constraints you are working within. 

### Version Control / Backup
Use Git to version control your software and all its dependencies. For example, if you’re working in openFrameworks, make all addons and openframeworks a submodule, so you always know what commits you are deploying with. This probably needs another write up...

## Make sure the installation stays up

### Watchdogs

Have a background script that launches your application automatically when it closes or crashes. 

### Heartbeats


### Restarts

Have a nightly shutdown and restart process to ensure software gets a fresh reboot each day.  

### One executable 

The less pieces to the system, the less dependencies that could cause issues/bugs. Don’t string different pieces of softwaretogether -- try to use APIs for services and design your architecture so that it's one executable. 

### If possible, never use wifi. 

LAN is your friend. 

### Bring back up of everything

Hardware seems to always fail onsite -- bring a backup of everything for this situation. Also, think about new or helpful hardware you may need onsite. For example, if you are putting up projections, a crosshair laser is helpful for aligning mesh grid points. 

## Clean up 

### Ensure All pop ups on your computer are disabled

### Hide your mouse

### All applications should launch in fullscreen mode

### Disable all automatic operating system updates

It’s likely you’ve tested your build using a specific operating system -- operating system updates are notorious for breaking software. Disable **ALL** updates, so you don’t have to deal with this. 

**This document is a WIP. Please feel free to add suggestions and edit. 





