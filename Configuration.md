## Required Settings
Add the following to your configuration file in the appropriate place. The following are the basic required fields.
```json
{
   "name": "Deebot",
   "countryCode": "your-ecovacs-country-code",
   "username": "your-ecovacs-username",
   "password": "your-ecovacs-password",
   "platform": "Deebot"
}
```

* ⚠️ The `"platform": "Deebot"` line **must not** be changed
* You can optionally use a `base64`-encoded version of your password
* See [[Country Codes]] for a list of allowed country codes
* If your account is based in China you should use your ECOVACS ID for your username

## Optional Settings

⚠️ It is easier to use the Homebridge/HOOBS UI to configure these settings

<table>
<thead>
<th>Entry</th>
<th>Type</th>
<th>Default</th>
<th>Explanation</th>
</thead>
<tr>
<td><code>refreshTime</code></td>
<td align="center"><code>integer</code></td>
<td align="center"><code>120</code></td>
<td>An interval (in seconds) in which your devices will refresh with ECOVACS. Must be <code>30</code> or more.</td>
</tr>
<tr>
<td><code>disableDeviceLogging</code></td>
<td align="center"><code>bool</code></td>
<td align="center"><code>false</code></td>
<td>Global logging setting for accessory status changes. If <code>true</code> then accessory status changes will not be logged. This can also be set per accessory later in the config.</td>
</tr>
<tr>
<td><code>debug</code></td>
<td align="center"><code>bool</code></td>
<td align="center"><code>false</code></td>
<td>Global logging setting for the plugin. If <code>true</code> then debug information will be added to the log. This can also be set per accessory later in the config.</td>
</tr>
<tr>
<td><code>disablePlugin</code></td>
<td align="center"><code>bool</code></td>
<td align="center"><code>false</code></td>
<td>If <code>true</code>, the plugin will remove all accessories and not load the plugin on restart.</td>
</tr>
<tr>
<td><code>devices</code></td>
<td align="center"><code>array</code></td>
<td align="center"><code>[]</code></td>
<td>

An array of objects to define custom options for your Deebot devices.
* `label` - This setting has no effect except to help identify this device
* `deviceId` - Deebot Device ID
* `ignoreDevice` - If <code>true</code>, this accessory will be removed and ignored from HomeKit
* `hideMotionSensor` - If <code>true</code>, the motion sensor for device alerts will be hidden
* `motionDuration` - The length of time (in seconds) that the motion detector will be activated if your Deebot sends a message or needs help. The message is viewable in the log. Must be <code>1</code> or more
* `lowBattThreshold` - The battery percentage at which the plugin should display a low battery status. Leave blank to match the Deebot default of 15%. Must be <code>1</code> or more
* `showMotionLowBatt` - If <code>true</code>, the motion sensor will activate when the Deebot's battery reaches the low battery threshold
* `showBattHumidity` - If <code>true</code>, a humidity sensor showing the battery percentage will be shown
* `overrideLogging` - Override global logging setting for this device. Can be `default` (follows global setting), `standard` for standard logging, `debug` for debug logging or `disable` to disable accessory logging

Example:

```json
"devices": [
   {
      "deviceId": "E2000000000000000000",
      "label": "Hoover Device",
      "hideMotionSensor": false,
      "motionDuration": 120,
      "lowBattThreshold": 20,
      "showMotionLowBatt": false,
      "showBattHumidity": true,
      "overrideLogging": "default"
   }
]
```

</td>
</tr>
</table>