# Network-Namespace-commands
1. adding namespace -> ip netns add <hostname>
2. deleting namespace -> ip netns del <hostname>
3. ip route
4. ip address/ ip addr / ip a
5. ip link add eth0 type veth peer name eth1
6. Check namespaces -> ip netns
7. execute in a namespace -> sudo ip netns exec <namespace-name> bash
8. ip netns exec red ip route add default via 10.0.0.2 dev eth0 -> we route every packet from eth0 to ip address 10.0.0.2
9. ip netns exec router sysctl -w net.ipv4.ip_forward=1 -> we make the namespace router to act as a router and using net.ipv4.ip_forward=1 by setting ip_forward to 1 this internally connects eth2 to eth3 (screenshot is there in the system.
