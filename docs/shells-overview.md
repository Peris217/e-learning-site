\# Shells Overview – Post-Exploitation Fundamentals



\## Overview

A shell is an interface that allows a user to interact with an operating system.  

In cybersecurity, shells are commonly used during post-exploitation to execute commands on a compromised system.



Understanding shells is important for both offensive and defensive security, as shells are often the mechanism attackers use to maintain access after an initial compromise.



---



\## What Is a Shell?

A shell provides a way to send commands to an operating system and receive output.



Common shell types include:

\- Command-line shells (e.g., Bash, CMD, PowerShell)

\- Remote shells obtained over a network connection



In an attack scenario, a shell allows an attacker to:

\- Execute system commands

\- Enumerate the system

\- Escalate privileges

\- Maintain persistence



---



\## Types of Shells



\### 1. Reverse Shell

A reverse shell occurs when the target system initiates a connection back to the attacker’s machine.



\*\*Why attackers use it:\*\*

\- Bypasses inbound firewall restrictions

\- Easier to receive connections behind NAT



\*\*Defensive indicators:\*\*

\- Unexpected outbound connections

\- Suspicious network traffic to external IPs

\- Abnormal process behavior



---



\### 2. Bind Shell

A bind shell opens a listening port on the compromised system, allowing the attacker to connect directly.



\*\*Why attackers use it:\*\*

\- Simple setup

\- Direct access if ports are reachable



\*\*Defensive indicators:\*\*

\- Unknown services listening on non-standard ports

\- Unrecognized processes binding to network interfaces



---



\### 3. Web Shell

A web shell is a script uploaded to a web server that allows command execution through a browser.



\*\*Common formats:\*\*

\- PHP

\- ASP / ASPX

\- JSP



\*\*Defensive indicators:\*\*

\- Unexpected files in web directories

\- Obfuscated code in web scripts

\- Suspicious HTTP requests triggering command execution



---



\## Shell Stabilization (Conceptual)

Initial shells are often unstable or limited.



Attackers may attempt to:

\- Upgrade shells to interactive TTYs

\- Improve usability for long-term access



From a defensive perspective, this activity may generate:

\- Additional process creation

\- Terminal-related commands

\- Unusual environment changes



---



\## Shells in the Attack Lifecycle

Shells typically appear after:

1\. Initial access (e.g., SQL injection, file upload, RCE)

2\. Exploitation success

3\. Post-exploitation begins



They are a \*\*strong indicator of compromise (IOC)\*\*.



---



\## Defensive Perspective (SOC Relevance)

Defenders may detect shell activity through:

\- Endpoint Detection and Response (EDR)

\- Process monitoring

\- Network traffic analysis

\- Log correlation (SIEM)



Key red flags include:

\- Shell processes spawned by web servers

\- Outbound connections from servers to unknown hosts

\- Command execution from unexpected parent processes



---



\## Key Takeaways

\- Shells enable command execution on compromised systems

\- Reverse, bind, and web shells are the most common types

\- Shell activity often indicates post-exploitation

\- Understanding shells improves detection and incident response



---



\## Ethics \& Legal Use

Shells should only be used in controlled environments or systems where explicit authorization has been granted. Unauthorized use is illegal and unethical.

