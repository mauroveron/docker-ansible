Ansible
=======

Ansible 2.7 running on Alpine 3.8 & Python 3

Run as

```
docker run --rm \
	-it \
	-v ${PWD}/hosts:/etc/ansible/hosts \
	-v ${PWD}/ansible.cfg:/etc/ansible/ansible.cfg \
	-v ${HOME}/.ssh:/root/.ssh:ro \
	ansible all -m ping
```