### Ansible playbook for setup Zabbix-Agent on Windows


##### # Install WinRM module for ansible:
`pip install https://github.com/diyan/pywinrm/archive/master.zip#egg=pywinrm`


##### # Activate WinRM module in Windows: 
```
@powershell -NoProfile -ExecutionPolicy Bypass -Command "iex ((new-object net.webclient).DownloadString('https://github.com/ansible/ansible/raw/devel/examples/scripts/ConfigureRemotingForAnsible.ps1'))"
```


##### # How to use:
Change variable Zabbix-Server IP in the playbook: `zabbix_ip_server`

Use: `ansible-playbook -i inventory zabbix-agent/zabbix.yml --ask-pass`


Zabbix-agent version 3.4.6: [https://www.zabbix.com/downloads/3.4.6/zabbix_agents_3.4.6.win.zip](https://www.zabbix.com/downloads/3.4.6/zabbix_agents_3.4.6.win.zip)


ZABBIX share: [https://share.zabbix.com/installers/ansible-playbook-for-install-agent-on-the-windows](https://share.zabbix.com/installers/ansible-playbook-for-install-agent-on-the-windows)
