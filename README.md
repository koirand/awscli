awscli
===

Debian base Docker image include the following commands.

- awscli(v2)
- ekscli
- aws-iam-authenticator
- kubectl

Build

```
docker build -t koirand/awscli:latest .
```

Usage

```
docker run \
    -it \
    --rm \
    --name awscli \
    -v $HOME/.aws:/root/.aws \
    koirand/awscli:latest \
    /bin/bash
```
