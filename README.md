# Kubernetes Cluster on DO
---

This repository contains the Ansible playbooks for standing up a simple Kubernetes cluster on 3 Ubuntu droplets. This is a constantly updated repository as I build on this for my own uses.

##Requirements

- 3x Ubuntu 16.04 Droplets
- Fill out hosts file with the IPs for you droplets
- Ensure droplets have your local SSH key added in creation.

##To Run

- `ansible-playbook -i hosts initial.yml`
- `ansible-playbook -i hosts kube-dependencies.yml`
- `ansible-playbook -i hosts master.yml`
- `ansible-playbook -i hosts workers.yml`

