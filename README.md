falcon-agent
===

fork自 openfalcon-agent，在此基础上 doing | to do 以下：
  - 取消api中的endpoint字段，改为从系统hostname中获取；
  - 增加参数，可以enable/disable http api，作为monitor service时使用；

===

This is a linux monitor agent. Just like zabbix-agent and tcollector.


## Installation

It is a golang classic project

```bash
# set $GOPATH and $GOROOT
mkdir -p $GOPATH/src/github.com/open-falcon
cd $GOPATH/src/github.com/open-falcon
git clone https://github.com/open-falcon/agent.git
cd agent
go get ./...
./control build
./control start

# goto http://localhost:1988
```

I use [linux-dash](https://github.com/afaqurk/linux-dash) as the page theme.

## Configuration

- heartbeat: heartbeat server rpc address
- transfer: transfer rpc address
- ignore: the metrics should ignore

# Deployment

http://ulricqin.com/project/ops-updater/

