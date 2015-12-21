# py-multicast-example
simple python multicast sender/receiver example

this example is based on demo python program http://svn.python.org/projects/python/trunk/Demo/sockets/mcast.py. the enhancement is to support interface as argument.

note that at CentOS/redhat system, you need run "iptables -I INPUT -p udp -i enp0s8 -m state --state NEW -m multiport --dports 8123 -j ACCEPT" to enable iptable rules at receiver machine
