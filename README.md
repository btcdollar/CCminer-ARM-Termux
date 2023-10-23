# ccminer for ARM (cortex-a77)

Based on https://github.com/monkins1010/ccminer/tree/ARM

Termux Git and Build Process:
```
pkg update -y
pkg upgrade -y
pkg install openssl libjansson automake build-essential clang lld curl git binutils
git clone https://github.com/Marx1001/CCminer-ARM-Termux.git
cp /data/data/com.termux/files/usr/include/linux/sysctl.h /data/data/com.termux/files/usr/include/sys
cd CCminer-ARM-Termux
chmod +x build.sh
chmod +x configure.sh
chmod +x autogen.sh
CXX=clang++ CC=clang ./build.sh
```

For specific details on installing clang-16 on your current OS, check: https://apt.llvm.org/
