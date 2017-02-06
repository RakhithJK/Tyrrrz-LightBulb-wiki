Although LightBulb is very customizable by itself, a portion of its settings is not exposed to users in GUI and those that are can be somewhat limited. The user interface controls aim to make it possible to customize LightBulb's behavior in an intuitive and straightforward manner. For advanced users that want to fine-tune their experience beyond what the GUI offers, it is recommended to edit the configuration file manually.

Please remember that changing the settings in such way can make the program run incorrectly. If you encounter a bug using custom settings make sure to mention it in the issue title or body. If at any point you will need to reset the settings to default - just exit LightBulb, delete the configuration file and launch LightBulb again.

### Location

Configuration file should be located in `%appdata%\LightBulb\Configuration.dat`. `%appdata%` variable can be expanded by most file explorers, so you can just paste the file path as is. If the configuration file is not there, it means that LightBulb hasn't created one yet. LightBulb saves settings to file every time it closes or when the system shuts down.

### Editing

Before you start editing the configuration file, you need to close LightBulb. Do that by right-clicking on the LightBulb's  tray icon and selecting "Exit".

When that's done, you can open the configuration file using any text editor. The file content is in JSON format, so an editor that's optimized for working with such files is more preferable.

![](https://i.imgur.com/aYqwKCE.png)


### Reloading settings

Once you are finished making your tweaks, make sure you save/overwrite the configuration file and then launch LightBulb. If you find your configuration reset to default, it means that LightBulb couldn't load or read the file and fell back to default values.