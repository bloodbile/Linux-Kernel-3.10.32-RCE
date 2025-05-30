# 🎀 Linux Kernel v3.10.32 RCE 🎀
## Overview
Versions 3.10.32 and below of the Linux Kernel have been found to be vulnerable to Remote Code Execution (RCE) via a stack-based buffer overflow vulnerability in the telnetd service.
## Details
By modifying the /etc/issue.net file, attackers are able to upload arbitrary telnet banners, allowing for a stack-based buffer overflow that can be exploited to execute arbitrary code with elevated privileges. The vulnerability arises from improper handling of banner content during the telnet daemon's initialization process, which can be manipulated to overwrite critical memory regions.
## Impact
Exploiting this vulnerability enables an attacker to gain remote shell access, leading to full system compromise.
