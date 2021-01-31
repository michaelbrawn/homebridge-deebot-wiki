## Required Settings
Add the following to your configuration file in the appropriate place. These following are the basic required fields.
```json
{
   "name": "Deebot",
   "countryCode": "your-ecovacs-country-code",
   "username": "your-ecovacs-username",
   "password": "your-ecovacs-password",
   "platform": "Deebot"
}
```
⚠️ The `"platform": "Deebot"` line **must not** be changed.

See [[Country Codes]] for a list of allowed country codes.

## Optional Settings

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
<td>An interval (in seconds) in which your devices will refresh with ECOVACS. Must be 30 or more.</td>
</tr>
<tr>
<td><code>disableDeviceLogging</code></td>
<td align="center"><code>bool</code></td>
<td align="center"><code>false</code></td>
<td>If <code>true</code>, device updates will not be added to the log.</td>
</tr>
<tr>
<td><code>debug</code></td>
<td align="center"><code>bool</code></td>
<td align="center"><code>false</code></td>
<td>If <code>true</code>, more information will be added to the log.</td>
</tr>
<tr>
<td><code>disablePlugin</code></td>
<td align="center"><code>bool</code></td>
<td align="center"><code>false</code></td>
<td>If <code>true</code>, the plugin will remove all accessories and not load the plugin on restart.</td>
</tr>
<tr>
<td><code>motionDuration</code></td>
<td align="center"><code>integer</code></td>
<td align="center"><code>30</code></td>
<td>The length of time (in seconds) that the motion detector will be activated if your Deebot sends a message or needs help. The message is viewable in the log. Must be 1 or more.</td>
</tr>
<tr>
<td><code>lowBattThreshold</code></td>
<td align="center"><code>integer</code></td>
<td align="center"><code>15</code></td>
<td>The battery percentage at which the plugin should display a low battery status. Leave blank to match the Deebot default of 15%. Must be 1 or more.</td>
</tr>
<tr>
<td><code>showMotionLowBatt</code></td>
<td align="center"><code>bool</code></td>
<td align="center"><code>false</code></td>
<td>If <code>true</code>, the motion sensor will activate when the Deebot's battery reaches the low battery threshold.</td>
</tr>
<tr>
<td><code>showBattHumidity</code></td>
<td align="center"><code>bool</code></td>
<td align="center"><code>false</code></td>
<td>If <code>true</code>, a humidity sensor showing the battery percentage will be shown.</td>
</tr>
<tr>
<td><code>ignoredDevices</code></td>
<td align="center"><code>array</code></td>
<td align="center"><code>[]</code></td>
<td>

A list of devices to ignore by Device ID. For example:

```json
[
   "E2000000000000000000"
]
```

</td>
</tr>
</table>