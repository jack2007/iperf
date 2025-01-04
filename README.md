# iperf3 With UDP GSO/GRO support
================================================================
## Build
clone repository, compile and install
```
git clone https://github.com/jack2007/iperf.git
cd iperf
./configure
make
make install
```

## Usage
add --gsro options to server and client

Server  
```
iperf3 -s --gsro
```
Client
```
iperf3 -c <server_ip> -u -b <udp rate> --gsro
```
