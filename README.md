# munin plugin for omreport

## Install
Recommendation: fill `OMREPORT_PATH` in `omreport_`

1. put `omreport_` to `/usr/share/munin/plugins/`
2. make symlinks in `/etc/munin/plugins/`
 * omreport_watt
 * omreport_current
 * omreport_temps
 * omreport_volts
3. test with `munin-run` and restart your munin-node
