# Use Ansible Playbook
```

ansible-playbook playbook.yml -i hosts

```


# Use Dynamic Inventory
```

pip install boto
pip install ansible

export AWS_ACCESS_KEY_ID='AK123'

export AWS_SECRET_ACCESS_KEY='abc123'

export EC2_INI_PATH=/Users/gianpaoloriva/Documents/Workshop/Ansible/ansible/inventory/my_ec2.ini
python ec2.py

es. ansible-playbook -i ./ec2.py --limit "tag_App_backend:&tag_Environment_staging:&tag_Usage_clock_worker" playbook.yml
   
```
