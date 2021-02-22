---
layout: portfolio_detail_text
order: 15
title:  Pcap Parser
name: pcap-parser
badge-description: An application for extracting data from pcap files.
filter: filter-os
badge-image: badge.png
category: Operating Systems
client: Karafarin Bank
project-date: Fall 2017
project-url:
github-repository: abradat/pcap-parsing
full-description: An application for extracting data from pcap files.
---
#### Introduction
This application is used for extracting information from captured packets in network and analyzing them. It accepts .pcap files as input, extracts them and produces results in **csv**, **byte**, **unhex**, **ip** formats. Information is extracted from pcap files using **Wireshark** and its inline tool, **TShark**.

Also, it has feature for listening on specific port and saving them as pcap files and sending the pcap files through **websockeet** to another host.
#### Technologies/Languages Used

{: .table .table-striped}
| Technology | Usage |
|------------------|--------|
| <img src="{{'assets/img/portfolio/technologies/python.png' | relative_url}}" width="60" height="60"> | **Python** language is used for developing this application. |
| <img src="{{'assets/img/portfolio/technologies/wireshark.png' | relative_url}}" width="60" height="60"> | **Wireshark** and its inline tool, **Tshark** are used for extracting data from pcap files |
| <img src="{{'assets/img/portfolio/technologies/websocket.png' | relative_url}}" width="60" height="60"> | incoming packet are sent to another host through **WebSocket** |