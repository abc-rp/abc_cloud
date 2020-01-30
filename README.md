# Installation

ABC Cloud Installer

The purpose of this repository is to provide a set of Ansible playbooks that can be used to install a range of ABC Cloud components via Ansible on Kubernetes (k8s).

These include:

- Grafana
- MQTT Broker
- TICK Stack

We will initially target Google Kubernetes Engine (GKE) and k3s.

    ansible-playbook --ask-pass -i inventories/abc.template playbooks/install.yml

