# docker-jenkins-node-android-sdk

Dockerfile for jenkins nodes that need to build android projects. It currently
support api27.

## Usage

Grab from docker cloud with: `docker pull narfman0/jenkins-node-android-sdk`

You must have jenkins security enabled, which yields a secret per-node. Then
you should have name, secret, and host/ip needed to run:

`docker run --user jenkins narfman0/jenkins-node-android-sdk:latest -url http://$JENKINS_HOST:8080 $NODE_SECRET $NODE_NAME`

## License

Copyright 2018 Jon Robison

See LICENSE for details
