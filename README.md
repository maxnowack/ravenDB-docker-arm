# RavenDB-docker-arm
RavenDB for docker on arm devices

## Why not use the official ravendb docker image?
Well the dockerfile and both scripts in this repo are basically copies of the [official image](https://hub.docker.com/r/ravendb/ravendb/), but the ubuntu image has been switched for an arm version that can run on the rasperry pi.

## Building the image
You still need to provide a version of raven-db in the same directory as the dockerfile named *RavenDB.tar.bz2*. Get your version of ravenDB [here](https://ravendb.net/download).
You will also need a *settings.json* file containing some initial settings. For more information on how to set this up visit [ravendb's docs](https://ravendb.net/docs/article-page/4.0/csharp/server/configuration/configuration-options)

## What exactly is this?
This is basically a copy of the dockerfile and configuration found in ravendb's repo under their docker folder. It has been adjusted to be usable on arm which there was no official (docker) version available at the time of writing this (It would be amazing to add support for arm, especially since its such a small change).