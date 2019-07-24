Role Name
=========

Automatically install zabbix ZoL userparameters on hosts that needs it. 

Requirements
------------

Needs https://share.zabbix.com/zfs-on-linux template imported on server.

Role Variables
--------------

None.

Dependencies
------------

dj-wasabi/zabbix-agent should be ran first, uses its variables to connect to zabbix server.

Example Playbook
----------------

    - name: deploy zabbix agent
      hosts: deploytest
      remote_user: root
      roles:
         - role: zabbix-agent
         - role: zabbix-zol

License
-------

BSD

Author Information
------------------

Dmitry Petuhov <mityapetuhov@gmail.com>
Installs userparameters and script from https://share.zabbix.com/zfs-on-linux AceSlash

