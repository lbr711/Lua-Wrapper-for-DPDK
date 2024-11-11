# Lua-Wrapper-for-DPDK
## libmoon 
[libmoon](https://github.com/libmoon/libmoon) is the Lua wrapper for DPDK. We can use libmoon framework to develop DPDK applications by Lua script.

## MoonGen
libmoon started out as the packet generator [MoonGen](https://github.com/emmericp/MoonGen.git) which evolved into a more general framework for packet processing.

## Installation for libmoon
Note that we should git clone the libmoon repository under the dpdk-19.05 branch; otherwise, some mistakes will appear owing to the header file being missing. 
```shell
git clone https://github.com/libmoon/libmoon.git --branch=dpdk-19.05
cd libmoon
./build.sh
```

## Installation for MoonGen
```shell
git clone https://github.com/emmericp/MoonGen.git --branch=dpdk-19.05
rm -fr libmoon
git clone https://github.com/libmoon/libmoon.git --branch=dpdk-19.05
cd libmoon
./build.sh ../build --moongen
```
