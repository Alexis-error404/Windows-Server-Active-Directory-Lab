# DNS & DHCP

Configure AD-integrated DNS and a DHCP scope.

```cmd
ipconfig /all
nslookup DC01
ipconfig /release
ipconfig /renew
```

Confirm clients receive intended gateway/DNS options and resolve the domain. Capture DNS zone, DHCP scope/options, lease, and resolution tests.