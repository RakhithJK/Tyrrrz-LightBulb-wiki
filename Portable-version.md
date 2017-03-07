If you prefer to setup LightBulb without an installer, it is possible to do so.

Every [release](https://github.com/Tyrrrz/LightBulb/releases) (after version 1.6.1) comes with an installer (e.g. `LightBulb_Install_1.6.1.exe`) and an archive of binaries (e.g. `LightBulb_Portable_1.6.1.zip`). In the latter you will find all the binaries required for LightBulb to work, which you can copy to any directory of your choice.

If you are updating LightBulb from a previous version, you only need need to replace old files. If you never had LightBulb installed before, you need to perform some extra steps.

Follow these steps to deploy a portable version of LightBulb for the first time:

- Extract the binaries from archive to any directory
- Run `Manual_Gamma_Registry_Fix.reg` file as administrator. This makes required changes to the registry, unlocking a broader gamma modification range, which is essential for LightBulb.
- Restart computer.

To run LightBulb in portable mode either launch the `LightBulb_Portable.bat` file or append the command line switch manually: `LightBulb.exe -portable`.

_Note: .NET framework 4.5.2 is assumed to be installed_

_Note: if you are running portable LightBulb from a directory with admin-only write access, you have to run LightBulb as administrator_