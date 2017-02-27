If you prefer to setup LightBulb without the installer, it's possible to do that since version 1.6.3.

Every release (after version 1.6.1) comes with an installer (e.g. `LightBulb_Install_1.6.3.exe`) and an archive of binaries (e.g. `LightBulb_BinariesOnly_1.6.3.zip`). In the archive you will find all the binaries required for LightBulb to work which you can copy to any directory of your choice.

Follow these steps to get a portable version of LightBulb working:

- Copy the binaries from archive to any directory
- Run `Manual_Gamma_Registry_Fix.reg` file as administrator. This makes required changes to the registry which unlocks the broader gamma modification range, which is essential for LightBulb. This step is not required if you've already done it previously.
- Restart your computer for changes to apply. Only necessary if you did anything in previous step.
- Run `LightBulb_Portable.dat` or use command line arguments `LightBulb.exe -portable`

_Note: .NET framework 4.5.2 is assumed to be installed_

_Note: if you are running portable LightBulb from a directory with admin-only write access, you have to run LightBulb as administrator_