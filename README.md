alpine-jvm8
=============

This image is the jvm8 base. It comes from rawmind/alpine-monit.

## Build

```
docker build -t rawmind/alpine-jvm8:<version> .
```

## Versions

- `1.8.144-2` [(Dockerfile)](https://github.com/rawmind0/alpine-jvm8/blob/1.8.144-2/Dockerfile)
- `1.8.112-1` [(Dockerfile)](https://github.com/rawmind0/alpine-jvm8/blob/1.8.112-1/Dockerfile)
- `1.8.102-2` [(Dockerfile)](https://github.com/rawmind0/alpine-jvm8/blob/1.8.102-2/Dockerfile)
- `1.8.92-7` [(Dockerfile)](https://github.com/rawmind0/alpine-jvm8/blob/1.8.92-7/Dockerfile)
- `1.8.74-1` [(Dockerfile)](https://github.com/rawmind0/alpine-jvm8/blob/1.8.74-1/Dockerfile)


## Usage

To use this image include `FROM rawmind/alpine-jvm8` at the top of your `Dockerfile`. Starting from `rawmind/alpine-monit` provides you with the ability to easily start any service using monit. monit will also keep it running for you, restarting it when it crashes.

To start your service using monit:

- create a monit conf file in `/opt/monit/etc/conf.d`
- create a service script that allow start, stop and restart function
