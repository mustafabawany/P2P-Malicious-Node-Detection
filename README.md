# P2P-Malicious-Node-Detection

## Abstract

Current peer-to-peer (P2P) streaming systems often assume that nodes cooperate to upload
and download data. However, in the open environment of the Internet, this is not necessarily
true and there exist malicious nodes in the system. This project studies malicious actions of
nodes that can be detected through peer-based monitoring. We require each node to monitor
the data received and to periodically send monitoring messages about its neighbors to some
trustworthy nodes. To efficiently store and search messages among multiple trustworthy nodes,
we organize trustworthy nodes into a threaded binary tree. Trustworthy nodes also dynamically
redistribute monitoring messages among themselves to achieve load balancing. Our simulation
results show that this scheme can efficiently detect malicious nodes with high accuracy and that
the dynamic redistribution method can achieve good load balancing among trustworthy nodes.

## Introduction

To understand the problem, it is necessary to understand the concept behind forming a P2P
network. A peer-to-peer (P2P) network is created when two or more PCs are connected and
share resources without going through a separate server computer. In a P2P environment,
access rights are governed by setting sharing permissions on individual machines. A
peer-to-peer network is designed around the notion of equal peer nodes simultaneously
functioning as both "clients" and "servers" to the other nodes on the network. This model of
network arrangement differs from the client-server model where communication is usually to
and from a central server. A typical file transfer that uses the client-server model is the File
Transfer Protocol (FTP) service. The client and server programs are distinct: the clients initiate
the transfer, and the servers satisfy these requests.BitTorrent is one of the powerful examples of
Peer to Peer network.
<br><br>
Since this network architecture is so helpful, there are some problems associated with it that we
are trying to solve to get the better out of P2P. Some common issues with P2P networks are that
Content shared via P2P applications is sometimes infected with malware, sometimes contains
legally protected copyrighted material, or may sometimes contain personal data accidentally
shared. We are trying to encounter the problem of Malicious nodes on the server-side with the
use of TCP connections and socket programming and in our methodology, if a malicious node is
encountered, It will forcefully kick the malicious node out of the network for security reasons.

## How to execute
NOTE: You must have pip and python pre-installed in your system

1. Clone this project on your local repository
```
git clone <repository link>
```
2. Open a new Terminal and Execute
```
python3 Tracker.py
```
3. Open another Terminal and Execute 
```
python3 Peer.py 6000 
```
## Technology Used

<div>
  <img name = "Python" src = "https://img.shields.io/badge/python%20-%2314354C.svg?&style=for-the-badge&logo=python&logoColor=white">
  <img name = "Socket" src = "https://img.shields.io/badge/Socket.io-black?style=for-the-badge&logo=socket.io&badgeColor=010101">
</div>
