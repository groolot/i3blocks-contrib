# `my-external-ip`

Display the external IP address returned by an external IP provider,
such as [ip.yunohost.org](http://ip.yunohost.org) or
[ipv4.icanhazeip.com](http://ipv4.icanhazeip.com).

Offers clipboarding with middle mouse button click on the block, even
in short display.

![](my-external-ip-long.png)
![](my-external-ip-short.png)

# Dependencies

- `wget` or `curl` for HTTP request,
- `xclip` for clipboarding.

# Config
## Output with pango markup available
```INI
[my-external-ip]
command=$SCRIPT_DIR/my-external-ip
markup=pango
interval=60
color=#aaffaa
# external_ip_provider=ip.yunohost.org
```

## Classic output
```INI
[my-external-ip]
command=$SCRIPT_DIR/my-external-ip
interval=60
color=#aaffaa
# external_ip_provider=ipv4.icanhazeip.com
```
