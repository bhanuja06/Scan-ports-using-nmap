#  Nmap Scan Report Summary

##  Objective

To perform a basic reconnaissance scan on the local IP address 192.168.29.211 using Nmap. The scan was aimed at identifying open ports, detecting running services, and attempting operating system fingerprinting. The results were exported to an HTML file (scan.html) for easy analysis and presentation.

---

##  Scan Methodology

- *Scan Type*: TCP SYN scan (-sS)
- *Service Version Detection*: Enabled (-sV)
- *Operating System Detection*: Enabled (-O)
- *Command Used*:
  ```bash
  nmap -sS -sV -O -oX scan.xml 192.168.29.211
  xsltproc scan.xml -o scan.html
