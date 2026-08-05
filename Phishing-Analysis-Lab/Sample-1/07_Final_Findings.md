# Sample 1 Analysis

## Executive Summary

A suspicious URL hosted on Microsoft Azure Static Website infrastructure was identified through OpenPhish and investigated using URLScan, VirusTotal, and AbuseIPDB. Multiple reputation sources classified the URL/domain as phishing-related.

---

## Indicators of Compromise (IOCs)

### URL

hxxps://extesrionexo.z13.web.core.windows.net/

### Domain

extesrionexo.z13.web.core.windows.net

### IP Address

57.150.87.132

---

## URLScan Findings

- IP Address: 57.150.87.132
- Hosting Provider: Microsoft Corporation
- ASN: 8075
- Location: Washington, United States
- HTTPS Enabled
- Google Safe Browsing: Malicious
- Page Title: WebContentNotFound
- No redirects observed

### Observation

The phishing content appears to have been removed or taken down before analysis.

---

## VirusTotal URL Findings

Detection Ratio:
1/92

Flagged By:
- Yandex Safebrowsing (Phishing)

---

## VirusTotal Domain Findings

Detection Ratio:
3/91

Flagged By:
- Emsisoft (Phishing)
- Yandex Safebrowsing (Phishing)
- Netcraft (Malicious)

### Observation

The domain reputation is more suspicious than the individual URL reputation.

---

## VirusTotal IP Findings

Detection Ratio:
1/91

Flagged By:
- alphaMountain.ai (Phishing)

### Observation

The IP belongs to Microsoft Azure infrastructure and has limited reputation detections.

---

## AbuseIPDB Findings

Reports:
2

Confidence of Abuse:
0%

ISP:
Microsoft Limited

Usage Type:
Data Center / Web Hosting

### Observation

The IP has minimal abuse history despite being associated with suspicious infrastructure.

---

## Analysis

Evidence collected from OpenPhish, URLScan, VirusTotal, and AbuseIPDB indicates the URL was likely part of phishing infrastructure hosted on Microsoft Azure.

Key indicators:

- OpenPhish reported the URL.
- Google Safe Browsing classified the site as malicious.
- Multiple VirusTotal vendors classified the domain as phishing or malicious.
- Randomized subdomain naming pattern.
- Hosted on cloud infrastructure frequently abused by threat actors.
- Phishing content appears to have been removed before investigation.

---

## MITRE ATT&CK

T1566.002 – Phishing: Spearphishing Link

---

## Verdict

Likely Phishing Infrastructure

Confidence Level: Medium to High
