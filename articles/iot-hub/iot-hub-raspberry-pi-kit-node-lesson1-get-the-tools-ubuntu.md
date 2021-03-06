---
title: Get the tools (Ubuntu 16.04) | Microsoft Docs
description: Download and install the necessary tools and software for the first sample application for Pi on Ubuntu.
services: iot-hub
documentationcenter: ''
author: shizn
manager: timlt
tags: ''
keywords: 'iot development, iot software, internet of things software, install git on ubuntu, gulp run, install node js ubuntu'

ms.assetid: 4d5e45c0-1db9-4662-a039-99ba26333085
ms.service: iot-hub
ms.devlang: node
ms.topic: article
ms.tgt_pltfrm: na
ms.workload: na
ms.date: 11/28/2016
ms.author: xshi

---
# Get the tools (Ubuntu 16.04)

> [!div class="op_single_selector"]
> * [Windows 7 or later](iot-hub-raspberry-pi-kit-node-lesson1-get-the-tools-win32.md)
> * [Ubuntu 16.04](iot-hub-raspberry-pi-kit-node-lesson1-get-the-tools-ubuntu.md)
> * [macOS 10.10](iot-hub-raspberry-pi-kit-node-lesson1-get-the-tools-mac.md)


## What you will do
Download the development tools and the software for the first sample application for Raspberry Pi 3. If you have any problems, look for solutions on the [troubleshooting page](iot-hub-raspberry-pi-kit-node-troubleshooting.md).

## What you will learn
In this article, you will learn:

* How to install Git and Node.js.
  * [Git](https://git-scm.com) is an open source distributed version control system. The sample application for this article is stored on Git.
  * [Node.js](https://nodejs.org/en/) is a JavaScript runtime with a rich package ecosystem.
* How to use NPM to install additional Node.js development tools.
  * The minimum required version of Node.js is 4.5 LTS.
  * [NPM](https://www.npmjs.com) is one of the package managers for Node.js.

## What do you need
To complete this operation, you will need:

* An Internet connection to download the development tools and the software.
* A computer that is running Ubuntu 16.04 or later.

## Install Git, Node.js, and NPM
Use the keyboard shortcut `Ctrl + Alt + T` to open a terminal and run the following commands:

```bash
sudo apt-get update
curl -sL https://deb.nodesource.com/setup_6.x | sudo -E bash -
sudo apt-get install -y nodejs
sudo apt-get install git
```

## Install additional Node.js development tools
You use [gulp.js](http://gulpjs.com) to automate the deployment of the sample application to Pi. You also use the [device-discovery-cli](https://github.com/Azure/device-discovery-cli) to retrieve network information about your IoT devices.

Install `gulp` and `device-discovery-cli` by running the following command in the terminal:

```bash
sudo npm install -g device-discovery-cli gulp
```

If you experience issues installing Node.js and these additional development tools on Ubuntu, see the [troubleshooting guide](iot-hub-raspberry-pi-kit-node-troubleshooting.md) for solutions to common problems.

## Install Visual Studio Code
[Download](https://code.visualstudio.com/docs/setup/linux) and install Visual Studio Code. Visual Studio Code is a lightweight but powerful source code editor for Windows, Linux, and macOS. You use this editor later in the tutorial to edit the sample code.

## Summary
You've installed the required development tools and software for the first sample application. The next task is to create, deploy, and run the sample application on Pi.

## Next steps
[Create and deploy the blink sample application](iot-hub-raspberry-pi-kit-node-lesson1-deploy-blink-app.md)

