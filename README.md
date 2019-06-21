# Code-Server Docker Image #

## Author ##

Teng Fu

Email: teng.fu@teleware.com

## Base Image ##
This is the docker image for generating JNI library (.so/.a file) for Android development.

## Additional installed packages ##

- Code-Server

- Anaconda

- JDK, JRE ver 8

- Virsual Stuido Code Extension:
	
	- Java Extension Package

	- Microsoft C++ Extension

	- CMaketool Extension

	- Extension stored at: "/root/.vscode/extensions"

- Bazel

- Android-SDK

- Android-NDK


## Docker Registry Repo ##

-  tftwdockerhub/android_jni_lib_build:latest

## Usage ##

on virtual machines


```
sudo docker pull tftwdockerhub/android_jni_lib_build:latest
```

remember the target port is __8889__
```
sudo docker run -p 8889:8888 -v -v \<project-dir-path\>:/app tftwdockerhub/vscodeandroid:latest
```

In local browser, remember the target port is __8889__ and the token string on CLI screen
```
http://\<vm-ipaddress-or-dns\>:8889
```