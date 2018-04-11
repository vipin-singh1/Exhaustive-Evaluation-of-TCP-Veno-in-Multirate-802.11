# Exhaustive-Evaluation-of-TCP-Veno-in-Multirate-802.11

TCP Veno combines the advantages of TCP Reno and TCP Vegas to improve TCP performance in wireless networks. This project aims to evaluate the performance of TCP Veno in the presence of Rate Adaptation Algorithms such as ARF, AARF, AARF-CD, ONOE and Minstrel.

Let N be the backlog at the queue i.e  the packets accumulated at the bottleneck link. TCP vegas uses this N to proactively adjust the cwnd to avoid packet loss due to buffer overlow. But TCP Veno uses same N value to know the packet loss is random packet loss or due to congestion by measuring N.

### How to simulate topology with tcp veno enabled:

Clone the repository to home directory<br />
`git clone https://github.com/vipin-singh1/Exhaustive-Evaluation-of-TCP-Veno-in-Multirate-802.11.git`<br />
Change directory to:<br />
`cd NS3repo/ns-3-allinone/ns-3-dev/`<br />
Compile and run the source code:<br />
`./waf`   
`./waf --run="scratch/test_ap --wifiManager=Arf/Aarf/Onoe --tcpVariant=TcpVeno --pcap" --vis` 
### References<br />
For more information refer https://ieeexplore.ieee.org/document/1177186/
