# Health Insurance Portability and Accountability Act (HIPAA)

[![Build Status](https://travis-ci.org/RedHatOfficial/ansible-role-rhel7-hipaa.svg?branch=master)](https://travis-ci.org/RedHatOfficial/ansible-role-rhel7-hipaa)
[![Ansible Role](https://img.shields.io/ansible/role/39709.svg)](https://galaxy.ansible.com/RedHatOfficial/rhel7_hipaa)
[![GitHub release](https://img.shields.io/github/release/RedHatOfficial/ansible-role-rhel7-hipaa.svg)](https://github.com/RedHatOfficial/ansible-role-rhel7-hipaa/releases/latest)

Ansible Role for Health Insurance Portability and Accountability Act (HIPAA)

Profile Description:  
The HIPAA Security Rule establishes U.S. national standards to protect individuals'  
electronic personal health information that is created, received, used, or  
maintained by a covered entity. The Security Rule requires appropriate  
administrative, physical and technical safeguards to ensure the  
confidentiality, integrity, and security of electronic protected health  
information.  
  
This profile configures Red Hat Enterprise Linux 7 to the HIPAA Security  
Rule identified for securing of electronic protected health information.

The tasks that are used in this role are generated using OpenSCAP.
See the OpenSCAP project for more details on Ansible playbook generation at [https://github.com/OpenSCAP/openscap](https://github.com/OpenSCAP/openscap)

To submit a fix or enhancement for an Ansible task that is failing or missing,
see the ComplianceAsCode project at [https://github.com/ComplianceAsCode/content](https://github.com/ComplianceAsCode/content)

## Requirements

- Ansible version 2.5 or higher

## Role Variables

To customize the role to your liking, check out the [list of variables](vars/main.yml).

## Dependencies

N/A

## Example Playbook

Run `ansible-galaxy install RedHatOfficial.rhel7_hipaa` to
download and install the role. Then you can use the following playbook snippet.


    - hosts: all
      roles:
         - { role: RedHatOfficial.rhel7_hipaa }


Then first check the playbook using (on the localhost):

    ansible-playbook -i "localhost," -c local --check playbook.yml

To deploy it, use (this may change configuration of your local machine!):

    ansible-playbook -i "localhost," -c local playbook.yml


## License

BSD-3-Clause

## Author Information

This Ansible remediation role has been generated from the body of security
policies developed by the ComplianceAsCode project. Please see
[https://github.com/complianceascode/content/blob/master/Contributors.md](https://github.com/complianceascode/content/blob/master/Contributors.md)
for an updated list of authors and contributors.
