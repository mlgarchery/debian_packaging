# Building a .deb package

Example with  a Gmail web app, based on Brave Browser.

## Build the .deb

Find the latest release of Brave https://github.com/brave/brave-browser/releases.
Extract the content of the `brave-browser-nightly-<version>-linux-amd64.zip` archive, containing the brave binary and its librairies into
gmail/usr/local/gmail/.

```
dpkg-deb --build gmail
```

Will build whatever is in the gmail/ dir into your fs
That's why I put files under a directory, otherwise the .git is included.

##  Install the .deb

```
sudo apt install ./gmail.deb
```

Tada!
