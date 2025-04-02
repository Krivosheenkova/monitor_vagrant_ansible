## DevOps Engineer Test Task
---
### Project Overview
- Vagrant is used to create and manage the virtual machine
- Ansible automates node_exporter and monitoring server setups
- Docker-compose manages the deployment of Prometheus and Grafana alongside using the same local network
- Node Exporter collects system metrics, configured in Prometheus for monitoring
- Grafana provides visualization of the metrics obtained from Prometheus

### Installation and Usage
#### Prerequisites
Make sure you have the following tools installed:
- Vagrant
- VirtualBox
- Ansible

1. Clone the Repository:
```
git clone https://github.com/Krivosheenkova/monitor_vagrant_ansible.git
cd monitor_vagrant_ansible/
```

2. Install Ansible requirements:
```
ansible-galaxy install -r requirements.txt
```

3. Start VM:
```
vagrant up
```

3. Access Grafana
Open your browser and navigate to http://localhost:3000

Use the default credentials:
    username: admin
    password: admin
