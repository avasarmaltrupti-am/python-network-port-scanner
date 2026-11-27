# Python Network Port Scanner & Security Assessment

## About the Project
This project demonstrates a beginner-friendly TCP port scanner developed using Python socket programming. It scans selected ports on the local machine, stores results in a CSV file, and verifies the findings using Nmap.

## Objectives
- Develop a TCP port scanner using Python.
- Identify whether selected TCP ports are open or not open.
- Export scan results into a CSV file.
- Verify results using Nmap.
- Perform basic service identification and security assessment.

## Tools & Technologies
- Python 3
- Kali Linux
- Nmap
- Python Socket Module
- CSV Module
- TCP/IP

## Project Scope
- Target: `127.0.0.1` (localhost)
- Ports scanned: `21, 22, 80, 443, 8000, 8080`
- Testing environment: Local machine only.

## Results

| Port | Result |
|---|---|
| 21 | Not open |
| 22 | Not open |
| 80 | Not open |
| 443 | Not open |
| 8000 | Open |
| 8080 | Not open |

Nmap service detection identified port `8000/tcp` as:

`SimpleHTTPServer 0.6 (Python 3.14.7)`

Python scanner results and Nmap results agreed that port 8000 was open.

## Project Files
- `scanner.py` – Python port scanner source code.
- `scan_results.csv` – Saved scan results.
- `nmap_basic.txt` – Nmap port scanning output.
- `nmap_service.txt` – Nmap service detection output.
- `security_assessment.txt` – Security observations and recommendations.
- `screenshots/` – Project execution screenshots.
- `presentation/` – Project presentation.

## Security Recommendations
- Stop the development HTTP server after testing.
- Bind development services to `127.0.0.1` when external access is unnecessary.
- Avoid storing confidential files in the server directory.
- Repeat scans after configuration changes.
- Scan only systems you own or have explicit permission to test.

## Learning Outcomes
- Understanding TCP port scanning.
- Using Python socket programming.
- Generating CSV reports.
- Performing Nmap verification.
- Understanding basic service identification and security assessment.

## Disclaimer
This project was developed for educational purposes and tested only on localhost (`127.0.0.1`). Do not scan systems without proper authorization.
