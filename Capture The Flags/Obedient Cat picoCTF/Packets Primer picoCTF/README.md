# PicoCTF Write-up: Obedient Cat

Platform: [PicoCTF](https://play.picoctf.org/)

## Description

Download the packet capture file and use packet analysis software to find the flag.

[Download packet capture](https://artifacts.picoctf.net/c/195/network-dump.flag.pcap)

## Solution

First, download the provided .pcap file.
To understand what kind of traffic we are dealing with, open the file in Wireshark.

Among all the 9 different TCP and ARP packets, packet # 4 stands out. Rest of them are part of standard TCP communication.

Click on packet 4 to view more details about it.
And the flag is present in hex-encoded format!

To view it in readable text format, right click on packet 4, click Follow -> TCP Stream.