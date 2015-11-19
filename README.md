# custom zabbix scripts

## Description

This is a project inspired and adapted from https://github.com/zbal/zabbix. The purpose of our project is to fix the problem existed in prior project due to out of date and lack of maintenance.

## Installation

### Prerequisite

* zabbix agent has been deployed to the machine you try to monitor.

### Manual Installation

* create folder if not exists: `/usr/lib/zabbix`
* move `scripts` folder in this project to `/usr/lib/zabbix/` in remote server you try to monitor.
* move all files in `userparameters` folder in this project to remote server.
* restart zabbix-agent with command like `sudo service zabbix-agent restart`

### check if it works

`telent 127.0.0.1 10050`, input `apache[cpuload]`, the expected result is like: `ZBXD     .0433374`
