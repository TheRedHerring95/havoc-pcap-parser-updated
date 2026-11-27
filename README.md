# havoc-pcap-parser-updated
Updated version of havoc-pcap-parser for newer versions of python (tested on python3.14)

Built from Immersive Labs' havoc-pcap-parser.py as at the 27th of November 2026, found here: https://github.com/Immersive-Labs-Sec/HavocC2-Forensics/blob/main/PacketCapture/havoc-pcap-parser.py. Rewritten to use scapy instead of pyshark due to issues running pyshark on Python3.14

Rewrite assisted by Gemma4 

## Requirements
Python3
PyCryptodome
Scapy

## Differencees in functionality
Due to using Scapy instead of Pyshark, it doesn't (currently) show all traffic with the C2. It only reveals the information within the packet with the magic byte. This is due to differences in how the dependencies work, though I have thoughts for how I could add the functionality in in the future if either I need to or it's requested.

## Attribution
Credit goes to Immersive Labs Sec, and to kevthehermit for the original parser and work on Havoc C2 forensics.
Apologies if I've messed up the handling of the license; this is my first time working on licensed work, let alone publishing a modified version of it. If I have, please let me know and I will do what I can to correct the error/s.
