vagrant-tomcat
===============

Tomcat 8 in a Vagrant VM

What You'll need
================

1. Recent version of Vagrant 
2. Recent version of VirtualBox
3. Disk space and memory for a VM

Usage
=====

Start the Vagrant machine with 'vagrant up'.

Put a .war file in ./webapps to install into Tomcat 8.

localhost:8080 is mapped by the Vagrantfile to the running Tomcat in the VM.

Notes
=====

It uses a bento box (see https://github.com/chef/bento).

Port mapping is done in the Vagrantfile.

Anything in the ./webapps, ./log, and ./conf folders isn't committed to Git, so the VM should stay small and can be readily destroyed at will (although I've not yet tested this... it's quite likely the conf folder will get overwritten)

