# Networkwalks-B084-wk2-footprinting-scanning.
footprinting and scanning with kali tools

Penetration testing report for Week 2 of the Networkwalks Cybersecurity & Ethical Hacking program. It covers passive reconnaissance with Kali Linux tools and host discovery with Zenmap.

**Report:** [Download the report (Word)](sakinah%20Penetration%20Testing%20Report%20wk-2.docx)

## Details

| Pentester | sakinah Abubakar |
| Batch | B084 |
| Testing dates | 8 November 2026 (footprinting), 11 November 2026 (network scanning) |
| Modules | W2-PM1 (multiple Kali tools), W2-PM5 (Zenmap) |
| Targets | networkwalks.com (lab target), microsoft.com (lab-specified, passive only), my own local network |

## What was done

- **Footprinting:** WHOIS, WhatWeb, nslookup, curl, wafw00f, DNSRecon and theHarvester
- **Scanning:** Zenmap Ping scan and topology of my own network, after finding the subnet with ipconfig

## Main findings

- WordPress and plugin versions were publicly visible on networkwalks.com (Medium)
- The SPF record uses softfail (`~all`), so spoofed email is more likely to be delivered (Medium)
- Missing security headers, DNSSEC not enabled and a disclosed BIND version were rated Low
- My own network showed only two hosts: my PC and the gateway
- theHarvester found many public subdomains for microsoft.com (Low)

No vulnerability was confirmed. The findings are observations from information gathering only, and no exploitation was performed.

## Disclaimer
Author
sakinah Abubakar, cybersecurity trainee
LinkedIn:https://www.linkedin.com/in/sakinah-abubakar-1183aa219

All activities were performed only on systems where I had permission or that I own. This material is for education and research purposes only.
