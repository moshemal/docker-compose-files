## Check setup
The vm.max_map_count setting should be set permanently in /etc/sysctl.conf:
```bash
grep vm.max_map_count /etc/sysctl.conf
vm.max_map_count=262144
```

## Setup
To apply the setting on a live system type:
```bash
sudo sysctl -w vm.max_map_count=262144
```