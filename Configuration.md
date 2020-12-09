### Required Settings
Add the following to your Homebridge configuration file in the appropriate place. These following are the basic required fields.
```json
{
   "countryCode": "your-ecovacs-country-code",
   "name": "Deebot",
   "username": "your-ecovacs-username",
   "password": "your-ecovacs-password",
   "platform": "Deebot"
}
```
> Please note the `"platform": "Deebot"` line **must not** be changed.

> `countryCode` must be one of `AU`, `BE`, `CH`, `CN`, `DE`, `DK`, `ES`, `FR`, `HK`,`IN`, `IT`, `JP`, `KR`, `MX`, `MY`, `NL`, `NO`, `PT`, `SE`, `SG`, `TH`, `TW`,`UK`, `US`, `OTHER`
### Optional Settings
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
<td>An interval (in seconds) in which your devices will refresh with ECOVACS.</td>
</tr>
<tr>
<td><code>lowBattThreshold</code></td>
<td align="center"><code>integer</code></td>
<td align="center"><code>20</code></td>
<td>The battery percentage at which the plugin should display a low battery status.</td>
</tr>
<tr>
<td><code>motionDuration</code></td>
<td align="center"><code>integer</code></td>
<td align="center"><code>30</code></td>
<td>The length of time (in seconds) that the motion detector will be activated if your Deebot sends a message or needs help. The message is viewable in the log.</td>
</tr>
<tr>
<td><code>hideBattHumidity</code></td>
<td align="center"><code>bool</code></td>
<td align="center"><code>false</code></td>
<td>If <code>true</code>, the humidity sensor showing the battery percentage will be hidden.</td>
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
</table>