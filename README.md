# Building a .deb package

GMail web app, base on firefox.

## Build the .deb

gmail/ is the directory containing DEBIAN/.

Extract the content of the brave-browser archive, containing the brave binary and its librairies into
usr/local/gmail/.

```
cd .. 
dpkg-deb --build gmail
```

## Install the .deb

```
sudo apt install ./gmail.deb
```
