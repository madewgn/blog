---
title: "Install Speedtest on Linux"
date: 2023-04-03T22:18:18Z
tags:
  - Speedtest
  - linux
image: https://telegra.ph/file/e29a20025e448ba165c45.jpg
comments: false
---


Speedtest CLI is a command-line interface tool that allows you to test your internet speed from the terminal. This tool is useful for network administrators, developers, and anyone who wants to check their internet speed quickly and easily. In this article, we will guide you through the process of installing Speedtest CLI on your computer.

Step 1: Install Dependencies

Before installing Speedtest CLI, you need to make sure that you have the necessary dependencies installed on your system. These dependencies include Python and pip. To check if you have Python installed, open a terminal and type:

Copy code
```bash
python --version
```
If you don't have Python installed, you can download it from the official website: https://www.python.org/downloads/

Once you have Python installed, you can install pip by running the following command:

Copy code
```bash
sudo apt install python3-pip
```
Step 2: Install Speedtest CLI

To install Speedtest CLI, you can use pip by running the following command:

Copy code

```bash

pip install speedtest-cli
```

This command will download and install Speedtest CLI and all its dependencies.

Step 3: Test Speedtest CLI

To test if Speedtest CLI is installed correctly, run the following command:

Copy code
```bash
speedtest-cli
```
This command will run a speed test and display the results in the terminal. The results will include your download and upload speeds, as well as your ping time.
and you can use this commad to install Speedtest cli with out pip

```bash
sudo apt-get install curl
curl -s https://packagecloud.io/install/repositories/ookla/speedtest-cli/script.deb.sh | sudo bash
sudo apt-get install speedtest
```


Step 4: Optional - Install Speedtest CLI via Homebrew

If you're using a Mac and have Homebrew installed, you can install Speedtest CLI using the following command:

Copy code
```
brew install speedtest-cli
```

This will download and install Speedtest CLI and its dependencies.

Conclusion

Installing Speedtest CLI is a simple and straightforward process. Once you have it installed, you can quickly and easily check your internet speed from the terminal. With this tool, you can quickly diagnose network problems, troubleshoot internet speed issues, and ensure that your internet connection is performing at its best.







