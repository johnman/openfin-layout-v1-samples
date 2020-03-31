# Please note that you should use the new Platform API instead of Layouts V1

https://developers.openfin.co/docs/platform-api

Samples in this repo:

## disable-tabs 

This app launches our sample webpage and allows you to snap the windows together. It demonstrates how to turn off tabs (it should be off be default). Look at the services section of the config.

_Requirements_

A localhost file server of choice on port 5001
The OpenFin CLI

_Sample Usage_

```
npx http-server -p 5001 -c-1
openfin -l -c http://localhost:5001/disable-tabs/app.json
```

## disable-tabs-for-specific-windows 

This app launches our sample webpage and allows you to snap the windows together. It also enables tabbing support for window one and window two (you can drop one window on top of the header/top part of the other window to create a tab). It shows you the config you need to include to exclude windows from the tabbing process.

We give an example of an app and a window (by providing a pattern for the name you want to exclude. The name is the name given to the window when you launch it).

By looking at the script in index.html and the service configuration in disable-tabs-for-specific-windows/app.json you can see how it is done.

_Requirements_

A localhost file server of choice on port 5001
The OpenFin CLI

_Sample Usage_

```
npx http-server -p 5001 -c-1
openfin -l -c http://localhost:5001/disable-tabs-for-specific-windows/app.json
```

## sample.json

If you open this file in Visual Studio Code (or something similar) it should give you intellisense when you start modifying the file.

This is to give you an idea of the options that are available. This file can be considered an area to experiment where you can then copy and paste the contents (excluding the schema) into the config of the layouts service.