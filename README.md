# Advice for Deploying Installations

## Checking your builds

### Test your software beforehand both with users and automatic testing

There will always be bugs in your code at some point during the development process. You should try and catch these before getting on sight to install. Some bugs will only come up after many hours of use, so it’s a good practice to run long form, automated testing. If you’re using xCode, run your applications using serialize and an automated test mode for as long as possible before install. 

### Test rebuilding your installation from zero before getting on sight

Learning how to rebuild your project before getting onsight will ensure you know the ins and outs of the equipment, as well as allow you to test all your equipment. Gather all the computers, wires, etc that you will be using and try rebuilding it. This will help you ensure all the cables and equipment are working, and you can debug the build process quickly.  

### Get to sight as early as possible 

Things are always different then expected onsight -- get there early, so you can learn what constraints you are working within early. 

### Version Control / Backup
Use Git to version control your software and all its dependencies. For example, if you’re working in openFrameworks, make all addons and openframeworks a submodule, so you always not what commits you are deploying with. This probably needs another write up...

## Make sure the installation stays up

### Watchdogs

Have a background script that launches your application automatically when it closes. 

### Restarts

Have a nightly shutdown and restart process to ensure software gets a fresh reboot each day.  

### One executable 

The less pieces to the system, the less dependencies that could cause issues/bugs. Don’t string different pieces of software/services together -- try to use APIs and get your architecture down to one executable. 

### If possible, never use wifi. 

LAN is your friend. 

### Bring back up of everything

Hardware seems to always fail onsight -- bring a backup of everything for this situation. Also, think about new hardware you may need on sight. 

## Clean up 

### Ensure All pop ups on your computer are disabled

### Hide your mouse

### All applications should launch in fullscreen mode

### Disable all automatic operating system updates

It’s likely you’ve tested your build using a specific operating system -- operating system updates are notorious for breaking things. Disable the update, so you don’t have to deal with this. 

**This document is a WIP. Please feel free to add suggestions and edit. 





