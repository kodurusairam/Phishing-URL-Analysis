# Sample 5 Analysis

## Executive Summary

A suspicious login-themed URL was identified through a phishing intelligence feed and investigated using URLScan, VirusTotal, and AbuseIPDB. Multiple security vendors classified the URL and domain as phishing. The site displayed a phishing warning page during analysis, indicating active phishing infrastructure.

---

## Indicators of Compromise (IOCs)

### URL

hxxps://login.banbenq.com/?Rf9JIC8l4DOPffX1tPDjDyy

### Domain

login.banbenq.com

### IP Address

188.114.97.3

---

## URLScan Findings

Primary Domain:

login.banbenq.com

Primary IP:

188.114.97.3

Hosting Provider:

Cloudflare, Inc.

ASN:

AS13335

URLScan Verdict:

Potentially Malicious

Page Title:

Suspected Phishing | Cloudflare

Targeted Brand:

Generic Cloudflare

Domain Age:

21 Hours

### Observation

URLScan identified the website as potentially malicious and displayed a phishing warning page. The domain was recently created and protected by Cloudflare infrastructure.

---

## VirusTotal URL Findings

Detection Ratio:

13/92

Flagged By:

- alphaMountain.ai (Phishing)
- ESET (Phishing)
- Fortinet (Phishing)
- Google Safe Browsing (Phishing)
- Lionic (Phishing)
- BitDefender (Phishing)
- Forcepoint ThreatSeeker (Phishing)
- G-Data (Phishing)
- LevelBlue (Phishing)
- PhishTank (Phishing)
- Sophos (Phishing)
- SOCRadar (Malware)
- Webroot (Malicious)

Additional Classification:

- Gridinsoft (Suspicious)

### Observation

The URL received significant phishing detections from multiple reputable security vendors.

---

## VirusTotal Domain Findings

Domain:

login.banbenq.com

Detection Ratio:

8/91

Flagged By:

- alphaMountain.ai (Phishing)
- ESET (Phishing)
- Google Safe Browsing (Phishing)
- PhishTank (Phishing)
- G-Data (Phishing)
- LevelBlue (Phishing)
- CRDF (Malicious)
- SOCRadar (Malware)

Additional Classification:

- Gridinsoft (Suspicious)

### Observation

The domain received multiple phishing and malware classifications from security vendors.

---

## VirusTotal IP Findings

IP Address:

188.114.97.3

Detection Ratio:

4/91

Flagged By:

- ADMINUSLabs (Malicious)
- Webroot (Malicious)
- Chong Lua Dao (Malicious)
- Xcitium Verdict Cloud (Malicious)

Additional Classification:

- alphaMountain.ai (Suspicious)

### Observation

The IP address received malicious classifications despite being part of Cloudflare infrastructure.

---

## AbuseIPDB Findings

IP Address:

188.114.97.3

ISP:

Cloudflare, Inc.

ASN:

AS13335

Usage Type:

Content Delivery Network (CDN)

Country:

United States

City:

San Francisco, California

Reports:

1,256

Confidence of Abuse:

0%

### Observation

The IP belongs to Cloudflare CDN infrastructure. Although heavily reported, shared CDN infrastructure can host both legitimate and malicious content.

---

## Analysis

Multiple indicators strongly suggest phishing activity.

Key Indicators:

- Login-themed URL commonly associated with credential harvesting.
- Domain age less than 24 hours.
- URLScan classified the site as potentially malicious.
- Phishing warning page observed.
- URL flagged by 13 security vendors.
- Domain flagged by 8 security vendors.
- IP flagged by 4 security vendors.
- Google Safe Browsing and PhishTank detections present.
- Cloudflare infrastructure used to obscure backend hosting.

---

## MITRE ATT&CK

T1566.002 – Phishing: Spearphishing Link

---

## Verdict

Confirmed Phishing Infrastructure

Confidence Level: High

Recommendation:

Block the URL and domain. Monitor security controls for related indicators and investigate any user interaction with the identified phishing infrastructure.
