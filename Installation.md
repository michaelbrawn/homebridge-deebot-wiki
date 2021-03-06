## 1. Install

### Homebridge UI & HOOBS

Simply go to the 'Plugins' page, search `homebridge-deebot` and click 'Install'.

### Manually

This will only work if you are using a platform which installs plugins globally.

```bash
sudo npm i homebridge-deebot -g
```

## 2. Configure

If you use the Homebridge UI or HOOBS then a configuration screen will appear after installing the plugin where you can enter your ECOVACS credentials. You can optionally use a `base64`-encoded version of your password.

See the [[Configuration]] page for JSON configuration templates and other optional settings if editing the configuration manually.

## 3. Restart

And voila your Deebot devices *should* be added to your Homebridge/HOOBS instance.