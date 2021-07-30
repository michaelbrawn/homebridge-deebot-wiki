If you're feeling brave, I also have a beta version, often with new features or code changes that needs testing. There are different methods of updating, based on the platform that you are running Homebridge on, or if you are using HOOBS.

There is no need to uninstall your current version of the plugin for any of these platforms.

The current versions of the plugin are:

[![npm](https://img.shields.io/npm/v/homebridge-deebot/latest?label=latest)](https://www.npmjs.com/package/homebridge-deebot) [![npm](https://img.shields.io/npm/v/homebridge-deebot/beta?label=beta)](https://github.com/bwp91/homebridge-deebot/wiki/Beta-Version)  

### Homebridge (UI)

You can use the 'Install Previous Version' feature to install a beta version.

![Feature Icon](https://user-images.githubusercontent.com/43026681/109934132-11437580-7cc4-11eb-9e50-e504c8a754fc.png)

This icon can be used to select a version of the plugin to install. The latest beta version is usually at the top of the list.

### Homebridge (Docker)

If Homebridge is installed using Docker use the following commands.

To install the beta version:

```bash
docker exec <container-name> npm install homebridge-deebot@beta
```

To revert back to the latest stable version:

```bash
docker exec <container-name> npm install homebridge-deebot@latest
```

### Homebridge (CLI)

These commands will only work if you are using a platform which installs plugins globally.

To install the beta, run the following command in your Homebridge terminal. 

```bash
sudo npm install homebridge-deebot@beta -g
```

To revert back to the stable version, run the following command in your Homebridge terminal.

```bash
sudo npm install homebridge-deebot@latest -g
```

You will need to restart Homebridge each time you change the version of the plugin.

### HOOBS 4

1. Go to the plugin page in the HOOBS UI and click on the 'Versions' tab
2. In the 'Tags' section, click on the download icon next to the version with `beta` on the right hand side
3. The version number will not be correct but this will still download the latest beta version
4. The UI will prompt you to select a bridge for the installation, choose your existing Meross bridge
5. The bridge will automatically restart and you can verify the plugin version in the startup logs

## Feedback
If you experience an issue with the beta package then do create an issue on GitHub and mention that you are using the beta 😄.