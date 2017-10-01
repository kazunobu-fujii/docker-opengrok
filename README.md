# docker-opengrok

The one-liner to spin up a code search engine

## Usage

### run

```sh
$ docker run -d -v [path/to/source]:/src -p [public port]:8080 --name kazunobufujii/opengrok opengrok
```

### reindex

```sh
$ docker exec -it opengrok /usr/OpenGrok/bin/OpenGrok index /src
```

### view

```sh
$ open http://localhost:[public port]/source/
```

