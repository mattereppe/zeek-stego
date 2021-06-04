# zeek-stego
Zeek extensions to detect covert channels in IPv6 header

## Patch zeek source code

Clone the git repository.
See <A href="https://docs.zeek.org/en/master/install.html">instuctions</A>.

Enter the zeek folder and patch the code:
cd <zeek dir>/
patch -p0 < zeek.patch

(Patch build from zeek commit 3dac5ed80.)

Configure, compile and install zeek as explained in the <A href="https://docs.zeek.org/en/master/install.html">documentation</A>.

## Install the plugins with utils

TODO

## Run the zeek stego

Configure the stego.zeek file according to the monitored IPv6 header field:


...

/usr/local/zeek/bin/zeek -C -i <interface> stego.zeek 
  
Look for data in the stego-counters.log file.
