# munin plugin for omreport

## Plugins
- `omreport_`: Get machine information by using `omreport chassis` command.
- `omreport_storage_enclosure_`: Get storage enclosures information by using
  `omreport storage enclosure` command.

## Install
Recommendation: Fill `OMREPORT_PATH` in `omreport_` and `omreport_storage_enclosure_`.

1. Put `omreport_` and/or `omreport_storage_enclosure_` to `/usr/share/munin/plugins/`
2. Make symlinks in `/etc/munin/plugins/`. Supported functions are:
 * omreport_
    * omreport_watt
    * omreport_current
    * omreport_temps
    * omreport_volts
 * omreport_storage_enclosure_
    * omreport_storage_enclosure_temps
    * omreport_storage_enclosure_fans
3. Test with `munin-run` and restart your munin-node.
