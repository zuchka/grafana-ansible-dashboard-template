## Prerequisites:

* Ansible installed on your local machine

* A Virtual Machine running Ubuntu 20

## Steps

* Clone this repo

* Now use the Ansible CLI on your local machine (or control node) to install `community.grafana`:

```
ansible-galaxy collection install -r ./requirements.yml
```

* Before running the playbook, make sure to set the variables in `vars.yml` and `hosts` to match your grafana instance.

* Now run the playbook, changing `your-vm-user` to the user on your Grafana instance:

```
ansible-playbook -i ./hosts grafana.yml -l server1 -u your-vm-user -vvvvv
```
