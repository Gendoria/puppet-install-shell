# -*- mode: ruby -*-
# vi: set ft=ruby :

Vagrant.configure("2") do |config|

  # Want to make sure cachier doesn't give false positives
  if Vagrant.has_plugin?("vagrant-cachier")
    config.cache.auto_detect = false
  end

  config.vm.provider "virtualbox" do |v|
    # v.gui = true
  end

  config.vm.define "centos65" do |centos65|
    centos65.vm.box = "centos6.5"
    centos65.vm.box_url = "http://puppet-vagrant-boxes.puppetlabs.com/centos-65-x64-virtualbox-nocm.box"
  end

  config.vm.define "precise64" do |precise64|
    precise64.vm.box = "precise64"
    precise64.vm.box_url = "http://files.vagrantup.com/precise64.box"
  end

  config.vm.define "quantal64" do |quantal64|
    quantal64.vm.box = "quantal64"
    quantal64.vm.box_url = "http://cloud-images.ubuntu.com/vagrant/quantal/current/quantal-server-cloudimg-amd64-vagrant-disk1.box"
  end

  config.vm.define "saucy64" do |saucy64|
    saucy64.vm.box = "saucy64"
    saucy64.vm.box_url = "http://cloud-images.ubuntu.com/vagrant/saucy/current/saucy-server-cloudimg-amd64-vagrant-disk1.box"
  end

  config.vm.define "trusty64" do |trusty64|
    trusty64.vm.box = "trusty64"
    trusty64.vm.box_url = "https://cloud-images.ubuntu.com/vagrant/trusty/current/trusty-server-cloudimg-amd64-vagrant-disk1.box"
  end

end
