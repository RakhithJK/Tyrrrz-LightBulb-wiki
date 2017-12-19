Users who don't directly connect to the internet, such as those behind proxies or VPN, will have their location identified incorrectly. If you are one of those users or for any other purpose decided to set your location manually, please refer to these instructions on how to do it.

The following steps will involve manual editing of the configuration file. For more information on that [read this](https://github.com/Tyrrrz/LightBulb/wiki/Config-file).

- Close LightBulb if it's currently opened
- Locate and open the configuration file \*
- Look for `GeoInfo` property
- Change `Country`, `CountryCode`, `City`, `Latitude`, `Longitude` as necessary \**
- Look for `IsGeoInfoLocked` property
- Set it to `true` instead of `false`
- Save file
- Launch LightBulb
- LightBulb will use stored geolocation settings and will not overwrite them

\* - if the file doesn't exist, LightBulb probably hasn't been launched before

\** - of all those, only `Latitude` and `Longitude` are actually necessary, the rest are for visuals