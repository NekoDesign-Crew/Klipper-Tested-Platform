# Orange Pi Zero Debian

## Image

[Debian image (orangepi.org)](http://www.orangepi.org/downloadresources/orangepizero_zerolts/2020-01-16/orangepizerolts_fb522ee7a3641224c632.html)

## Default Account and Password

- user: root
- password: orangepi 

## Install Guide

### Flash SD Card

Download [balenaEtcher](https://www.balena.io/etcher/) and install.

Plug SD card to the computer.

Select the image and SD card. (Important! This process will format the `SD Card` !)

### SSH

Once the system has been flashed to the SD card. Insert the SD card into the SD card slot of the Orange Pi then connect the power and network cable. Than following the step below.

#### Windows

Open `Windows Terminal`. Then using `ssh root@orangepi.local` to connect Orange Pi Zero. 

Make sure `orangepi.local` is your Orange Pi IP address.

#### macOS

Open `Terminal`. Then using `ssh root@orangepi.local` to connect Orange Pi Zero.

Make sure `orangepi.local` is your Orange Pi IP address.

#### Linux (Debian)

Install `openssh-client` by using `sudo apt install openssh-client`

Then using `ssh root@orangepi.local` to connect Orange Pi Zero.

### Setup User Account

Follow the SSH Hints to install and configure your account. 

(This part will complete later)

### Install Requirement

```shell
sudo apt-get update
sudo apt-get upgrade
sudo apt install git
```

### Install Klipper with KIAUH

GitHub

```shell
cd ~
git clone https://github.com/th33xitus/kiauh.git
kiauh/kiauh.sh
```

Gitee 

```shell
cd ~
git clone https://gitee.com/miroky/kiauh.git
./kiauh/kiauh.sh
```
