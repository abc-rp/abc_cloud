# Installation

ABC Cloud Installer

The purpose of this repository is to provide a set of Ansible playbooks that can be used to install a range of ABC Cloud components via Ansible on Kubernetes (k8s).

These include:

- [Grafana](https://github.com/integr8ly/grafana-operator)
- [MQTT Broker](https://github.com/EnMasseProject/enmasse)
- [TICK Stack](https://github.com/influxdata/influxdata-operator)

We will initially target Google Kubernetes Engine (GKE) and k3s.

    git clone https://github.com/active-building-centre/installation.git
    cd installation

If running on a cluster with local_path storage:

    ansible-playbook -i inventories/k3s.template playbooks/install.yml

If running on GKE:

    ansible-playbook -i inventories/gke.template playbooks/install.yml