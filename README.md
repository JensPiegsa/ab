# Dockerized Apache Benchmark

* [Dockerfile](https://github.com/JensPiegsa/ab/blob/master/Dockerfile)

## Usage

### Show help

```sh
docker run --rm ab
```

### Start web server and run a simple load test

```sh
docker run -d --name=web nginx && \
docker run --rm piegsaj/ab -c 20 -n 1000 http://192.168.99.100/
```
