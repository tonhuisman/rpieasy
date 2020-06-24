If you like this project, or you wants to support the development, you can do that by:
- Buying a [coffee](https://ko-fi.com/I3I5UT4H)
- Direct [PayPal donation](https://www.paypal.me/rpieasy)
- Contributing to any of my [Wishlist items](https://www.wishlist.com/wishlists_/alexander-nagy/dwGnV/)
- Adding Python code by [Pull Request](https://github.com/enesbcs/rpieasy/pulls)

# RPIEasy

Easy MultiSensor device based on Raspberry PI

![RPIEasy](https://m.blog.hu/bi/bitekmindenhol/image/rpi_devs.png)

Based on Python 3.x and Raspberry PI (Raspbian Linux) this project tries to mimic the magnificent [ESPEasy](https://www.letscontrolit.com/wiki/index.php/ESPEasy) project functions.
Main goal is to create a multisensor device, that can be install and setup quickly. 

# Requirements
- Debian/Ubuntu/Raspbian Linux
- Python3

Tested with Raspberry Pi Zero W/Raspbian Buster and PC/Ubuntu 20.04. (may work with other Debian/Ubuntu derivatives)
For obvious reasons GPIO based devices needs GPIO support, mainly targeted for Raspberry Pi. 
However experimental Orange Pi and USB FTDI GPIO support also added for testing purposes. Some basic devices (dummy, system informations...) and controllers will work on a normal PC.

# Installation

    sudo apt install python3-pip screen alsa-utils wireless-tools wpasupplicant zip unzip git
    git clone https://github.com/enesbcs/rpieasy.git
    cd rpieasy
    sudo pip3 install jsonpickle

In case of Debian Stretch or other linux that misses "ifconfig" command:

`sudo apt install net-tools`

Other dependencies can be reached and installed through the webGUI after starting with: (See Hardware page)

`sudo ./RPIEasy.py`

# Update
There are an external updater and command line manager script by [haraldtux](/haraldtux):

https://github.com/haraldtux/rpieasy-update

Or you can use the integrated updater at Tools->System Updates, but be warned: save your "data" directory before update if it is containing data that you can't or won't readd manually!

# FAQ
In case of questions or problems:
- [Check the Wiki](https://github.com/enesbcs/rpieasy/wiki)
- [Check the Forum](https://www.letscontrolit.com/forum/viewforum.php?f=24&sid=73480306697e27e1e89fe9e67c18c7d6)
- [Make a new Issue](https://github.com/enesbcs/rpieasy/issues)
