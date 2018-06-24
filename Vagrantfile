# -*- mode: ruby -*-
# vi: set ft=ruby :

Vagrant.configure("2") do |config|
  config.vm.box = "bento/ubuntu-16.04"

  config.vm.provision "ansible_local", run: "always" do |ansible|

    # Install Ansible using pip instead of the package manager
    ansible.install_mode = "pip"

    # Often a good idea to freeze it to a specific version
    # to ensure that your playbooks work a year later
    # ansible.version = "2.5.5"

    # Setting version to "latest" keeps ansible updated
    ansible.version = "latest"

    # Compatibility mode. For details, check the documentation:
    # https://www.vagrantup.com/docs/provisioning/ansible_common.html
    ansible.compatibility_mode = "2.0"

    ansible.playbook = "playbook.yml"
  end
end
