README
====

A tunnel uses utp2raw, kcptun and shadowsocks.

`user <-> shadowsocks client <-> kcptun client <-> udp2raw client <-> udp2raw server <-> kcptun server <-> ss server <-> target`

# How to use it

Clone this repository to your server or local environment.

## Server

Provision the server using `./provision -s pwd up kp sp` inside the server folder.

Please check `./provision -h` for more information.

## Client 

Install the clients using `./client -i pwd ip up sp` inside the client folder.

Start the clients using `./client -s`. You will need to config your local network to use the socks5 proxy provided by shadowsocks.

Please check `./client -h` for more information.

The port for http proxy is 8123; the port for socks5 proxy is 8083. 

Note: only mac is supported in this script for now.

