[![Circle CI](https://circleci.com/gh/caerusassociates/cliff_container.svg?style=svg)](https://circleci.com/gh/caerusassociates/cliff_container)

# cliff_compose
Dockerized CLIFF

This repo contains a Dockerfile for building MIT's CLIFF geolaocation server. CLIFF takes text as input and returns a structured list of the places the text is about. It is built on Berico Technologies' [CLAVIN](https://github.com/Berico-Technologies/CLAVIN) geotagging and geoparsing software and Stanford's
[CoreNLP](http://nlp.stanford.edu/software/corenlp.shtml) natural language parsing software.

Setup
--------

Build the image using `docker build` and run using `docker run`. The server is exposed on port 8080 and the endpoint can be reached like so:

```
http://localhost:8080/CLIFF-2.0.0/parse/text?q=In%20Syria,%20two%20airstrikes%20west%20of%20Al-Hasakah%20successfully%20struck%20multiple%20ISIL%20buildings,%20including%20an%20air%20observation%20building%20and%20staging%20areas.
```
