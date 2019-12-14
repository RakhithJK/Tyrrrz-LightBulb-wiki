### LightBulb isn't launching

LightBulb requires .NET Core runtime to work. Please download .NET Core Desktop Runtime from [the official website](https://dotnet.microsoft.com/download/dotnet-core/3.1/runtime). If you're having trouble installing, please check out [this step-by-step guide](https://github.com/Tyrrrz/LightBulb/wiki/How-to-install-.NET-Core-runtime).

### LightBulb isn't launching (despite .NET Core Runtime being correctly installed)

- If running on Windows 7, make sure **KB2533623 update is installed**. Either install Windows updates or manually download KB2533623 ([x64](https://www.microsoft.com/en-ie/download/details.aspx?id=26764), [x86](https://www.microsoft.com/en-us/download/details.aspx?id=26767)). More info [here](https://github.com/Tyrrrz/LightBulb/pull/105#issuecomment-565435593).

### Gamma is not changing

You may experience that, despite LightBulb being enabled, the screen color doesn't change in any way.

- **Make sure latest Windows updates are installed**.
- **Update GPU drivers**.
- Monitors connected via **DisplayLink** don't allow changing gamma by default. Refer to [this post](https://support.displaylink.com/knowledgebase/articles/1886413-how-to-enable-night-light-or-f-lux-on-displaylink) to enable this feature.
- If you've installed **TeamViewer** you may have also installed its own display driver which doesn't support changing gamma. You will have to uninstall the driver (no need to uninstall the software). More info [here](https://github.com/Tyrrrz/LightBulb/issues/100#issuecomment-554009433).
- Disable **integrated GPU** in BIOS if you're using a discrete GPU as it may cause interference. More info [here](https://github.com/Tyrrrz/LightBulb/issues/130#issuecomment-565752598).

### Cursor is not affected by gamma changes

When hardware cursor rendering is enabled, your mouse pointer is rendered by GPU on a separate layer, thus preventing it from being affected by LightBulb.

### Gamma conflicts with other applications

Some applications may also try to override gamma settings, especially games. In cases where both the application and LightBulb are regularly refreshing gamma, the screen may either flicker or changes by one of the sides may not be seen. Most of the time, you can disable changing gamma in other applications so they don't interfere.