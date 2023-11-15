# example@local

This is the __level 1__ config.

## content

There are two naming methods for the __level 2__ host directory,
one is named by the host domain name, the other is named by system type group.
In the latter case it will be possible for once host to be in multiple host directories.

like this:

```bash
.
├── openwrt@home
└── windows.local
```

`openwrt@home` is named by system type group.
other `windows.local` are named by host domain name.

If part of host directory hosts is unreachable, or just want to run playbook on one host use [override-hosts](#override-hosts).


### override-hosts

Select host from all hosts just `--limit` option run ansible-playbook, [see](https://stackoverflow.com/a/57395307)

use `ansible-playbook` command

```bash
ansible-playbook -i openwrt@home/ansible-inventories --limit k3.lan
```

use executable playbook file

```bash
/seed-homelab-workspace/openwrt/image/ansible-playbook.build.yml -l k3.lan
```
