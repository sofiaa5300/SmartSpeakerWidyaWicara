# SmartSpeakerWidyaWicara
To run the Smart Speaker, follow the steps bellow :

## 1. Host Setup

The required packages for supporting Ubuntu distribution as the host development system are shown in the following command:
1. Open Ubuntu terminal
Press CTRL+ALT+T in the blank area
> ubuntu@ubuntu-virtual-machine:~

2. Run cmd in Ubuntu terminal
> $ sudo apt-get install gawk wget git-core diffstat unzip texinfo gcc-multilib build-essential chrpath socat libsdl1.2-dev xterm g++ libstdc++6 libpulse-dev libevent-dev ninja-build rpm2cpio

> $ wget -O gn http://storage.googleapis.com/chromium-gn/3fd43e5e0dcc674f0a0c004ec290d04bb2e1c60e

> $ sudo chmod 777 gn

3. Put the gn in build 
> server/usr/bin/

## 2. Build Source Code
To build source code, perform the following steps in Ubuntu terminal

1. Sync all compile
> ubuntu@ubuntu-virtual-machine:~/MT8516folder/hcn_overlay$ ./Sync_all_compile.sh

2. Set environment
> ubuntu@ubuntu-virtual-machine:~/MT8516folder$ . env.sh 06d_32b

The output shown below :

> ======================================================================================

> platform : bwd06 32b

> ======================================================================================

3. Build source code
> ubuntu@ubuntu-virtual-machine:~/MT8516folder/build$ ./mybuild.sh

## 3. Run Smart Speaker

After a build is completed, you can run the Speaker
1. Open Ubuntu Terminal
> ubuntu@ubuntu-virtual-machine:~MT8516/build/tmp/deploy/images/bwd06l-consys-emmc-128-32b$

2. Run smart speaker
> ubuntu@ubuntu-virtual-machine:~MT8516/build/tmp/deploy/images/bwd06l-consys-emmc-128-32b$ python flashimage_adb.py
