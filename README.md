# Guiding Principles and Long Term Goals of the Small Size League

English | [Japanese](README_ja.md)

This is the AsciiDoc source for the unofficial Japanese translation of RoboCup Small Size League guiding principles and long term goals.  
You can see original on [Small Size League official repository](https://github.com/robocup-ssl/ssl-goals).

## Build
The document is automatically built on updates to the master branch and published to [Github Pages](https://kkimurak.github.io/ssl-goals-ja/sslgoals.html).
There is also a [PDF-version](https://kkimurak.github.io/ssl-goals-ja/sslgoals.pdf).

### Using AsciiDoctor natively
Install AsciiDoctor on your system (https://asciidoctor.org/). Afterwards, build HTML5 version with
```
# Build the HTML5 version
asciidoctor sslgoals.adoc
# Build the PDF version
asciidoctor-pdf sslgoals.adoc
```

### Using docker image
If you have Docker installed, you can use the official AsciiDoctor image:
```
# Pull image once
docker pull asciidoctor/docker-asciidoctor
# Build the HTML5 version
docker run -v $PWD:/documents/ asciidoctor/docker-asciidoctor asciidoctor sslgoals.adoc
# Build the PDF version
docker run -v $PWD:/documents/ asciidoctor/docker-asciidoctor asciidoctor-pdf sslgoals.adoc
```
