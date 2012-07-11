xvfb-init
=========

Xvfb lsb init script for debian systems

installation
============

* Copy the script to /etc/init.d/
* invoke as root
    update-rc.d Xvfb defaults
* Optionally create the file /etc/default/Xvfb
  and override the default values for DAEMON_ARGS and PIDFILE variables:
    DAEMON_ARGS=":99 -ac -screen 0 1024x768x16"
    PIDFILE=/var/run/my_custom_xvfb.pid

notes
=====

Only tested on debian systems (*may* work in ubuntu)
