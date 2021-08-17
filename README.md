Prerequisites:

Ansible installed on your local machine

A Virtual Machine running Ubuntu 20

Clone this repo

Now use the Ansible CLI on your local machine (or control node) to install `community.grafana`:

```
ansible-galaxy collection install -r ./requirements.yml
```

then run the playbook:

```
ansible-playbook -i ./hosts grafana.yml -l server1 -u your-vm-user -vvvvv
```

Make sure to set the variables in `vars.yml` and `hosts` to match your grafana instance.