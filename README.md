*Simple bash scripts to add/remove domains from pihole wildcard blacklist. (to be used with `crontab` for scheduled toggling)*  
___

* Requires `domains.txt` as a `\n` separated list of domains to block.
* `safeEnable` adds them to the pihole wildcard blocklist.
* `safeDisable` removes them from the pihole wildcard blocklist.

___

**NOTES**

* gravity db
  * https://docs.pi-hole.net/database/gravity/
  * located at `/etc/pihole/gravity.db`
  * remove all regex blacklisted items with `delete from domainlist where type=3`
* logging
  * located at `/var/log/pihole.log`
  * `pihole -l off` disbables logging and flushes logs
  * `pihole -a -l 0` enables logging with 100% visibility
