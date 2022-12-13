# SLURM monitoring & logging practice

This Ansible playbook installs Prometheus with node_exporter and EFK stack on Ubuntu 20.04:

    - prometheus
    - node_exporter
    - fluent_bit
    - elasticsearch_and_kibana

To run this playbook make sure you have all neccessary requirements:
```
python -m pip install -r requirements.txt
```

Then start virtual machine with supplied Vagrantfile:

```
vagrant up
```


Finally run the playbook:

```
ansible-playbook monitoring_practice.yml
```

