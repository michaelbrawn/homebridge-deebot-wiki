Depending on your setup, Homebridge/HOOBS may or may not automatically remove the plugin's accessories from the cache when you uninstall the plugin. This plugin contains a useful configuration option to remove all your Deebot accessories from the cache.

These steps need to be completed **before** uninstalling the plugin.

If you have already uninstalled the plugin and found remaining accessories in your system, simply reinstall the plugin again and follow the steps below.

1. **Set the `disablePlugin` option to `true`. This setting can be found in the:**
    #### Homebridge UI

    <img alt="Screenshot 2021-02-10 at 11 39 19" src="https://user-images.githubusercontent.com/43026681/107505549-c5098780-6b94-11eb-969a-67b9ef8eb372.png">

    #### HOOBS UI
    <img alt="Screenshot 2021-02-10 at 11 38 10" src="https://user-images.githubusercontent.com/43026681/107505544-c2a72d80-6b94-11eb-875d-99ec26a8f4d5.png">

    or by editing your configuration file directly.

2. **Restart Homebridge/HOOBS**

    Once the system has restarted, you should find that the accessories no longer appear in the UI or in HomeKit applications.

3. **Uninstall the plugin as normal**

    Use the 'Uninstall' option in the Homebridge/HOOBS UI to remove the plugin.