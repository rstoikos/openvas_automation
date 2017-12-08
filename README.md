# openvas_automation
Automated openvas scanning with Python script and instalation with Ansible playbook

openvas.py creates a new scan for the requested subnet and produces an Html report. All the required arguments are created and passed to openvas cli hiding thus the complexity of this powerful software.

Our ansible playbook installs openvas and deals with the many errors that do not allow a fresh openvas instalation to start a scan immediately.

The point here is to simulate an automated instalation, scanning and to copy the report in our machine. For testing enviroment Vagrant was used with 3 Centos servers, and one Ubuntu machine was used to initiate the scanning.

