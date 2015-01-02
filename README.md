# MongoDB driver for Python Twisted

txmongo is a Python/Twisted driver for MongoDB that implements the wire
protocol on non-blocking sockets. The API derives from the original pymongo.

## Installing

You can use setuptools to install:

```sh
sudo python setup.py install
```

## Docs and examples

Generate them with `make docs`. You will need `epydoc` installed.
There are some examples in the *examples/* directory.

## Hacking

Run `make env` to create clean hacking environment with `virtualenv`.
Run `make` to torture your code with tests and code style tools.

## Packages

### Debian

Packing for debian exists in *debian/*, you can build yourself a package
(remember to update debian/changelog) if you make changes.

```sh
dpkg-buildpackage -b
```

Then look for the package in your home directory.

### Fedora

```sh
rpmbuild -bb python-txmongo.spec
```

You might need to download Source0 from the .spec and place it in
rpmbuild/SOURCES first.
