# Phishing Incident Analysis - Ephemeral Infrastructure (IoC: finances.portal-update.xyz)

## Project Overview
This repository contains the full analysis and incident response documentation for a simulated critical phishing alert. The project demonstrates core Security Operations Center (SOC) Tier 1 and Tier 2 capabilities in handling a rapidly deployed, evasive threat.

## Incident Context
* **Trigger:** User-reported phishing attempt via an email directing them to a fake financial "update portal."
* **Indicator of Compromise (IoC):** `https://finances.portal-update.xyz/login`
* **Goal:** Determine the threat level, confirm the attack vector, and provide immediate containment/long-term mitigation strategies.

## Key Findings
The analysis confirmed the IoC was part of an **Ephemeral Phishing Infrastructure**:
* **Evasion:** Zero detection score on most VirusTotal engines, bypassing initial automated blacklists.
* **Inactivity:** Immediate failure of behavioral analysis (HTTP 400 / DNS Error), indicating the domain was taken down or never fully deployed to evade detection tools.
* **Intent:** The domain's structure (`portal-update.xyz`) is a clear example of **Typosquatting** intended for credential harvesting.

## Skills Demonstrated
| Skill | Tools Used |
| :--- | :--- |
| **Threat Intelligence (TI)** | VirusTotal (VT), URLScan.io |
| **Open Source Intelligence (OSINT)** | WHOIS Lookup, DNS Lookup (MXToolbox) |
| **Incident Response (IR)** | Triage, Containment Planning, and Documentation (SOC T1/T2 methodology) |
| **Reporting** | Structured professional documentation and actionable recommendations. |

---

## View the Full Incident Report

The detailed report includes the step-by-step analysis, technical conclusions, and a breakdown of SOC response actions (T1, T2, and T3 recommendations).

[**Click Here to View the Full Professional Incident Report ▶️**](./ANALYSE_FINALE_PHISHING.md)
