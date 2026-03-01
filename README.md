# Meshtastic Workshop resources

## Step 1

First, ensure you have python installed on your system. [The guide on Real Python](https://realpython.com/installing-python/) is good. Follow the directions for your operating system.

We recommend installing Python v3.13.1

## Step 2

Once you have python installed, run the following command. 

```
$ python3 -m venv venv
$ source venv/bin/activate   # or venv\Scripts\activate on Windows
$ pip3 install -r requirements.txt
```

This creates a `venv` of all the required tooling for our workshop:

1. `protobuf` v4.25.8
1. [Meshtastic CLI](https://meshtastic.org/docs/software/python/cli/)
1. [PlatformIO Core](https://docs.platformio.org/en/latest/core/installation/index.html)
1. [`esptool`](https://pypi.org/project/esptool/)

## Step 3

You'll want to manually install a Chrome-based browser as well as the [CP210x serial drivers](https://meshtastic.org/docs/getting-started/serial-drivers/esp32/).

## Step 4

By the end of this setup process, you should be able to verify most of the tooling by running:

```
$ meshtastic --version
2.7.7

$ pio --version
PlatformIO Core, version 6.1.19

$ esptool version
esptool v5.1.0
5.1.0
```
