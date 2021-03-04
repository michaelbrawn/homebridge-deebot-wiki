If you're feeling brave, I also have a beta version, often with new features or code changes that needs testing. There are different methods of updating, based on the platform that you are running Homebridge on, or if you are using HOOBS.

There is no need to uninstall your current version of the plugin for any of these platforms.

The current versions of the plugin are:

[![npm](https://img.shields.io/npm/v/homebridge-deebot/latest?label=latest)](https://www.npmjs.com/package/homebridge-deebot) [![npm](https://img.shields.io/npm/v/homebridge-deebot/beta?label=beta)](https://github.com/bwp91/homebridge-deebot/wiki/Beta-Version)  

## Homebridge UI

You can use the `Install Previous Version` feature to install a beta version.

![Feature Icon](https://user-images.githubusercontent.com/43026681/109934132-11437580-7cc4-11eb-9e50-e504c8a754fc.png)

This icon can be used to select a version of the plugin to install. The latest beta version is usually at the top of the list.

## Homebridge CLI

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

## HOOBS UI

⚠️ Make sure you have already used the HOOBS UI to install the plugin.

1. Stop the HOOBS service

2. Using the HOOBS terminal run these commands separately:

    ```bash
    cd ~/.hoobs/
    npm install homebridge-deebot@beta
    ```

3. Start HOOBS again

To revert back to the stable version, follow the steps above replacing the two commands with the two below.

```bash
cd ~/.hoobs/
npm install homebridge-deebot@latest
```

You will need to restart HOOBS each time you change the version of the plugin.

## Further Updates

A limitation of the beta version is that further beta updates are not displayed. To update to the latest beta (or check if an update is available) simply use the same command as above to install the beta. An update will display in Homebridge/HOOBS once the beta has been released as the stable version.

## Feedback
If you experience an issue with the beta package then please create an issue on GitHub and mention that you are using the beta 😄.