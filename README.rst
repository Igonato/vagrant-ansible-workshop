Vagrant Ansible Workshop
========================
Simple vagrant box with ansible installed.

Are you working with Ansible on Windows?
Do you want to have a consistent environment to run your playbooks?
Maybe you want to test a specific Ansible version?

.. code:: bash

    $ git clone git@github.com:Igonato/vagrant-ansible-workshop.git
    $ cd vagrant-ansible-workshop
    $ vagrant up  # Might take some time to download the box and install ansible
    $ vagrant ssh
    ...
    vagrant@vagrant:~$ ansible --version
    ansible 2.5.5
