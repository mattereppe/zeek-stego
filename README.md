# zeek-stego
Zeek extensions to detect covert channels in IPv6 header

## Patch zeek source code

Clone the git repository.
Patch zeek code:
patch -p0 < zeek.patch

(Patch build from zeek commit 3dac5ed80.)

## Install the plugins with utils

TODO

## Run the zeek stego

/usr/local/zeek/bin/zeek -C -i <interface> stego.zeek 
  
Look for data in the stego-counters.log file.
