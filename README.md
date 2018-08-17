# Ansible CSR generator

Easily create a certificate signing request using Ansible


## Usage

    ansible-playbook csr-generator.yml -e "common_name=example.com country=GB state=foo locale=foo organisation=foo oraganizationalunit=foo emailaddress=foo"

By default the private key and CSR are stored in their respective folders within /etc/ssl. If the respective folders do not exist, this script will create them. If this is not desired then feel free to modify.

The script will then output the CSR and private key within a debug output at the end of the script.
