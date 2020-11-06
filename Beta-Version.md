If you're feeling brave, I also have a beta version, often with new features or code changes that needs testing. There are different methods of updating, based on the platform that you are running Homebridge on, or if you are using HOOBS.

There is no need to uninstall your current version of homebridge-deebot for any of these platforms.

### Homebridge UI (config-ui-x)

You can use the `Install Previous Version` feature to install a beta version.

![Feature Icon](https://user-images.githubusercontent.com/43026681/98367572-beb3be80-202d-11eb-8e5b-f4beaba2c42d.png)

This icon can be used to select a version of the plugin to install. The latest beta version is usually at the top of the list.

### Homebridge CLI

> These commands will only work if you are using a platform which installs plugins globally.

To install the beta, run the following command in your Homebridge terminal. 

```bash
sudo npm install homebridge-deebot@beta -g
```

To revert back to the stable version, run the following command in your Homebridge terminal.

```bash
sudo npm install homebridge-deebot@latest -g
```

### HOOBS

Coming soon.

### Further Updates

A limitation of the beta version is that further beta updates are not displayed. To update to the latest beta (or check if an update is available) simply use the same command as above to install the beta. An update will display in Homebridge/HOOBS once the beta has been released as the stable version.

### Feedback
If you experience an issue with the beta package then please create an issue on GitHub and mention that you are using the beta 😄.