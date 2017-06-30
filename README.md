# alpine-cloud-datastore-emulator

[![Docker Pulls](https://img.shields.io/docker/pulls/xaviiic/alpine-cloud-datastore-emulator.svg)]()
[![Docker Build Status](https://img.shields.io/docker/build/xaviiic/alpine-cloud-datastore-emulator.svg)]()
[![Docker Automated Build](https://img.shields.io/docker/automated/xaviiic/alpine-cloud-datastore-emulator.svg)]()

This is minimal Docker image for running cloud datastore emulator.
Reference and build from [Google Cloud SDK](https://hub.docker.com/r/google/cloud-sdk/) alpine-based image.

## Usage

To use this image, pull from [Docker Hub](https://hub.docker.com/r/xaviiic/alpine-cloud-datastore-emulator/).

```
docker pull xaviiic/alpine-cloud-datastore-emulator
```

Check the image content versions.

```
$ docker run -it xaviiic/alpine-cloud-datastore-emulator:latest gcloud version
Google Cloud SDK 161.0.0
cloud-datastore-emulator 1.2.1
```

You can start the emulator by,

```
$ docker run -it xaviiic/alpine-cloud-datastore-emulator:latest gcloud beta emulators datastore start --project=<project-id>
```

Further emulator setup can be found from the [official documentation](https://cloud.google.com/datastore/docs/tools/datastore-emulator).
