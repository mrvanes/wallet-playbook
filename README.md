# wallet-playbook
wallet-ecosystem ansible playbook

Create a new environment by copying demo or w100 environement.

Copy environments/<new env>/secrets.yml.example to secrets.yml and add valid github_token and github_ssh_key.

Adjust environments/<new env>/inventory to reflect target host(s).

Adjust environments/<new env>/group_vars/all.yml to reflect desired configuration.

You need an account and ssh access with sudo rights on the target host(s).

Deploy Wallet-Ecosystem:
```
$ ansible-playbook playbook.yml [-i environments/demo/inventory] <--tags tag,tag,tag>
```
