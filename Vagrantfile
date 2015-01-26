# -*- mode: ruby -*-
# vi: set ft=ruby :

Vagrant.configure("2") do |config|

  config.vm.define :centos do |d|
    d.vm.box = "hfm4/centos6"
  end

  config.vm.define :ubuntu do |d|
    d.vm.box = "ubuntu-12.04-amd64"
    d.vm.box_url = "https://cloud-images.ubuntu.com/vagrant/precise/current/precise-server-cloudimg-amd64-vagrant-disk1.box"
  end

  config.vm.provider :virtualbox do |v|
    # v.customize ["modifyvm", :id, "--memory", "1024"]
  end

  config.vm.provider :docker do |d|
    d.image = "ubuntu:precise"
    # d.build_dir = "docker"
  end
  # config.vm.network "forwarded_port", guest: 80, host: 8080
  # config.vm.network "private_network", ip: "192.168.33.10"
  # config.vm.network "public_network"

  # config.vm.synced_folder "../data", "/vagrant_data"

end
