# ssl-hardware-challenge-rules

This is the AsciiDoc source for the hardware challenge rules for RoboCup 2021.

## Build
The rules are automatically built on updates to the master branch and published to [Github Pages](https://robocup-ssl.github.io/ssl-hardware-challenge-rules/rules.html). There is also a [PDF-version](https://robocup-ssl.github.io/ssl-hardware-challenge-rules/rules.pdf).

### Using AsciiDoctor natively
Install AsciiDoctor on your system (https://asciidoctor.org/). Afterwards, build HTML5 version with
```
# Build the HTML5 version
asciidoctor rules.adoc
# Build the PDF version
asciidoctor-pdf rules.adoc
```

### Using docker image
If you have Docker installed, you can use the official AsciiDoctor image:
```
# Pull image once
docker pull asciidoctor/docker-asciidoctor
# Build the HTML5 version
docker run -v $PWD:/documents/ asciidoctor/docker-asciidoctor asciidoctor rules.adoc
# Build the PDF version
docker run -v $PWD:/documents/ asciidoctor/docker-asciidoctor asciidoctor-pdf rules.adoc
```
