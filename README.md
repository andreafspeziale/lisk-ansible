# lisk-ansible
###With love by liskit delegate, for donation 10310263204519541551L

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

Now is possible to connect to Lisk PGSQL DB from a client (like http://www.psequel.com/) using:

    - localhost as host
    - vagrant as user
    - password as password
    - lisk_test as DB

This is very useful for and ONLY LOCAL DEVELOPMENT

# ToDo
    - use custom templates for the lisk config.json
    - useful bash profile
    - install jq
    - install git and more -.-
