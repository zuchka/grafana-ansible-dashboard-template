## Prerequisites:

* Ansible installed on your local machine

* Grafana 7+ installed and configured on a machine running Ubuntu 18+

* A Grafana API Token

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
