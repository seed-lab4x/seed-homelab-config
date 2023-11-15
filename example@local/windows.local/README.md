# windows.local

This is the __level 2__ config.

`windows.local` is a domain name, `*.local` domain generally points to `127.0.0.1`,
Usually by setting dnsmasq `--address` option on the router (such as openwrt) for work.

## content

There are usually several necessary files or directories here.

```bash
.
├── ansible-inventories/
├── other/
└── requirements.yml
```

`ansible-inventories` should always exist, 
this is the inventory directory of ansible, see ansible [intro_inventory](https://docs.ansible.com/ansible/latest/inventory_guide/intro_inventory.html#organizing-inventory-in-a-directory).
`requirements.yml` should exist,
it is recommended to set it to executable, see ansible galaxy [user_guide](https://docs.ansible.com/ansible/latest/galaxy/user_guide.html#installing-roles-and-collections-from-the-same-requirements-yml-file).

## run

You should always open a terminal in this directory and run a script or playbook.

When you open the terminal, the terminal displays as follows

```bash
xy@INTC-NUC13:/mnt/f/code/seed-lab4x/seed-homelab-workspace/.config/example@local/windows.local$ 
```

At this time you can run the script or playbook. 
Usually the scripts or playbooks in this project are executable,
Just type the file path or drag the file into it and press *Enter* to run it.


```bash
xy@INTC-NUC13:/mnt/f/code/seed-lab4x/seed-homelab-workspace/.config/example@local/windows.local$ '/mnt/f/code/seed-lab4x/seed-homelab-workspace/.seed/ansible-playbook/seed-local.init.yml'
```
