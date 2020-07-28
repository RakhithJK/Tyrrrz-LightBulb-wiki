### LightBulb isn't launching

LightBulb requires .NET Core runtime to work. Please download .NET Core Desktop Runtime from [the official website](https://dotnet.microsoft.com/download/dotnet-core/3.1/runtime). If you're having trouble installing, please check out [this step-by-step guide](https://github.com/Tyrrrz/LightBulb/wiki/How-to-install-.NET-Core-runtime).

If you're on a 32-bit version of Windows, launch LightBulb by going to its directory and running `dotnet LightBulb.dll` instead of running `LightBulb.exe`.

### LightBulb isn't launching (despite .NET Core Runtime being correctly installed)

- Make sure you have [Microsoft Visual C++ 2015 Redistributable installed](https://www.microsoft.com/download/details.aspx?id=52685).
- If running on Windows 7, make sure **KB2533623 update is installed**. Either install Windows updates or manually download KB2533623 ([x64](https://www.microsoft.com/en-ie/download/details.aspx?id=26764), [x86](https://www.microsoft.com/en-us/download/details.aspx?id=26767)). More info [here](https://github.com/Tyrrrz/LightBulb/pull/105#issuecomment-565435593).

[Full list of prerequisites](https://docs.microsoft.com/en-us/dotnet/core/install/dependencies?pivots=os-windows&tabs=netcore31).

### Gamma is not changing

You may experience that, despite LightBulb being enabled, the screen color doesn't change in any way.

- **Make sure latest Windows updates are installed**.
- **Update GPU drivers**.
- Monitors connected via **DisplayLink** don't allow changing gamma by default. Refer to [this post](https://support.displaylink.com/knowledgebase/articles/1886413-how-to-enable-night-light-or-f-lux-on-displaylink) to enable this feature.
- If you've installed **TeamViewer** you may have also installed its own display driver which doesn't support changing gamma. You will have to uninstall the driver (no need to uninstall the software). More info [here](https://github.com/Tyrrrz/LightBulb/issues/100#issuecomment-554009433).
- Disable **integrated GPU** in BIOS if you're using a discrete GPU as it may cause interference. More info [here](https://github.com/Tyrrrz/LightBulb/issues/130#issuecomment-565752598).

### Cursor is not affected by gamma changes

When hardware cursor rendering is enabled, your mouse pointer is rendered by GPU on a separate layer, thus preventing it from being affected by LightBulb.

In some cases, you should be able to disabled hardware cursor rendering in GPU settings. Otherwise, a common workaround is to change your cursor to a darker/black color scheme.

Another workaround is to enable cursor trail, as explained [here](https://github.com/Tyrrrz/LightBulb/issues/157#issuecomment-647428692).

### Gamma conflicts with other applications

Some applications may also try to override gamma settings, especially games. In cases where both the application and LightBulb are regularly refreshing gamma, the screen may either flicker or changes by one of the sides may not be seen. Most of the time, you can disable changing gamma in other applications so they don't interfere.

### Can't set a hotkey

If a hotkey is already registered by another application, you will not be able to use in LightBulb. If you try to assign a hotkey which is already in use, LightBulb will not even know it was pressed at all.

Refer to [this issue](https://github.com/Tyrrrz/LightBulb/issues/149#issuecomment-620044640) for more info.
