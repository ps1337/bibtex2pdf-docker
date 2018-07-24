# bibtex2pdf-docker

[![Build Status](https://travis-ci.org/ps1337/bibtex2pdf-docker.png?branch=master)](https://travis-ci.org/ps1337/bibtex2pdf-docker)

This downloads all references in a bibtex file as pdf if shorthands are used. If it doesn't make sense to download a file as pdf (e.g. png) it will try to save it in the native format.

## Building
Run `make build`. There's also an automated build at docker hub at `ps1337/bibtex2pdf-docker`

## Running
Use `make run` as non-root user and make sure the data folder can be accessed by your user. Be sure to provide the required file(s).

## Why did you disable chrome sandboxing?
Because some kernels still don't allow user namespaces.
