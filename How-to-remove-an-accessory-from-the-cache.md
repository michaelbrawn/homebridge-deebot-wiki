> Note this guide only applies to Homebridge users and also have Homebridge [installed as a service](https://github.com/oznu/homebridge-config-ui-x/wiki/Homebridge-Service-Command).

Removing an accessory from the cache is sometimes needed to take advantage of new features added to this plugin. If you remove an accessory from the cache it will simply be re-added again when Homebridge restarts.

This will, however, reset it's room designation in the Home app and it will remove the accessory from any automations it is currently in.

### 1. Go to `Homebridge Settings`
Click on the `⋮` in the top right hand corner and click on `Homebridge Settings`.

![Homebridge Settings](https://user-images.githubusercontent.com/43026681/93014435-ff043c80-f5a8-11ea-9431-ebe3e71a2206.png)
### 2. Go to `Manage Cached Accessories`
From the `Homebridge Settings` page, scroll down to the `Manage Cached Accessories` section. Click the box to open the `Remove Single Cached Accessory` option. If you don't see this section then you probably don't have Homebridge [installed as a service].(https://github.com/oznu/homebridge-config-ui-x/wiki/Homebridge-Service-Command)

![Manage Cached Accessories](https://user-images.githubusercontent.com/43026681/93014440-0e838580-f5a9-11ea-9764-31f5b139f3f7.png)
### 3. Remove the accessory
A list of your cached accessories will appear. Scroll to find the accessory you wish to remove from the cache and click the corresponding delete icon. After you click on the delete icon, the accessory will be removed and Homebridge will **automatically** restart. The accessory will then be re-added.

![Remove the Accessory](https://user-images.githubusercontent.com/43026681/93014455-1e02ce80-f5a9-11ea-844c-ba9de4d650eb.png)