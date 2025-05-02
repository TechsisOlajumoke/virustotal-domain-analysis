# virustotal-domain-analysis

## Overview
This repository presents a domain threat intelligence analysis using VirusTotal. We examined the reputations and behaviors of three domains—**17ebook.com**, **aladel.net**, and **clicnews.com**—to assess their connection to malicious activity such as phishing, malware delivery, and site compromise.

## Objectives
- Determine whether the domains are associated with phishing or malware.
- Identify any Indicators of Compromise (IoCs).
- Provide actionable recommendations for improving cybersecurity posture.

## Tool Used
- **VirusTotal**: A cloud-based threat intelligence platform that aggregates results from 70+ antivirus engines and URL scanners.

## Methodology
1. Input domain names into VirusTotal's search interface.
2. Analyzed scan results from multiple security vendors.
3. Reviewed IPs, redirection behavior, subdomains, and metadata.
4. Assessed behavioral indicators for risk classification.

## Summary of Findings

### 🔴 17ebook.com
- **Flagged by**: 12/96 engines
- **IoCs**: IP `208.91.196.152`, SHA-256 hash `d7357e4a...`
- **Threats**: Phishing, malware distribution
- **Risk Level**: **High**

### 🟠 aladel.net
- **Flagged by**: 9/96 engines
- **IoCs**: IP `185.107.56.59`, 18 subdomains
- **Threats**: Malware hosting, phishing, compromised infrastructure
- **Risk Level**: **Medium to High**

### 🟡 clicnews.com
- **Flagged by**: 1/96 engines
- **IoCs**: IP `13.248.169.48`
- **Threats**: Possibly compromised in the past
- **Risk Level**: **Low to Moderate** (requires continued monitoring)

## Behavioral Risk Assessment
| Domain        | Behavior Summary                             | Risk Level       |
|---------------|----------------------------------------------|------------------|
| 17ebook.com   | Redirects, malware delivery, phishing        | 🔴 High          |
| aladel.net    | Active file comms, site compromise signs      | 🟠 Medium-High   |
| clicnews.com  | Historical compromise suspicion               | 🟡 Low-Moderate  |

## Recommendations

### 🔒 Immediate Actions
- Block all three domains across enterprise systems and security gateways.

### 🔁 Long-Term Mitigation
- Train users on phishing and social engineering threats.
- Monitor related IPs, hashes, and domains.
- Conduct periodic domain reputation checks.

## Conclusion
This investigation revealed substantial evidence that 17ebook.com and aladel.net are active threats, while clicnews.com requires observation. Proactive mitigation steps are crucial to maintaining network security and avoiding potential compromise.

---

**License**: MIT  
**Author**: [Akinmola Blessing Olajumoke]  
**Tool**: [VirusTotal](https://www.virustotal.com/)

