# custom-caddy

Github workflow building a custom caddy binary. Runs every day and builds+publishes a new binary if caddy received a new update.

To use as your own, populate `CADDY_PLUGINS.txt` as follows (replace with your plugins).

``` bash
$ cat CADDY_PLUGINS.txt
github.com/caddy-dns/cloudflare
github.com/hslatman/caddy-crowdsec-bouncer/http
```
## rationale 

`caddy upgrade` is unreliable and might be removed in the future. This offers a replacement without having to build locally
```
$ wget -q https://github.com/HamletDuFromage/custom-caddy/releases/latest/download/caddy-custom
```
