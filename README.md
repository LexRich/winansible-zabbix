# Ansible role for install Zabbix-Agent on the Windows


##### # Install WinRM module for ansible:
`pip install https://github.com/diyan/pywinrm/archive/master.zip#egg=pywinrm`


##### # Activate WinRM module in Windows: 
```
@powershell -NoProfile -ExecutionPolicy Bypass -Command "iex ((new-object net.webclient).DownloadString('https://github.com/ansible/ansible/raw/devel/examples/scripts/ConfigureRemotingForAnsible.ps1'))"
```



Change variable Zabbix-Server IP in the vars/main.yml: `zabbix_ip_server`


Zabbix-agent version 3.4.6: [https://www.zabbix.com/downloads/3.4.6/zabbix_agents_3.4.6.win.zip](https://www.zabbix.com/downloads/3.4.6/zabbix_agents_3.4.6.win.zip)


ZABBIX share: [https://share.zabbix.com/installers/ansible-playbook-for-install-agent-on-the-windows](https://share.zabbix.com/installers/ansible-playbook-for-install-agent-on-the-windows)
