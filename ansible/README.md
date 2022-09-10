```
Ansible Command
ansible-playbook --ask-become-pass install_apache.yml
```



```
Ansible Command
ansible-playbook --ask-become-pass install_apache.yml
```


```
Ansible Command
ansible all -m gather_facts --limit server1 | grep ansible_distribution
```


```
Ansible Command
ansible-playbook --list-tags site.yml
```



```
Ansible Command
ansible-playbook --tags centos -K site.yml
```



```
Ansible Command
ansible-playbook --tags "db, apache" -K site.yml
```








