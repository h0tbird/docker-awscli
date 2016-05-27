# docker-awscli

[![Build Status](https://travis-ci.org/h0tbird/docker-awscli.svg?branch=master)](https://travis-ci.org/h0tbird/docker-awscli)

AWS command line interface.

#### Show the command help:
```
docker run -it --rm h0tbird/awscli help
```

#### Download a file to the current working directory:
```
docker run -it --rm \
--volume ${HOME}/.aws:/root/.aws \
--volume ${PWD}:/aws \
h0tbird/awscli \
s3 cp s3://my_bucket/my_file .
```
