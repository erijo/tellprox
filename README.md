tellprox
========

A local server to use in place of Tellstick Live. Based on remotestick-server (https://github.com/pakerfeldt/remotestick-server)

Raspberry Pi telldus-core install instructions:
http://elinux.org/R-Pi_Tellstick_core

Installation
============

Make sure TelldusCenter is installed (TelldusCore.dll is needed for Windows)

Ensure Python is installed and setup (tested on Python 2.7 only).
All settings are contained within config.ini

cd ~

sudo apt-get install python-cherrypy3 python-bottle python-oauth python-configobj git

git clone --recursive git://github.com/p3tecracknell/tellprox.git

cd tellprox/telldus-py/

sudo python setup.py install

cd ..

sudo python -m tellprox
