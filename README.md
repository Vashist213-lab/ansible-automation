# Ansible starter template

## Overview

This is the starter code for an automation setup using Ansible. Roles are missing and should be
created. Please check the following sections for more details about how to get started and for
instructions to build the docker-compose.yml files.

## Getting Started

```bash
# Clone the project
git clone https://github.com/EdgeKing810/interns-ansible-automation.git
cd interns-ansible-automation/

# Make sure you have python installed
sudo apt update
sudo apt install -y python3 python3-virtualenv python3.10-venv python3.11-venv

# Create and setup the virtualenv
python3 -m venv .venv
source .venv/bin/activate
pip install --upgrade pip setuptools wheel
pip install -r requirements.txt
ANSIBLE_CONFIG=./ansible.cfg ansible-galaxy collection install -r requirements.yml
```

Please make sure that you have docker installed on your system before continuing.

## Instructions

1. Files found in sub-directories of `playbooks/roles/` contain comments that need
to be resolved.
2. Run the `ansible-playbook playbooks/main.yml -v` command to test whether everything
runs properly.
3. Run the `ansible-lint` command and ensure that all issues are resolved.
