
# wp-ubuntu

# Installing wordpress with ansible 2.9.6

## Used Ubuntu 18.04.2 LTS ##

# Edit inventory file, installation can be done on localhost.

#vim hosts

[wordpress]

127.0.0.1

# Access the wp-ubuntu directory and execute the commands

# To test host communication

#ansible localhost -m ping

## Run the file # playbook.yml

#ansible-playbook playbook.yml
