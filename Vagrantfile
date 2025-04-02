# -*- mode: ruby -*-
# vi: set ft=ruby :

Vagrant.configure("2") do |config|
  config.vm.box = "generic/ubuntu2004"
  
  config.vm.hostname = "monitoring-server"
  config.vm.network "forwarded_port", guest: 3000, host: 3000 # Grafana
  config.vm.network "forwarded_port", guest: 9090, host: 9090 # Prometheus
  config.vm.network "forwarded_port", guest: 9100, host: 9100 # node_exporter


  config.vm.provision :ansible do |ansible|
    ansible.playbook = "./ansible/playbook.yml"
    ansible.become = true
  end
  
end
