### General settings

![](http://tyrrrz.me/Projects/LightBulb/1.png)

- **Day-time color temperature**

Default: 6600K

Config file property name: `MaxTemperature`

Description: This is the color temperature of your screen during day-time. Day-time is the timespan between sunrise and sunset, which is typically when the sun is the primary light source and indoor lights are turned off.

- **Night-time color temperature**

Default: 3900K

Config file property name: `MinTemperature`

Description: This is the color temperature of your screen during night-time. Night-time is the timespan before sunrise and after sunset, which is typically when the sun is hidden and the indoor lights are the primary light source.

- **Transition duration**

Default: 01:30:00

Config file property name: `TemperatureTransitionDuration`

Description: This is the duration of time during which the color temperature switches from day-time to night-time or vice versa. This event occurs twice a day - at sunrise and at sunset. Setting this to 0 (zero) will make the transition instant.

### Geolocation settings

![](http://tyrrrz.me/Projects/LightBulb/2.png)

- **Sunrise time**

Default: 07:20:00

Config file property name: `SunriseTime`

Description: The time at which the sun rises. If "Internet synchronization" is enabled, this value is ignored and overwritten.

- **Sunset time**

Default: 16:30:00

Config file property name: `SunsetTime`

Description: The time at which the sun sets. If "Internet synchronization" is enabled, this value is ignored and overwritten.

- **Internet synchronization**

Default: enabled

Config file property name: `IsInternetTimeSyncEnabled`

Description: When enabled, LightBulb will pull sunrise and sunset times for your location automatically from the internet.

### Advanced settings

![](http://tyrrrz.me/Projects/LightBulb/3.png)

- **Gamma polling**

Default: enabled

Config file property name: `IsGammaPollingEnabled`

Description: When enabled, gamma is refreshed every couple of seconds to make sure it is not overriden by anything else.

- **Temperature smoothing**

Default: enabled

Config file property name: `IsTemperatureSmoothingEnabled`

Description: When enabled, temperature change is smoothed out when toggling LightBulb. This gives a bit of time for the eyes to adjust.

- **Pause when fullscreen**

Default: disabled

Config file property name: `IsFullscreenBlocking`

Description: When enabled, LightBulb's workflow will pause if a fullscreen application is currently in foreground.

- **LightBulb toggle hotkey**

Default: not set

Config file property name: `ToggleHotkey`

Description: Global hotkey to toggle LightBulb.

- **Polling toggle hotkey**

Default: not set

Config file property name: `TogglePollingHotkey`

Description: Global hotkey to toggle gamma polling.

- **Refresh gamma hotkey**

Default: not set

Config file property name: `RefreshGammaHotkey`

Description: Global hotkey to force refresh gamma on demand.