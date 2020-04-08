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

    ansible-playbook -i inventories/gke.template playbooks/install.yml -e lets_encrypt_email=<your email> -e gke_project=<your project>

These playbooks are tested on Kubernetes 1.15+ and if using cert-manager this is a dependency.

![system diagram](https://docs.google.com/drawings/d/e/2PACX-1vTZfKZIDEEScdSg60ew5PWjDPDEjWVbA5djhbiDbJDMwePXs_LW_7SpuPlONS42hevcjGfNuIhYbswT/pub?w=1229&h=686 "System Diagram")

