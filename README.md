Kibana role
=========

Роль для установки Kibana на хостах с ОС: Debian, Ubuntu, CentOS, RHEL.

Requirements
------------

Поддерживаются только ОС семейств debian и EL.

Role Variables
--------------

Variable name	Default	Description  
kibana_version	"7.14.0"	Параметр, который определяет какой версии filebeat будет установлен


Example Playbook
----------------

```
# requirements.yml
---
- src: git@github.com:iv-art074/kibana_role.git
  scm: git
  version: "1.0.0"
  name: kibana-role

# site.yml
---
- name: Install Kibana 
  hosts: all
  roles:
    - kibana-role
  tags: kibana
  ``` 
  
License
-------

MIT

