# Tutorial Ansible + Docker-Swarm + Portainer
https://www.youtube.com/watch?v=UoBf18JCF9o

# Tutorial Portainer Templating
https://www.youtube.com/watch?v=nmas_zbcMeU&t=928s

# Tutorial Traefik
https://www.youtube.com/watch?v=zg-rL7n_t-A

# Insall in Mac
brew install ansible

# Vault usage
copy inventory/managers/vault.example to vault.yaml and fill the credentials
ansible-vault encrypt inventory/group_vars/managers/vault.yaml 

# To edit vault, decrypt it, edit and re-encrypt
ansible-vault decrypt inventory/group_vars/managers/vault.yaml 

# Run Playbook
ansible-playbook site.yaml --ask-vault-pass