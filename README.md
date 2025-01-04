# iperf3 With UDP GSO/GRO support
================================================================
## Build
1. clone repository
   git clone https://github.com/jack2007/iperf.git
2. compile and install
   cd iperf
   ./configure
   make
   make install
   

## Usage
add --gsro options to server and client

Server  
iperf3 -s --gsro

Client
iperf3 -c <server_ip> -u -b <udp rate> --gsro
