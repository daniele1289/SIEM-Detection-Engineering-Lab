# SIEM-Detection-Engineering-Lab
Map to MITRE ATT&CK Take 5-10 common attack techniques from the MITRE ATT&amp;CK framework (like T1059 Command &amp; Scripting Interpreter) and write detection logic for each one in Splunk or Elastic. Document each use case with the attack description, detection rule, and expected alert output.


# Day 1 Notes
What is a SIEM?
- SIEM short for "Security Information and Event Management" is a cybersecurity technology that provides a single, streamlined view of your data, insight into security activities, and operational capabilities so you can stay ahead of yoru cyber threats

Why do organizations use SIEM?
- Organizations use SIEM systems to aggregate, analyze, and monitor log data from across their entire IT infrastructure in real time. It serves as a central nervous system for security teams, allowing them to manage their security posture from a single platform.

Logs and Metrics
- Almost all programs emit activities that occur within their program flow in the form of a log
- Logs provide detailed, timestamped records of events, making them crucial for root cause analysis and auditing
- Metrics capture structured numerical data over time, ideal for tracking trends, performance, and generating real-time alerts


Windows Event ID Cheat Sheet
4624 - This event occurs when a logon session is created. It generates on the computer that was accessed, where the session was created.(account successfuly logged on)

4625 - Security audit log that records every failed logon attempt on a local Windows system(generates on exact computer login was attempted)

4688 - Generated every time a new process has been created on a Windows system

4697 - This event occurs when a new service was installed into the system

7045- Crucial system log that records  when a new service or driver is successfully installed on your computer(difference from 4697 is that 7045 is a native System log while 
4697 is a Security auditing event)

1102 - This event indicates that the Windows Security audit log is cleared


# Day 2 Notes
Detection Engineering Notes
