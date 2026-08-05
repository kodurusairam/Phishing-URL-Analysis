# Sample 3 Analysis

## Executive Summary

A phishing URL hosted behind Cloudflare infrastructure was identified through OpenPhish and investigated using URLScan, VirusTotal, and AbuseIPDB. Multiple threat intelligence vendors classified both the URL and domain as phishing-related. The domain was newly registered and displayed a phishing warning page during analysis.

---

## Indicators of Compromise (IOCs)

### URL

hxxps://vinepixo.click/3-wZa

### Domain

vinepixo.click

### IP Address

104.18.95.41

---

## URLScan Findings

Main Domain: vinepixo.click

Primary IP: 172.67.153.171

Hosting Provider: Cloudflare, Inc.

ASN: AS13335

HTTPS: Enabled

URLScan Verdict: Potentially Malicious

Targeted Brand: Generic Cloudflare

Page Title:

Suspected Phishing | Cloudflare

### Observation

The URLScan screenshot displayed a phishing warning page indicating suspected phishing activity. The domain was protected behind Cloudflare infrastructure.

---

## VirusTotal URL Findings

Detection Ratio: 2/92

Flagged By:

- LevelBlue (Phishing)
- PREBYTES (Phishing)

Status: 200 OK

Content Type: text/html

### Observation

Multiple security vendors classified the URL as phishing-related.

---

## VirusTotal Domain Findings

Domain: vinepixo.click

Detection Ratio: 5/91

Flagged By:

- Forcepoint ThreatSeeker (Phishing)
- PREBYTES (Phishing)
- Sophos (Phishing)
- G-Data (Phishing)
- SOCRadar (Phishing)

Additional Classifications:

- ESET (Suspicious)
- LevelBlue (Suspicious)

Registrar:

NameSilo, LLC

Domain Age:

Approximately 7 days

### Observation

The domain was recently registered and received multiple phishing detections from security vendors, significantly increasing confidence in malicious intent.

---

## VirusTotal IP Findings

IP Address: 104.18.95.41

ASN: AS13335

Organization: Cloudflare, Inc.

Detection Ratio: 0/91

### Observation

The IP itself was not classified as malicious. This is common because Cloudflare infrastructure is shared among many websites.

---

## AbuseIPDB Findings

IP Address: 104.18.95.41

ISP: Cloudflare, Inc.

ASN: AS13335

Usage Type: Content Delivery Network (CDN)

Country: United States

City: San Francisco, California

Reports: 37

Confidence of Abuse: 0%

### Observation

The IP belongs to Cloudflare CDN infrastructure. Abuse reports alone cannot be used as evidence because Cloudflare hosts many unrelated domains behind shared infrastructure.

---

## Analysis

Evidence collected from OpenPhish, URLScan, VirusTotal, and AbuseIPDB strongly indicates phishing activity.

Key Indicators:

- OpenPhish reported the URL.
- URLScan classified the site as potentially malicious.
- A phishing warning page was observed during analysis.
- VirusTotal URL received phishing detections.
- VirusTotal domain received multiple phishing detections.
- Domain was recently registered.
- Domain used a suspicious .click TLD.
- Cloudflare infrastructure was used to conceal backend hosting.

---

## MITRE ATT&CK

T1566.002 – Phishing: Spearphishing Link

---

## Verdict

Confirmed Phishing Infrastructure

Confidence Level: High
