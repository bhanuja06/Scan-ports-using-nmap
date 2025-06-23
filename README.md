#  Nmap Reconnaissance Scan Report

##  Overview

This project demonstrates a basic network reconnaissance scan using [Nmap](https://nmap.org/), with results exported to an HTML file (scan.html). The scan targets a local IP address (192.168.29.211) to identify open ports, services, and potential vulnerabilities.

---

##  Objectives

- Perform a TCP SYN scan (-sS)
- Detect running services and their versions (-sV)
- Attempt OS detection (-O)
- Export results to a readable .html format

---

##  Tools Used

- *Nmap* : Network mapping and port scanning
- *Command Used*:
  ```bash
  nmap -sS -sV -O -oX scan.xml 192.168.29.211
  xsltproc scan.xml -o scan.html
