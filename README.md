# Project Blueberry: A Custom Buildkit for running Fedora IOT on Raspberry Pi.

## Installing Fedora IOT on a Raspberry Pi

```shell
sudo arm-image-installer --image=Fedora-IoT-raw-40-20240422.3.aarch64.raw.xz --media=/dev/sdc --addkey=/var/home/n3ddu8/.ssh/id_rsa.pub --norootpass --resizefs --target=rpi4 -y
```

## Using Project Blueberry

- Update the file `group_vars/edge.yaml`.

- Confirm connection with remote pi:
```shell
ansible edge -i inventory.yaml -m ping
```

- Run playbook:
```shell
ansible-playbook -i inventory.yaml playbook.yaml
```
