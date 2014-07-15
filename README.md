# Graphite service - Arch Linux ARM

## How to use?

First, find the pi on the network by doing an arp-scan:

    sudo /usr/local/bin/arp-scan --interface=en0 --localnet | grep b8:27:eb

Then copy your ssh key for automatic ansible authentication:

    ssh-copy-id root@1.2.3.4

Then run the playbook!

    ansible-playbook -i hosts site.yml