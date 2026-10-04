# Group Policy

Create safe lab policies such as screen lock, selected account/security settings, mapped drives, or desktop settings. Link the GPO to the intended OU and validate on CLIENT01.

```cmd
gpupdate /force
gpresult /r
```

Capture GPMC configuration and client validation.