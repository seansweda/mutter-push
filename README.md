# README #

Mutter Push is a ZNC module that provides push notification capability to the Mutter IRC client.

### Download Module ###

You can download the module from bitbucket:

```
#!

wget https://bitbucket.org/jmclough/mutter-push/get/master.zip
unzip -d mutter -j master.zip
cd mutter
```

### Prerequisites ###

Install PIP which is a package management system used to install and manage software packages written in Python:


```
#!

$ sudo apt-get instll python3-pip

```

Install Requests which is a HTTP library used by Mutter:

```
#!python

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
#!python

$ cp mutter.py ~/.znc/modules
```

Load the ZNC module:


```
#!python

/znc loadmod mutter
```