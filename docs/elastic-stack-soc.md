\# Elastic Stack — SOC Fundamentals



\## Overview

This document captures my hands-on learning from the \*\*Elastic Stack: The Basics\*\* lab on TryHackMe.  

The focus is on understanding how the Elastic Stack supports visibility, detection, and investigation in a Security Operations Center (SOC) environment.



Elastic Stack plays a critical role in collecting, indexing, and visualizing security and system data, enabling analysts to identify suspicious activity and respond efficiently.







\## SOC Context

In a SOC workflow, Elastic Stack typically supports the following process:



\*\*Log Collection → SIEM → Alert Generation → Investigation → Documentation / Escalation\*\*



This lab helped reinforce how visibility at the log level translates into actionable security decisions at the analyst level.







\## Core Components

\### Elasticsearch

\- Stores and indexes large volumes of structured and unstructured data

\- Enables fast searching and correlation of security events

\- Acts as the backbone for detection and investigation



\### Kibana

\- Provides dashboards and visualizations for security data

\- Used by analysts to explore alerts, logs, and trends

\- Supports investigation and reporting workflows



\### Beats

\- Lightweight data shippers that collect logs and metrics from endpoints and servers

\- Sends data into the Elastic pipeline for processing



\### Logstash

\- Processes, filters, and normalizes incoming data

\- Helps structure logs for consistent analysis and detection







\## What I Learned

\- How logs move from endpoints and systems into a centralized SIEM platform

\- How dashboards and visualizations improve situational awareness

\- How alerts are generated and reviewed by SOC analysts

\- The role of correlation and filtering in reducing noise and false positives







\## Analyst Workflow

\### Alert Triage

\- Review alert details and associated logs

\- Validate whether the activity is benign or suspicious

\- Identify affected systems, users, or IP addresses



\### Investigation

\- Pivot through logs using filters and search queries

\- Look for patterns, anomalies, and timelines of events

\- Correlate activity across multiple data sources



\### Documentation \& Escalation

\- Record findings clearly and accurately

\- Escalate confirmed threats to Tier 2 / Incident Response teams

\- Preserve context for forensic or remediation work







\## Key Security Concepts

\- Centralized logging

\- Event correlation

\- Detection engineering (basic concepts)

\- Situational awareness

\- False positive reduction







\## Tools \& Platform

\- TryHackMe

\- Elastic Stack (Elasticsearch, Kibana, Beats, Logstash)

\- Web-based SOC  labs environment.

