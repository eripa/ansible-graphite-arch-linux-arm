# Ansible - Graphite - Arch Linux ARM

**Status: not in a working state!**

## How to use?

First, find the ip of your ALARM machine, For Raspberry Pi you do an arp-scan, something like this:

    sudo /usr/local/bin/arp-scan --interface=en0 --localnet | grep b8:27:eb

Then copy your ssh key for automatic Ansible authentication:

    ssh-copy-id root@1.2.3.4

Then run the playbook!

    ansible-playbook -i hosts site.yml