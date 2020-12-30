# JDownloader
This plugin provides a convenient way to install JDownloader in a FreeBSD jail using the [iocage](https://github.com/iocage/iocage) jail manager.

JDownloader is a free, open-source download management tool.
For more info on this project, see https://jdownloader.org/

## To install this Plugin
Download the plugin manifest file to your local file system.
```
fetch https://raw.githubusercontent.com/jsegaert/iocage-my-plugins/master/jdownloader.json
```
Install the plugin.  Adjust the network settings as needed.
```
iocage fetch -P jdownloader.json -n jdownloader vnet=1 nat=1
```
## Post-installation steps

 - register for a free account at https://my.jdownloader.org
 - run the following command inside the jail to link to your account to the plugin: `jdownloaderinit <email> <password>`
