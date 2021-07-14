# ansible-zabbix-agent
Enabling the Zabbix Agent repository on Ubuntu &amp; Debian systems

## Why
I initially used dj-wasabi's Ansible module (https://galaxy.ansible.com/dj-wasabi/zabbix-agent) to install the Zabbix 4.4 Agent on my Debian & Ubuntu servers. Unfortunately, this is no longer maintained and so can't be used to provision the newer 5.0 LTS or 5.4 agents

## Full usage
Modify the yml files to make the hosts line match your configuration, then run either the Focal or Buster scripts against your hosts. These can also be modified to run on newer/older distributions of Debian/Ubuntu

## Remove 4.4 repositories only
If you previously used dj-wasabi's module, and only want to remove it, run the zabbix-remove-4-4.yml against your hosts. This will remove both the deb and deb-src repositories
