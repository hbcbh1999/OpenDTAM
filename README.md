OpenDTAM for Opencv 3.4
========

An open source implementation of DTAM

Based on Newcombe, Richard A., Steven J. Lovegrove, and Andrew J. Davison's "DTAM: Dense tracking and mapping in real-time."

This project depends on qtbase5-dev, [OpenCV 3](https://github.com/Itseez/opencv "OpenCV") and [Cuda](https://developer.nvidia.com/cuda-downloads "Cuda").

## Build Instructions on Ubuntu 16.04

Tested in this environment

* Ubuntu 16.04 x64
* GCC 5.4.0
* Boost 1.5.8
* OpenCV 3.4.0
* Cuda Toolkit 8.0

installation instructions are in "install-OpenDTAM.sh"

### Build OpenDTAM
```bash
cd OpenDTAM
mkdir build
cd build
cmake ../Cpp
make -j4
````

### Run OpenDTAM
For the following command, replace `$TRAJECTORY_30_SECONDS` with the path to the directory of the same name.
```bash
./a.out $TRAJECTORY_30_SECONDS
```
Assuming you are executing this command from the build folder, as shown above, enter the following:
```bash
./a.out ../Trajectory_30_seconds
```
