# Kazan ansible 🧊

Ansible plays for configuring kazan kubernetes cluster worker, controller and load balancing nodes.

Terraform project for infrastructure: [https://github.com/kevinmidboe/kazan-terraform](https://github.com/kevinmidboe/kazan-terraform)

## Setup
Currently requires a lot of certificate generation which is references in these plays as `/kazan-ssl`. Want to move to vault or at least script it.

Change values in `kazan.ini` to match your configuration.

## Run

```
ansible-playbook -i kazan.ini plays/launch.yml
```

If you don't have ansible-playbooks yet download following these instructions: [https://docs.ansible.com/ansible/latest/installation_guide/intro_installation.html](https://docs.ansible.com/ansible/latest/installation_guide/intro_installation.html)