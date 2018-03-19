# RavenDB-docker-arm
RavenDB for docker on arm devices

## Why not use the official ravendb docker image?
The official ravenDB docker image does sadly not support arm devices and afaik there are no docker images out there supporting arm devices. RavenDB has (on their download page) versions for the rasperry pi, but sadly does not provide a docker image built on that. This dockerfile is almost an exact copy of their ubuntu image with ubuntu for arm.

## Building the image
You still need to provide a version of raven-db in the same directory as the dockerfile named *RavenDB.tar.bz2*.<br/>
You can get a version of ravenDB [here](https://ravendb.net/download).<br/>
You will also need a *settings.json* file containing some initial settings. For more information on how to set this up visit [ravendb's docs](https://ravendb.net/docs/article-page/4.0/csharp/server/configuration/configuration-options)

## What exactly is this?
Well the dockerfile and both scripts in this repo are basically copies of the [official image's](https://hub.docker.com/r/ravendb/ravendb/) docker setup (found [here](https://github.com/ravendb/ravendb/tree/v4.0/docker/ravendb-ubuntu1604)), but the ubuntu image has been switched for an arm version that can run on the rasperry pi or similar arm devices. Thats actually all there is to it.