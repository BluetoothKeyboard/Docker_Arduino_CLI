![https://github.com/BluetoothKeyboard/Docker_Arduino_CLI/actions](https://github.com/BluetoothKeyboard/Docker_Arduino_CLI/workflows/Build%20Docker%20Image/badge.svg)

## Using the image

The image is available on [docker hub](https://hub.docker.com/repository/docker/bluetoothkeyboard/arduino-cli/general). 

To use the docker image, do a docker pull, then you can call the CLI as part of the docker run command.

Note that to see your sketch, the working directory must be mounted in the image.

```
docker pull bluetoothkeyboard/arduino-cli

docker run -it --mount src=${PWD},target=/mnt,type=bind  bluetoothkeyboard/arduino-cli:latest arduino-cli

```


## Building the image yourself

```

 docker build .

```
