*Simple bash scripts to add/remove domains from pihole wildcard blacklist. (to be used with `crontab` for scheduled toggling)*  
___

* Requires `domains.txt` as a `\n` separated list of domains to block.
* `safeEnable` adds them to the pihole wildcard blocklist.
* `safeDisable` removes them from the pihole wildcard blocklist.
