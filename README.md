First use the Ansible CLI on your local machine (or control node) to install `community.grafana`:

```
ansible-galaxy collection install -r ./requirements.yml
```

then run the playbook:

```
ansible-playbook -i ./hosts grafana.yml -l server1 -u your-vm-user -vvvvv
```

Make sure to set server1 to your ip or FQDN for your grafana instance