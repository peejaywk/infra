# infra
Home network configuration using infrastructure as code.

### Install Galaxy Roles
`ansible-galaxy install -r requirements.yml`

- Run the playbook:

`ansible-playbook playbook.yml`

- To run a particular section of the playbook:
`ansible-playbook playbook.yml --tags "docker"`
