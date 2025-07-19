# custom-caddy

Github workflow building a custom caddy binary. Runs every day and builds+publishes a new binary if caddy received a new update.

To use as your own, populate `CADDY_PLUGINS.txt` as follows (replace with your plugins).

``` bash
$ cat CADDY_PLUGINS.txt
github.com/caddy-dns/cloudflare
github.com/hslatman/caddy-crowdsec-bouncer/http
```
