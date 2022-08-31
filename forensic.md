# Forensic

## hex editor (online)
https://hexed.it/

## Disk forensic
### Tools
- `Autopsy` (https://www.autopsy.com/)


## Memory forensic
### Tools
- `volatility` (https://github.com/volatilityfoundation/volatility)
### important command
```bash
./vol.py -f file.dmp windows.vadyarascan.VadYaraScan --yara-rules "CTF{"
./vol.py -f file.dmp yarascan.YaraScan --yara-rules "CTF{"
```
**for more information read** https://github.com/carlospolop/hacktricks/blob/master/forensics/basic-forensic-methodology/memory-dump-analysis/volatility-examples.md

## Network forensic : Packet analysis
### Tools
- `Wireshark` (https://www.wireshark.org/download.html)
- `Scapy` Packet crafting for Python (https://scapy.net/)



## Malware Forensic
### MS Office documents analyzer
#### Tools
- `oletools` (https://github.com/decalage2/oletools)



## Tips & Tricks


### Wireshark
#### - `TLS`
- `secrets.log` file can view the `TLS` content in plain text by config under `Edit` -> `Preferences` -> `Protocols` -> `TLS` in `(Pre)-Master-Secret log filename` field.

#### - `USB` : if you have a pcap containing the communication via USB of a keyboard like the following one:
![usb](https://1517081779-files.gitbook.io/~/files/v0/b/gitbook-legacy-files/o/assets%2F-L_2uGJGU7AVNRcqRvEi%2F-MiqBTLrqhx3Eh36PwsU%2F-MiqBoJOETIsG923ubGY%2Fimage.png?alt=media&token=da64a1dd-e84b-411c-b5c1-237d3d4908a2)
<br>
You can use the tool `ctf-usb-keyboard-parser` to get what was written in the communication:

You can read more information and find some scripts about how to analyse this in:
- https://medium.com/@ali.bawazeeer/kaizen-ctf-2018-reverse-engineer-usb-keystrok-from-pcap-file-2412351679f4
- https://github.com/tanc7/HacktheBox_Deadly_Arthropod_Writeup
