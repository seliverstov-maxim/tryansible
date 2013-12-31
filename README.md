Try Ansible
==========

First need clone repository.
```
git clone git@github.com:seliverstov-maxim/tryansible.git
cd ./tryansible
```
then update 'hosts' file
```
162.243.194.158 ansible_connection=ssh ansible_ssh_user=root
```
to
```
<ip_your_server> ansible_connection=ssh ansible_ssh_user=<remote_user>
```

CHECK
==========
Can you get ssh access to you server, like
```
ssh <user>@<server_addr>
```
for instance
```
ssh root@162.243.194.158
```

Cook
==========
```
ansible-playbook playbooks/common.yml -i ./hosts
```

Hist
==========
v1
- postgresql
- git
- curl
