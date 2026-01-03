\# SQLMap – Automated SQL Injection Testing



\## Overview

SQLMap is an open-source automated tool used to detect and exploit SQL injection (SQLi) vulnerabilities in web applications. It automates payload generation, injection techniques, and database enumeration while allowing controlled and authorized testing.



This documentation is based on hands-on learning and focuses on understanding SQLMap from both an offensive testing and defensive (SOC) perspective.



---



\## SQL Injection Summary

SQL Injection occurs when an application constructs SQL queries using unsanitized user input, allowing an attacker to manipulate database queries.



Potential impact includes:

\- Unauthorized data access

\- Authentication bypass

\- Data modification or deletion

\- Full database compromise



---



\## What SQLMap Automates

SQLMap automates:

\- Detection of injectable parameters

\- Identification of database management systems (DBMS)

\- SQL injection technique selection

\- Enumeration of databases, tables, and columns

\- Data extraction when authorized



Supported techniques:

\- Boolean-based blind

\- Time-based blind

\- Error-based

\- UNION-based



SQLMap does not replace understanding. Proper scope, interpretation, and authorization are essential.



---



\## High-Level Workflow

1\. Identify a target input (URL parameter or request)

2\. SQLMap sends controlled payloads

3\. Server responses are analyzed

4\. SQL injection technique is confirmed

5\. Enumeration or extraction is performed if permitted



---



\## Core Commands
-u
-r
--dbs
--tables
--columns
--dump
--batch



\### Test a Target URL

```bash

sqlmap -u "http://target.site/page.php?id=1"



