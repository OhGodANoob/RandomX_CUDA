# RandomX CUDA implementation

This repository contains full RandomX implementation for NVIDIA GPUs. The latest version of RandomX (as of May 15th, 2019) is supported.

Note: it's only a benchmark/testing tool, not an actual miner. RandomX hashrate is expected to improve somewhat in the future thanks to further optimizations.

GPUs tested so far:

Model|CryptonightR H/S|RandomX H/S|Relative speed
-----|---------------|-----------|--------------
GTX 1660 Ti max overclock (2070/13760 MHz)|626 (98 W)|671 (103 W)|107.2%
GTX 1660 Ti low power (1785/13760 MHz)|604 (70 W)|564 (70 W)|93.4%
GTX 1070 [[1]](https://termbin.com/g2z7)|612 (89 W)|609 (108 W)|99.5%
GTX 1070 Ti [[2]](https://termbin.com/orh3)|625 (97 W)|769 (123 W)|123.0%
GTX 1080 Ti [[3]](https://termbin.com/lgir)|787 (145 W)|1136 (190 W)|144.3%
RTX 2080 [[4]](https://termbin.com/cgxn)|828 (142 W)|1191 (189 W)|143.8%
RTX 2080 Ti [[5]](https://termbin.com/zt40)|1028 (191 W)|1692 (235 W)|164.6%

## Building on Windows

- Install Visual Studio 2017 Community and NVIDIA CUDA 10.1
- Open .sln file in Visual Studio and build it

## Building on Ubuntu

```
sudo apt install build-essential git nvidia-cuda-toolkit
git clone --recursive https://github.com/SChernykh/RandomX_CUDA/
cd RandomX_CUDA
make
```

## Donations

If you'd like to support further development/optimization of RandomX miners (both CPU and AMD/NVIDIA), you're welcome to send any amount of XMR to the following address:

```
44MnN1f3Eto8DZYUWuE5XZNUtE3vcRzt2j6PzqWpPau34e6Cf4fAxt6X2MBmrm6F9YMEiMNjN6W4Shn4pLcfNAja621jwyg
```
