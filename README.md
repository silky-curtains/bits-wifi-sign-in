## Introduction

Desgined particularly for BITS-GOA students, this is a simple bash script which enables you to connect to the college wifi directly from any unix-based terminal.

Since a unix-based termianal is required, this bash script will only work on Linux and macOS.

## Basic Usage

Ensure you're connected to the wifi, and run the following command to automatically login to the college wifi.

```
$ bits-login
```

## Setup

First, clone the repository to any directory of your choie.

```
$ git clone 
```

Open the file `bits-login.sh` in the editor of your choice, and change the variables `BITS_USERNAME` and `BITS_PASSWORD` to match your own credentials. (the provided credentials are for example purposes and won't work, so make sure you do this step)

Make the script executable by running the following command:

```
$ chmod +x bits-login
```

To be able to execute your custom command from anywhere, move it to a directory that's listed in your system's PATH. Common directories include `/usr/local/bin` or `~/bin` (if it exists)

```
$ mv bits-login /usr/local/bin
```

Now you should be able to connect to the wifi by running

```
$ bits-login
```

And a response similar to the following will be printed in your terminal

```
<?xml version='1.0' ?><requestresponse><status><![CDATA[LIVE]]></status><message><![CDATA[You are signed in as {username}]]></message><logoutmessage><![CDATA[You have successfully logged off]]></logoutmessage><state><![CDATA[]]></state></requestresponse>
```

## How to change name of executable
If you want to rename the command from `bits-login` to something of your convinience, first change the name of the file from `bits-login.sh` to (for example) `wifi-login.sh` by the following commmand:

```
$ mv bits-login.sh wifi-login.sh
```

from here on, follow the Setup procedure just as described, but replace `bits-login` by your custom name.
