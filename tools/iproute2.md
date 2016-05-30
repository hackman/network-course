iproute2 cheetsheet: http://baturin.org/docs/iproute2/

* basic stuff
 + configure interface
  ip addr add 10.0.0.1/24 dev eth0
 + configure routing
  ip route add 10.1.2.0/24 dev eth0
  ip route add 10.1.2.0/24 via 10.0.0.2
 + manage the arp tables (neighbors)
  ip neigh list
  ip neigh add/del 

* advanced stuff
 + manage rules 
 + manage multiple routing tables

* create interfaces
  ip link add NAME [options] type TYPE

 + vlan
  ip link add eth0.1 link eth0 type vlan id 1
 + tunnel (ipip/sit/gre)
 + bridge
  ip link add br0 type bridge
 + bond
 + veth/macvlan/macvtap
 + vxlan



