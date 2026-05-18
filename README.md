# Splunk Brute-Force Detection Home Lab

## Project Overview
This project demonstrates a hands-on SOC home lab built using Splunk SIEM and the BOTS v3 dataset to simulate real-world security investigations.

## Objectives
- Install and configure Splunk locally
- Ingest BOTS v3 dataset
- Detect brute-force attacks
- Analyze authentication logs
- Identify suspicious IP addresses

## Tools & Technologies Used

| Tool | Purpose |
|---|---|
| Splunk Enterprise | SIEM monitoring and log analysis |
| BOTS v3 Dataset | Real-world SOC investigation practice |
| Windows Event Logs | Authentication and security event analysis |
| Sysmon | Endpoint activity monitoring |
| Windows OS | Home lab environment |

## Home Lab Setup
The lab was created by installing Splunk locally on Windows and ingesting the BOTS v3 dataset for security monitoring and log analysis practice.

## Investigation Scenario
The project focused on detecting:
- Failed login attempts
- Suspicious authentication activity
- Brute-force attack patterns
- Malicious IP addresses

## Splunk Query Example

```spl
index=* EventCode=4625
| stats count by Account_Name, Source_Network_Address
| sort - count
```

## Skills Gained

- Splunk SIEM
- Log Analysis
- Threat Detection
- Authentication Monitoring
- IOC Identification
- Incident Triage
- SPL Query Writing
- Windows Event Log Analysis

## Challenges Faced

- Troubleshooting Splunk installation and storage path issues
- Understanding log ingestion and indexing processes
- Learning SPL query syntax and event correlation techniques
- Managing large datasets during analysis

## Conclusion

This project provided hands-on experience in building a SOC home lab using Splunk and the BOTS v3 dataset. Through authentication log analysis and brute-force attack investigations, I strengthened practical skills in SIEM monitoring, threat detection, and SOC investigation workflows.

## Future Improvements

- Improve Splunk search and log analysis skills
- Explore more SOC investigation scenarios using BOTS datasets
- Practice creating basic Splunk dashboards and alerts
- Learn more about Windows Event Logs and Sysmon analysis
- Continue building hands-on cybersecurity home lab projects
