# PicoCTF Write-up: Packets Primer

Platform: [PicoCTF](https://play.picoctf.org/)

## Description

Download the packet capture file and use packet analysis software to find the flag.

[Download packet capture](https://artifacts.picoctf.net/c/195/network-dump.flag.pcap)

<img width="605" height="206" alt="image" src="https://github.com/user-attachments/assets/ba5a5a06-ca38-4c82-8bf3-b8a94fdfd0f9" />


## Solution

First, download the provided .pcap file.
To understand what kind of traffic we are dealing with, open the file in Wireshark.

<img width="1919" height="427" alt="image" src="https://github.com/user-attachments/assets/8ecfceb3-405c-40a6-8982-65a3b1f2eb77" />

Among all the 9 different TCP and ARP packets, packet # 4 stands out. Rest of them are part of standard TCP communication.

Click on packet 4 to view more details about it.
And the flag is present in hex-encoded format!

<img width="920" height="469" alt="image" src="https://github.com/user-attachments/assets/571b0f88-0845-466c-9087-0e57ad796d4f" />

To view it in readable text format, right click on packet 4, click Follow -> TCP Stream.

