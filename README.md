Sawtooth-ansible

This repository provides a set of generic Ansible roles that can be
used as building blocks for creating a sawtooth network.

1) Modify the hosts file to match the network, host names, and IP addresses to
match the environment. See hosts-example to get started.

2) Create a configuration yaml file based off the config-example.yaml. Here
you can modify several parameters used for installation, and configuration.

2) Create playbooks to put the rolls together. A couple playbooks are provided
showing ways these roles can be used.

Usage
`ansible-playbook -i hosts --extra-vars "@./configs/config.yaml" -f 2 sawtooth-deploy.yaml`
