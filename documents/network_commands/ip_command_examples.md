Here are the `ip` command examples from the provided article:

*   `ip help`
*   `ip link show`
*   `ip link ls up`
*   `ip link show dev [device]`
*   `ip link show dev enp0s3`
*   `ip -s link`
*   `ip -s link ls [interface]`
*   `ip -s link ls enp0s3`
*   `ip -s -s link ls enp0s3`
*   `sudo ip link set enp0s3 down`
*   `ip link show`
*   `ip link set enp0s3 up`
*   `sudo ip link set txqueuelen [number] dev [interface]`
*   `sudo ip link set txqueuelen 10000 dev enp0s3`
*   `ip link show dev enp0s3`
*   `sudo ip link set mtu [number] dev [interface]`
*   `sudo ip link set mtu 10000 dev enp0s3`
*   `ip link show dev enp0s3`
*   `ip link set dev [interface] down`
*   `ip link set dev [interface] address [mac_address]`
*   `ip link set dev [interface] up`
*   `ip addr`
*   `ip addr show`
*   `ip addr show dev enp0s3`
*   `ip -4 addr`
*   `ip -6 addr`
*   `sudo ip addr add [ip_address] dev [interface]`
*   `sudo ip addr add 10.0.2.12 dev enp0s3`
*   `ip a`
*   `sudo ip addr add brd [ip_address] dev [interface]`
*   `ip addr del [ip_address] dev [interface]`
*   `ip addr del 10.0.2.12/32 dev enp0s3`
*   `ip route`
*   `ip route list`
*   `ip route list [selector]`
*   `ip route list table local`
*   `ip route list [ip_address]`
*   `ip route add [ip_address] dev [interface]`
*   `ip route add [ip_address] via [gateway_IP] dev [interface]`
*   `sudo ip route add 192.168.0.0/24 via 192.168.0.254 dev enp0s3`
*   `sudo ip route add default 192.168.0.0/24 via 192.168.0.254 dev enp0s3`
*   `ip route del [ip_address]`
*   `ip route del default`
*   `ip neigh show`
*   `ip neigh add [ip_address] dev [interface]`
*   `ip neigh del [ip_address] dev [interface]`
*   `ip -c link`