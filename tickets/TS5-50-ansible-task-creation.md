# TS5-50 – Create Tasks Using Ansible Playbook

## Summary
Automated common system administration tasks using Ansible, including local user creation, password expiration enforcement, and package installation. This ticket demonstrates task-based automation, idempotent playbook execution, and validation through command-line verification.

## Environment
- OS: RHEL / CentOS / Rocky Linux
- Automation Tool: Ansible
- Target: Localhost and managed Linux systems
- Privilege Escalation: sudo / become

## Requirements
- Create a local user account
- Force password expiration on first login
- Install required system packages
- Ensure tasks are repeatable and idempotent
- Validate changes after execution

## Implementation

### Playbook Overview
```yaml
- name: Create local user, expire password, and install tmux
  hosts: localhost
  become: yes

  tasks:
    - name: Create local user tfleming
      user:
        name: tfleming
        state: present
        shell: /bin/bash
        create_home: yes

    - name: Expire tfleming password
      command: chage -d 0 tfleming

    - name: Install tmux
      yum:
        name: tmux
        state: present

## Execution

The playbook was executed using:
ansible-playbook create_tfleming_tmux.yml

## Validation

- Verified user account exists
- Confirmed password expiration is enforced
- Confirmed tmux package is installed
- Play recap shows successful execution with no failures


