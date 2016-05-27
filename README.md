# docker-awscli

[![Build Status](https://travis-ci.org/h0tbird/docker-awscli.svg?branch=master)](https://travis-ci.org/h0tbird/docker-awscli)

AWS Command line interface

Show the command help:
```
docker run -it --rm h0tbird/awscli help
```

Download a file to the current working directory:
```
docker run -it --rm -v ${PWD}:/aws h0tbird/awscli --region eu-west-1 s3 cp s3://my_bucket/my_file .
```
