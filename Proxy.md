If you're using proxy to connect to the internet, there is a chance LightBulb's geolocation services (and other parts requiring an internet connection) may not work. There are a couple of things you can do to deal with that.

- **_(Recommended)_ Configure Windows Internet Options to use the correct proxy server.**

LightBulb will try to retrieve proxy settings used within Windows. To make sure they are set correctly, go to Internet Options (Start->type "Internet Options"->Enter) then navigate to the "Connections" tab and press the "LAN settings" button. The "Use proxy server..." checkbox should be checked and Address and Port should be set to correct values.

Windows will use your default credentials when connecting to a proxy server and you cannot set custom credentials using this method. Typically this problem is circumvented by creating an intermediate credential-less proxy server.

- **Use Proxy override in Configuration.dat**

[Manually edit the configuration file](https://github.com/Tyrrrz/LightBulb/wiki/Config-file) and change the `Proxy` property.

````json
"Proxy": {
    "Host": "proxy.server.com",
    "Port": 1337,
    "Username": "john.doe",
    "Password": "password.in.plain.text.yo"
}
````

Setting `Username` and `Password` is optional. If the `Host` property is not set, LightBulb will forcefully ignore all proxy settings, even those set in Internet Options.