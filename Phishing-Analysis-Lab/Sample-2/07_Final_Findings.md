# Sample 2 Analysis

## Executive Summary

A suspicious URL hosted on Microsoft Azure Static Website infrastructure was identified through OpenPhish and investigated using URLScan, VirusTotal, and AbuseIPDB. Multiple threat intelligence sources classified the URL as phishing-related infrastructure.

---

## Indicators of Compromise (IOCs)

### URL

hxxps://nexoexterior.z13.web.core.windows.net/empr...

### Domain

nexoexterior.z13.web.core.windows.net

### IP Address

52.239.169.97

---

## URLScan Findings

IP Address: 52.239.169.97

Hosting Provider: Microsoft Corporation

ASN: 8075

Location: Washington, United States

HTTPS: Enabled

Google Safe Browsing: Malicious

Page Title: WebContentNotFound

Redirects Observed: 0

### Observation

The URL was hosted on Microsoft Azure Static Website infrastructure. The phishing content appears to have been removed or disabled prior to investigation.

---

## VirusTotal URL Findings

Detection Ratio: 4/92

Flagged By:

- Emsisoft (Phishing)
- ESET (Phishing)
- Yandex Safebrowsing (Phishing)
- Netcraft (Malicious)

Status: 404

Content Type: text/html

### Observation

Multiple security vendors classified the URL as phishing or malicious, increasing confidence in the malicious assessment.

---

## VirusTotal Domain Findings

Detection Ratio: 1/91

Flagged By:

- Yandex Safebrowsing (Phishing)

### Observation

The domain itself has limited reputation detections; however, the URL path shows stronger phishing indicators than the base domain.

---

## VirusTotal IP Findings

IP Address: 52.239.169.97

Detection Ratio: 1/91

Flagged By:

- alphaMountain.ai (Phishing)

ASN: 8075

Organization: Microsoft Corporation

### Observation

The IP belongs to Microsoft Azure cloud infrastructure and has limited reputation detections.

---

## AbuseIPDB Findings

IP Address: 52.239.169.97

ISP: Microsoft Corporation

ASN: AS8075

Usage Type: Data Center / Web Hosting / Transit

Country: United States

City: Washington, Virginia

Reports: 3

Confidence of Abuse: 2%

### Observation

The IP has a small number of abuse reports and low confidence of abuse. This is common for cloud-hosted phishing infrastructure due to rapid resource rotation by threat actors.

---

## Analysis

Evidence collected from OpenPhish, URLScan, VirusTotal, and AbuseIPDB indicates the URL was likely used as phishing infrastructure hosted on Microsoft Azure.

Key Indicators:

- OpenPhish reported the URL as phishing.
- Google Safe Browsing classified the site as malicious.
- Multiple VirusTotal vendors classified the URL as phishing or malicious.
- URL hosted on Azure Static Website infrastructure.
- Randomized subdomain naming convention.
- Content appears removed before analysis.
- Cloud-hosted infrastructure commonly abused for credential harvesting campaigns.

---

## MITRE ATT&CK

T1566.002 – Phishing: Spearphishing Link

---

## Verdict

Likely Phishing Infrastructure

Confidence Level: High
