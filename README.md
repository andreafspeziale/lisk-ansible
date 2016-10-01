# lisk-ansible
This repository uses Vagrant + Ansible to create a Lisk node environment without pain.<br>
It will also install the Node + packages and some other utils like MongoDB.

# Pre-req
    - virtualbox

# Req
    - Ansible 2+
    - Vagrant

# Install
    - ansible-galaxy install -r requirements.yml
    - vagrant up

# Notes
At this point you will have a running lisk node.
You can check if localhost:7000 responses with the node interface.

You can also check the loading status of bloackchain with this api

    - localhost:7000/api/loader/status/sync

# ToDo
    - after turning the VM off and on, check if lisk has started
    - use custom templates for the lisk config.json
    - useful bash profile
    - install jq
    - make auto apt upgrade-update
    - install git -.-
