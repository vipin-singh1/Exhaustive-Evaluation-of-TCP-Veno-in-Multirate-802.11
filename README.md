# Exhaustive-Evaluation-of-TCP-Veno-in-Multirate-802.11

TCP Veno combines the advantages of TCP Reno and TCP Vegas to improve TCP performance in wireless networks. This project aims to evaluate the performance of TCP Veno in the presence of Rate Adaptation Algorithms such as ARF, AARF, AARF-CD, ONOE and Minstrel.

Let N be the backlog at the queue i.e  the packets accumulated at the bottleneck link TCP vegas uses this N to proactively adjust the cwnd to avoid packet loss due to buffer overlow. But TCP Veno uses same N value to know the packetloss is random packet loss or due to congestion by measuring N.<br />



<br />For more information refer https://ieeexplore.ieee.org/document/1177186/<br />



How to simulate topology with tcp veno enabled:<br />

1.Clone the repository to home direction(cmd:  git clone https://github.com/vipin-singh1/Exhaustive-Evaluation-of-TCP-Veno-in-Multirate-802.11.git NS3repo)
<br />2. cd NS3repo/ns-3-allinone/ns-3-dev/<br />
3 ./waf        /* to compile the files in scratch */<br />
4../waf --run="scratch/test_ap --wifiManager=Arf --tcpVariant=TcpVeno --pcap" --vis  /*cmd to run<br />
                                                                                     /* can change wifi manager to Aarf,Onoe<br />
                                                                                     /* pcap argument enable pcap and generate pcap<br />                                   files
