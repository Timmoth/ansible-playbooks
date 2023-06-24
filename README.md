# ansible-playbooks

## secure-shell.yml
* Adds your public key to the remote server
* Disable empty password login
* Disable root login
* Disable password login
* Disable Challenge Response Authentication
* Disable Password Authentication
  
```
# generate ssh keys id_rsa & id_rsa.pub
ssh-keygen

# define vars in hosts
[servers:vars]
ssh_user=<your ssh user>
ssh_pub_key=<path to id_rsa.pub>

# run
ansible-playbook secure-ssh.yml -kK
