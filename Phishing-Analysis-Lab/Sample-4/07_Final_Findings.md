# Sample 4 Analysis

## Executive Summary

A suspicious domain impersonating Google Drive was identified through phishing intelligence sources and investigated using URLScan, VirusTotal, and AbuseIPDB. Multiple threat intelligence vendors classified the URL and domain as phishing. The domain was newly registered and demonstrated phishing-related behavior, indicating active phishing infrastructure.

---

## Indicators of Compromise (IOCs)

### URL

hxxps://gdrive-document.com/

### Domain

gdrive-document.com

### IP Address

45.74.61.11

---

## URLScan Findings

Submitted URL:

hxxps://gdrive-document.com/

Observed Redirect:

gdrive-document.com ? index.php ? www.google.com/404

Primary IP:

45.74.61.11

ASN:

AS205397

Hosting Provider:

69HOST LLC

URLScan Verdict:

No Classification

Page Title:

Error 404 (Not Found)

### Observation

The domain redirected users to a Google 404 page through an intermediate redirect. Such behavior is commonly observed when phishing infrastructure is disabled, removed, or attempting to avoid detection.

---

## VirusTotal URL Findings

Detection Ratio:

9/92

Flagged By:

- BitDefender (Phishing)
- G-Data (Phishing)
- Kaspersky (Phishing)
- PhishTank (Phishing)
- VIPRE (Phishing)
- ESET (Phishing)
- Google Safe Browsing (Phishing)
- LevelBlue (Phishing)
- Sophos (Phishing)

Additional Classification:

- Fortinet (Spam)

### Observation

Multiple reputable security vendors classified the URL as phishing.

---

## VirusTotal Domain Findings

Domain:

gdrive-document.com

Detection Ratio:

13/91

Flagged By:

- alphaMountain.ai (Phishing)
- ESET (Phishing)
- Google Safe Browsing (Phishing)
- Kaspersky (Phishing)
- PhishTank (Phishing)
- Sophos (Phishing)
- BitDefender (Phishing)
- G-Data (Phishing)
- Gridinsoft (Phishing)
- Lionic (Phishing)
- SOCRadar (Phishing)
- VIPRE (Phishing)
- Webroot (Malicious)

Registrar:

OVH sas

Domain Age:

22 Hours

### Observation

The domain was newly registered and heavily flagged by security vendors as phishing.

---

## VirusTotal IP Findings

IP Address:

45.74.61.11

Detection Ratio:

2/91

Flagged By:

- alphaMountain.ai (Phishing)
- ESET (Phishing)

Additional Classification:

- AlphaSOC (Suspicious)

### Observation

The hosting IP received phishing-related detections from multiple vendors.

---

## AbuseIPDB Findings

IP Address:

45.74.61.11

ISP:

MICFO-CA

ASN:

AS205397

Usage Type:

Data Center / Web Hosting / Transit

Country:

Germany

City:

Frankfurt am Main

Reports:

8

Confidence of Abuse:

0%

### Observation

Although the confidence score is low, the IP has historical abuse reports and is hosted within a data center environment commonly used for internet-facing infrastructure.

---

## Analysis

Several indicators strongly suggest phishing activity.

Key Indicators:

- Domain impersonates Google Drive branding.
- Newly registered domain (22 hours old).
- URL flagged by multiple security vendors.
- Domain flagged by 13 security vendors.
- Google Safe Browsing and PhishTank detections present.
- Redirect behavior observed.
- Hosting infrastructure associated with phishing detections.

---

## MITRE ATT&CK

T1566.002 – Phishing: Spearphishing Link

---

## Verdict

Confirmed Phishing Domain

Confidence Level: High

Recommendation:

Block the URL, domain, and associated IP address. Monitor security controls for additional activity related to the identified indicators.
