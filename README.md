# Lua-Wrapper-for-DPDK
## libmoon 
[libmoon](https://github.com/libmoon/libmoon) is the Lua wrapper for DPDK. We can use libmoon framework to develop DPDK applications by Lua script.

## MoonGen
libmoon started out as the packet generator [MoonGen](https://github.com/emmericp/MoonGen.git) which evolved into a more general framework for packet processing.

## Installation for libmoon
```shell
git clone https://github.com/libmoon/libmoon.git
cd libmoon
git checkout dpdk-19.05
git submodule update --init
./build.sh
```

Note that: when using the gcc version after 7.0 to build DPDK (libmoon uses DPDK up to 19.08), there will appear "fallthrough" warnings being treated as errors. we need to manually add '-w' to 'CFLAGS' in the makefiles included within both the directory "yourPath2dpdk/kernel/linux/kni/Makefile" and the directory "yourPath2dpdk/kernel/linux/igb_uio/Makefile".

## Installation for MoonGen
```shell
git clone https://github.com/emmericp/MoonGen.git
git checkout dpdk-19.05
git submodule update --init
./build.sh
```

Note that: as the same to the libmoon installation.
