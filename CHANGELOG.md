**** Zamba LXC Toolbox main branch ****
- added dhcp support
- fixed hardcoded samba sharename in `zmb-standalone` script
- added support for container id's larger than 999

**** Zamba LXC Toolbox v0.1 ****
- `locales` are now configured noninteractive #21
- timezone is now configured with `pct set` command in `install.sh` #22
- changed command sequence in `install.sh` - select container first, then start the installation
- improved / updated documentation
- replaced `just-lxc` container by `debian-priv` and `debian-unpriv` container
- (un)privileged now defined as constant based on created service #6
- improved log messages in `install.sh`
- `mailpiler`: website is now also `default_host`, removed nginx default site, dns entry is still required
- changed `mailpiler` version to 1.3.11
- changed `element-web` version to 1.7.25
- `LXC_AUTHORIZED_KEY` variable now defines an `authorized_keys` file, by default the configuration of you proxmox host will be inherited (`~/.ssh/authorized_keys`)
