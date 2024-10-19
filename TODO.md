# TODO

## Priorty

### High
- Add systemd service to autostart for samba container
- Add systemd service to autostart for homeassistant container
- Configure homeassistant to work with SELinux w/o disabling it

### Medium
- Add certificate for homeassistant
- Homeassistant recipe throws a warning on new install
```
[WARNING]: Module remote_tmp /var/home/piadmin/.ansible/tmp did not exist and was created with a mode of 0700, this may cause issues when running as another user. To avoid this, create the remote_tmp dir with the correct permissions manually
```
- Homeassistant logs show:
```
WARNING (MainThread) [bluetooth_adapters.dbus] DBus authentication error; make sure the DBus socket is available and the user has the correct permissions: authentication failed: REJECTED: ['EXTERNAL']
```

### Low
- Configure non-build tasks to run as unprivileged user
- Move extended packages to packages.json

## Ideas
- Add a Nix package manager (extended build?)
  - Add useful CLI tools via Nix (extended build?)
- Add Incus (full build?)
  - Add OMV via Incus (recipie?)
