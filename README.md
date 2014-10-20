debian-webdis-armhf
===================

A debian package of the webdis server for the armhf platform.

## Building the package

Here is a quick and dirty way to build it:

```sh
git clone https://github.com/AutogrowSystems/debian-webdis-armhf.git
rm debian-webdis-armhf/LICENCE    # delete these so they don't polute your root
rm debian-webdis-armhf/COPYING
rm debian-webdis-armhf/README.md
fakeroot dpkg-deb -b debian-webdis-armhf webdis_0.1.1_armhf.deb
```

Or install [dpkg-git](http://penguinpowernz.github.io/dpkg-git/) and do it like this:

```sh
git clone https://github.com/AutogrowSystems/debian-webdis-armhf.git
cd debian-webdis-armhf
fakeroot git deb
```