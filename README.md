# ansible-pi

A collection of ansible playbooks etc to configure your raspberry pi

## Getting started

### Install ansible locally
For macOS users this is easy with [brew](https://brew.sh):

    brew install ansible

### Create your inventory
Copy `inventory.template.yml` to `inventory.yml`.
Adjust at least the property ansible_host to your needs.

### Test your setup
Show your inventory:

    ansible-inventory

Gather ansible setup:

    ansible all -m setup

## Individual playbooks

Configure them first (adjust variables, i.e. as host-vars in your inventory.yml).
Then run them with `ansible-playbook <playbook.yml>`

### time-machine-target.yml

Configure pi as target device for Apples TimeMachine.
