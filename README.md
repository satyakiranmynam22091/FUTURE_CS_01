# FUTURE_CS_01 — Vulnerability Assessment Report

## Internship
Future Interns — Cyber Security

## Task
Task 1 — Vulnerability Assessment Report for a Live Website

## Target
https://altoro.testfire.net/

## Objective
To perform a passive vulnerability assessment of the target web application and document identified security weaknesses, their risk levels, evidence, impact, and remediation recommendations.

## Tools Used
- Nmap
- OWASP ZAP — Passive Scan
- Browser Developer Tools
- Kali Linux

## Methodology

### 1. Reconnaissance
Nmap was used to identify accessible HTTP/HTTPS services and obtain service information.

### 2. HTTP Header Analysis
HTTP response headers were reviewed using Nmap and browser Developer Tools.

### 3. Passive Vulnerability Assessment
OWASP ZAP was used in passive scanning mode while browsing the target application.

### 4. Risk Classification
Findings were recorded using the risk and confidence classifications reported by OWASP ZAP.

## Findings

| ID | Finding | Risk | Confidence |
|---|---|---|---|
| F-01 | Missing Anti-clickjacking Header | Medium | Medium |
| F-02 | Content Security Policy (CSP) Header Not Set | Medium | High |
| F-03 | Server Leaks Version Information via Server Header | Low | Medium |

## Nmap Results

HTTP and HTTPS services were identified on ports 80 and 443.

Detected service:

Apache Tomcat/Coyote JSP engine 1.1

## Limitations

This assessment was limited to reconnaissance, HTTP response-header analysis, browser inspection, and OWASP ZAP passive scanning.

No active scanning, exploitation, brute-force testing, or fuzzing was performed.

## Evidence

Screenshots and supporting evidence are available in the `evidence/` directory.

## Disclaimer

This assessment was performed against the intentionally vulnerable Altoro Mutual training application for cybersecurity learning and internship documentation purposes.
