# Project One: Cyber-Enabled Fraud Targeting Nigerian SMEs

**Analyst:** ABIGAIL AJETUNMOBI | **Date:** NovEMBER 2025 

## Executive Summary
This project investigates a systematic social engineering campaign targeting Small and Medium Enterprises (SMEs) in Nigeria. The analysis focuses on "Verification Gap" exploits, where adversaries use visual forgery (fake receipts) and psychological pressure to bypass payment validation.

Unlike traditional cyberattacks that exploit software vulnerabilities, this campaign exploits Logic Flaws in the business process.

---

## Project Artifacts (Downloads)
[Read the Full Analysis Report (PDF)](./CTI_REPORT_SME_FRAUD.pdf)
*The complete investigation, narrative analysis, TTP mapping, and defense guide.*

[View Indicators of Compromise (CSV)](./IOCs.csv)
*Redacted list of phone numbers, aliases, and transaction references used in the campaign.*

---

## Threat Analysis (MITRE ATT&CK)

### The "Kill Chain" Visualization
The attack relies on momentum. The adversary moves quickly from Deception to Pressure to force the Release of goods. Breaking the chain requires a "Verification Pause" at Step 3.

![Kill Chain Diagram](CYBER%20KILL%20CHAIN.PNG)
*Figure 1: The SME Fraud Kill Chain. Defense relies on breaking the process at the "Pressure" phase.*

### TTP Mapping Matrix
The following table maps the observed scammer behaviors to the industry-standard MITRE ATT&CK Framework.

![MITRE Matrix](MITRE%20MATRIX.PNG)
*Figure 2: TTP Analysis Matrix mapping observed procedures to standard techniques.*

---

## Key Findings & Defense
The investigation identified three primary fraud scenarios:
1.  **Physical Marketplace Theft:** Using fake Bank alerts during meetups.
2.  **Digital Vendor Harassment:** Using forged bank receipts + aggression ("Reverse Victimization").
3.  **High-Value POS Fraud:** Using "Shock Value" (e.g., N1m fake receipts) to overwhelm logic.

**Analyst Verdict:** The primary defense is "Zero Trust for Visual Evidence." No goods should be released based on a screen shown by the customer; verification must occur via backend database checks or bank app transaction history or statements.

---

## Privacy & Disclaimer
Specific Personally Identifiable Information (PII), such as full phone numbers and bank account details, has been redacted from this public report to comply with Data Privacy regulations and platform policies. Full indicators are available to verified security researchers upon request.

All data was gathered via Open Source Intelligence (OSINT) for educational and defensive purposes.
