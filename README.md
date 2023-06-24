# ansible-playbooks

## secure-shell.yml
```
define vars:
ssh_user=<your ssh user>
ssh_pub_key=<path to id_rsa.pub>

run:
ansible-playbook secure-ssh.yml -kK
