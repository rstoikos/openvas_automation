# openvas_automation
Automated openvas scanning with Python script and instalation with Ansible playbook

openvas.py creates a new scan for the requested subnet and produces an Html report. All the required arguments are created and passed to openvas cli hiding thus the complexity of this powerful software.

Our ansible playbook installs openvas and deals with the many errors that do not allow a fresh openvas instalation to start a scan immediately.

The point here is to simulate an automated instalation, scanning and to copy the report in our machine. For testing enviroment Vagrant was used with 3 Centos servers, and one Ubuntu machine was used to initiate the scanning.

Report Sample


Summary

This document reports on the results of an automatic security scan. The report first summarises the results found. Then, for each host, the report describes every issue found. Please consider the advice given in each description, in order to rectify the issue.

Vendor security updates are not trusted.

Overrides are off. Even when a result has an override, this report uses the actual threat of the result.

Notes are excluded from the report.

This report might not show details of all issues that were found. It only lists hosts that produced issues. Issues with the threat level "False Positive" are not shown.

This report contains all 103 results selected by the filtering described above. Before filtering there were 190 results.

All dates are displayed using the timezone "Coordinated Universal Time", which is abbreviated "UTC".
Scan started: 	Fri Dec 8 12:41:03 2017 UTC
Scan ended: 	Fri Dec 8 14:38:41 2017 UTC
Task: 	My scan
Host Summary
Host 	Start 	End 	High 	Medium 	Low 	Log 	False Positive
192.168.60.1 	Dec 8, 12:41:19 	Dec 8, 14:38:17 	1 	1 	1 	31 	0
192.168.60.5 (orc-app2) 	Dec 8, 12:41:23 	Dec 8, 14:38:38 	1 	2 	1 	13 	0
192.168.60.7 	Dec 8, 12:41:23 	Dec 8, 14:33:06 	0 	1 	0 	27 	0
192.168.60.4 	Dec 8, 12:41:22 	Dec 8, 14:17:52 	0 	1 	1 	10 	0
192.168.60.6 	Dec 8, 12:41:22 	Dec 8, 14:17:38 	0 	1 	1 	10 	0
Total: 5 			2 	6 	4 	91 	0
