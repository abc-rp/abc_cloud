# Installation

**ABC Cloud Installer**

> Note: This repo is archived.  Our focus is now supporting the development of [Drogue IoT](https://www.drogue.io/).


The purpose of this repository is to provide a set of playbooks that can be used to configure and install a range of ABC Cloud components via Ansible on Kubernetes (k8s).

These include:

- Core messaging and IoT infrastructure (based on [enmasse](https://enmasse.io/))
- Example [TICK](https://www.influxdata.com/time-series-platform/) + [Grafana](https://grafana.com/) application

We are initially targeting Google Kubernetes Engine (GKE) and K3S with the ambition of being disto agnostic.

## Documentation

For design documentation and guides please visit the [project wiki](https://github.com/active-building-centre/installation/wiki).

Component diagram:

![system diagram](https://docs.google.com/drawings/d/e/2PACX-1vTZfKZIDEEScdSg60ew5PWjDPDEjWVbA5djhbiDbJDMwePXs_LW_7SpuPlONS42hevcjGfNuIhYbswT/pub?w=1229&h=686 "System Diagram")

*Image derived from the enmasse project.*
