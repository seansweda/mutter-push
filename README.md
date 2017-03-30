# Mutter Push ZNC Module #

Mutter Push is a ZNC module for the Mutter IRC client.  It will send notifications to Apple's Push Notification Service for any messages that match your own nickname or keywords in the client settings; this includes: private messages, private notices, channel messages, and channel notices. **Note: notifications will only be sent if you are set to away.**

The module is work in progress, but should be stable enough for every day use.  It has been tested against ZNC 1.6.  Users are more than welcome to submit feature requests or patches for inclusion.


### Download ###

You can download the module from bitbucket:

```
#!

wget https://bitbucket.org/jmclough/mutter-push/get/master.zip
unzip -d mutter -j master.zip
cd mutter
```

### Dependencies ###

Install PIP which is used to install and manage software packages written in Python:


```
#!

$ sudo apt-get install python3-pip

```

Install Requests which is a HTTP library used by Mutter:

```
#!

$ sudo pip3 install requests
```


Load ModPython if not already loaded:

```
#!

/znc loadmod modpython

```

### Installation ###

Copy the Mutter ZNC module to your modules directory:

```
#!

$ cp mutter.py ~/.znc/modules/
```

Load the ZNC module:


```
#!

/znc loadmod mutter
```