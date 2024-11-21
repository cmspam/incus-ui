# incus-ui
Automatic daily repackaged incus-ui based on incus-ui-canonical deb packages from [Zabbly](https://github.com/zabbly/incus).

These are tarballs of pre-built /opt/incus/ui folder from his deb packages, and ready to drop into /opt/incus/ or wherever you like:

```
tar xvf incus-ui-stable.tar.gz -C /opt/incus/
```

Assuming you dropped the files into /opt/incus/ give incusd the environment variable: 
```
INCUS_UI=/opt/incus/ui
```

The place to put the environment variable might differ depending on how incus was packaged. It could go direclty in the init file/systemd file, or there may be another script somewhere like `/opt/incus/systemd/incusd`

