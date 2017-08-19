# vgen-xbox
Node wrapper for vGenInterface (xbox) to feed xinput events to Windows

# Example
```js
const VGen = require("vgen-xbox")
const vgen = new VGen();

var controllerId = vgen.pluginNext() // Plugs in next available controller
vgen.setDpad(controllerId, vgen.Dpad.UP); // Set dpad to point up
vgen.setButton(controllerId, vgen.Buttons.B, true); // Press B button
vgen.setButton(controllerId, vgen.Buttons.B, false); // Release B button

vgen.unplug(controllerId); // Unplug controller
```
Full example available in [demo.js](https://github.com/Jeflux/vgen-xbox/blob/master/demo.js)


# Installation
Make sure you have the build tools for [node-ffi](https://github.com/node-ffi/node-ffi#installation). Then install with:
``` bash
$ npm install vgen-xbox
```
