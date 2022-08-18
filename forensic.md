# Forensic

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
- `secrets.log` file can view the `TLS` content in plain text by config under `Edit` -> `Preferences` -> `Protocols` -> `TLS` in `(Pre)-Master-Secret log filename` field.