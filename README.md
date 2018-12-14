# NetEye 4 Monitoring Fileshare setup 

This project aims to provide scripts, monitoring plugins and other useful data to setup a folder structure to simplify monitoring operations with NetEye 4.

## Features provided

- 010_init_neteyeshare.sh
  Create a folder structure for Agents, Monitoring Configuration and scripts under /neteye/shared/neteyeshare/

- 011_init_neteyeshare_weblink.sh
  Initialize an Apache Alias with authentication for neteyeshare access wia https

- 020_get_icinga2_agents.sh
  Fetch Icinga2 Agents from packages.icinga.org and store in /neteye/shared/neteyeshare/monitoring/agents/

- 030_ressources_init.sh
  Define sample Ressource for LDAP bind.

- 040_monitoring_templates_init.sh
  Provide monitoring templates for Icinga Director in neteyeshare

- 050_monitoring_plugins.sh
  Provide monitoring plugins neteyeshare

- 051_monitoring_plugins_activate.sh
  Activate useful monitoring plugins in PluginsContribDir

- 052_monitoring_configurations.sh
  Place additional Icinga2 monitoring configuration into neteyeshare. 
  a) Provide general Dependency apply rule to implement a parent-child hierarchy

- 053_monitoring_analytics.sh
  Place sample Analytics dashboards into neteyeshare.
  a) generic_services_by_hosts.json
  b) generic_snmp_interfaces.json



## Install:

Clone git repository to NetEye filesystem
```
git clone https://github.com/zampat/neteye4_monitoring_share.git
```

Run configuration and setup script
```
./neteye4_monitoring_share/run_setup.sh
```
