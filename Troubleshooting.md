### LightBulb isn't launching

LightBulb requires .NET Core runtime to work. Please download .NET Core Desktop Runtime from [the official website](https://dotnet.microsoft.com/download/dotnet-core/3.1/runtime). If you're having trouble installing, please check out [this step-by-step guide](https://github.com/Tyrrrz/LightBulb/wiki/How-to-install-.NET-Core-runtime).

If despite installing .NET Core runtime, LightBulb still doesn't run, here are the possible solutions:

- Windows 7 **KB2533623** update is missing. Running `dotnet` in console shows an error regarding `hostfxr.dll`. To fix that, install Windows updates or manually download KB2533623 ([x64](https://www.microsoft.com/en-ie/download/details.aspx?id=26764), [x86](https://www.microsoft.com/en-us/download/details.aspx?id=26767)). More info [here](https://github.com/Tyrrrz/LightBulb/pull/105#issuecomment-565435593).

### Nothing is happening

You may experience that, despite LightBulb being enabled, the screen color doesn't change in any way. This could happen due to several reasons:

- **Outdated drivers**. Make sure you're using the latest version of drivers available for your GPU.
- **DisplayLink**. Monitors connected via DisplayLink dock don't allow changing gamma by default. Refer to [this post](https://support.displaylink.com/knowledgebase/articles/1886413-how-to-enable-night-light-or-f-lux-on-displaylink) for a workaround.
- **TeamViewer**. When installing TeamViewer, you can opt in to install its display driver that allows drawing on the screen. This driver doesn't allow changing gamma so in order to have LightBulb working you will need to uninstall it. More info [here](https://github.com/Tyrrrz/LightBulb/issues/100#issuecomment-554009433).

### Cursor is not affected by gamma changes

When hardware cursor rendering is enabled, your mouse pointer is rendered by GPU on a separate layer, thus preventing it from being affected by LightBulb.

### Gamma conflicts with other applications

Some applications may also try to override gamma settings, especially games. In cases where both the application and LightBulb are regularly refreshing gamma, the screen may either flicker or changes by one of the sides may not be seen. Most of the time, you can disable changing gamma in other applications so they don't interfere.