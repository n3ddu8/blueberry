# TODO

## Priorty

### High
- Add systemd service to autostart for samba container
- Add systemd service to autostart for homeassistant container
- Configure homeassistant to work with SELinux w/o disabling it

### Medium
- Add certificate for homeassistant
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
