### Required Configuration
Add the following to your Homebridge configuration file in the appropriate place. These following are the basic required fields.
```json
{
   "platform": "Deebot",
   "name": "Deebot",
   "username": "your-ecovacs-username",
   "password": "your-ecovacs-password",
   "countryCode": "your-ecovacs-country-code"
}
```
> Please note the `"platform" : "Deebot",` line **must not** be changed.

> `countryCode` must be one of `AU`, `BE`, `CH`, `CN`, `DE`, `DK`, `ES`, `FR`, `HK`,`IN`, `IT`, `JP`, `KR`, `MX`, `MY`, `NL`, `NO`, `PT`, `SE`, `SG`, `TH`, `TW`,`UK`, `US`, `OTHER`
### Additional Configuration
All of these settings are optional - just pick and choose the ones you require.

The following entries are also available to configure through the `homebridge-config-ui-x` plugin settings interface.
<table>
<thead>
<th>Entry</th>
<th>Type</th>
<th>Default</th>
<th>Explanation</th>
</thead>
<tr>
<td><code>debug</code></td>
<td align="center"><code>bool</code></td>
<td align="center"><code>false</code></td>
<td>If set to <code>true</code> then more information will be added to the Homebridge log.</td>
</tr>
<tr>
<td><code>hideBattHumidity</code></td>
<td align="center"><code>bool</code></td>
<td align="center"><code>false</code></td>
<td>If set to <code>true</code> then the humidity sensor showing the battery percentage will be hidden.</td>
</tr>
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
<td>The battery percentage at which Homebridge should display a low battery status.</td>
</tr>
<tr>
<td><code>motionDuration</code></td>
<td align="center"><code>integer</code></td>
<td align="center"><code>30</code></td>
<td>The length of time (in seconds) that the motion detector in Homebridge will be activated if your Deebot sends a message or needs help. The message sent is viewable in the Homebridge logs.</td>
</tr>
</table>