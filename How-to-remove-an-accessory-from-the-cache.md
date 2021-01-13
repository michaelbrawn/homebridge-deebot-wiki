## Method 1 (Homebridge UI)

You can use the `Remove Single Cached Accessory` option within `Homebridge Settings` to remove an accessory from the cache.

![Manage Cached Accessories](https://user-images.githubusercontent.com/43026681/93014440-0e838580-f5a9-11ea-9764-31f5b139f3f7.png)

Once removed, Homebridge will automatically restart and the accessory should be re-added by the plugin (you can verify this through the logs)

## Method 2 (HOOBS)

If the above option isn't available or you use HOOBS you can use the `ignoredDevices` configuration option.

1. Open the plugin "Configuration" (HOOBS) or "Settings" (Homebridge UI) screen
2. Add the Device ID to the "Ignored Devices" settings entry
3. Click "Save Changes"
4. Restart Homebridge (HOOBS should automatically restart)
5. If you watch the logs during the restart, you should see a message that says something like:

```13/01/2021, 06:52:20 [plugin] [Device] has been removed from Homebridge.```

6. Once it has been removed, you should return to the configuration and remove the Device ID from the "Ignored Devices"
7. Click "Save Changes"
8. Restart Homebridge again (HOOBS should automatically restart)
9. The accessory should be re-added by the plugin (you can verify this through the logs)