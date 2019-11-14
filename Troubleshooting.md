### LightBulb isn't launching

LightBulb requires .NET Core runtime to work. Please download both the .NET Core Runtime and .NET Core Desktop Runtime from [here](https://dotnet.microsoft.com/download/dotnet-core/3.0/runtime) (you need both .NET Core Runtime and .NET Core Desktop Runtime).

### Nothing is happening

You may experience that, despite LightBulb being enabled, the screen color doesn't change in any way. This could happen due to several reasons:

- **Outdated drivers**. Make sure you're using the latest version of drivers available for your GPU.
- **DisplayLink**. Monitors connected via DisplayLink dock don't allow changing gamma by default. Refer to [this post](https://support.displaylink.com/knowledgebase/articles/1886413-how-to-enable-night-light-or-f-lux-on-displaylink) for a workaround.
- **TeamViewer**. When installing TeamViewer, you can opt in to install its display driver that allows drawing on the screen. This driver doesn't allow changing gamma so in order to have LightBulb working you will need to uninstall it. More info [here](https://github.com/Tyrrrz/LightBulb/issues/100#issuecomment-554009433).

### Cursor is not affected by gamma changes

When hardware cursor rendering is enabled, your mouse pointer is rendered by GPU on a separate layer, thus preventing it from being affected by LightBulb.

### Gamma conflicts with other applications

Some applications may also try to override gamma settings, especially games. In cases where both the application and LightBulb are regularly refreshing gamma, the screen may either flicker or changes by one of the sides may not be seen. Most of the time, you can disable changing gamma in other applications so they don't interfere.