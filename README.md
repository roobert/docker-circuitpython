# Docker CircuitPython

## Abstract

Originally written to adjust maximum number of displays from 1 to 5.

Remove `sed` lines to use as a build process for vanilla circuitpython.

## Usage

```bash
docker rm -f circuitpython
docker build -t circuitpython .
docker run --name circuitpython circuitpython
docker cp circuitpython:/firmware/circuitpython-firmware.bin .
docker rm circuitpython
```
