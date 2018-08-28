参考: [Run a single Node.js script](https://github.com/nodejs/docker-node/blob/master/README.md#run-a-single-nodejs-script)

```sh
docker run -it --rm \
    --name my-running-script \
    -v "$PWD":/usr/src/app \
    -w /usr/src/app \
    node:8 \
    npx create-react-app my-app
```

```sh
docker run -it --rm \
    --name my-running-script \
    -p 8080 \
    -v "$PWD":/usr/src/app \
    -w /usr/src/app \
    node:8 \
    /bin/bash
```