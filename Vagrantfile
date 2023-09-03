# -*- mode: ruby -*-
# vi: set ft=ruby :

VAGRANTFILE_API_VERSION = "2"

Vagrant.configure(VAGRANTFILE_API_VERSION) do |config|
  config.vm.define "ansible-homeserver-test" do
    config.vm.box = "ubuntu/focal64"
    config.vm.hostname = "homeserver.test"
    config.vm.network :private_network, ip: "192.168.56.55"
    config.ssh.insert_key = false
    config.vm.synced_folder ".", "/vagrant", disabled: true

    config.vm.provider :virtualbox do |v|
      v.memory = 2048
    end

    # Ansible provisioner.
    #config.vm.provision :ansible do |ansible|
    #  ansible.playbook = "provisioning/playbook.yml"
    #end
  end
end

