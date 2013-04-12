Phonegap Toast plugin
===============================
By Pierre-Yves Orban

This Android Phonegap plugin allows you to show Toast in your application. You can show Toast with a short, long or custom duration.

This plugin was successfully tested with Phonegap 2.5 and Android 4.2.2 (on a Samsung Galaxy Nexus device).

## Adding this plugin to your project ##
0. (Make sure you are using Phonegap > 2.0)
1. Move ToastPlugin.js to your project's www folder and include a reference to it in your html files. 
2. Add the java file from src to your project's src hierarchy
3. Reference the plugin in your res/config.xml file
```<plugin name="ToastPlugin" value="org.apache.cordova.plugin.ToastPlugin"/>```

## Using the plugin ##
To instantiate the plugin object:
```javascript
var toastPlugin = cordova.require('cordova/plugin/toastplugin');
```

### show ###
Show a Toast with a custom duration (in the example: 500 ms).

Example:
```javascript
  toastPlugin.show ("Hello World", 500, function() {
    // toast correctly displayed
  }, function() {
    // an error occured
  });
```

### shortshow ###
Show a Toast with a short duration.

Example:
```javascript
  toastPlugin.shortshow ("Hello World", function() {
    // toast correctly displayed
  }, function() {
    // an error occured
  });
```

### longshow ###
Show a Toast with a long duration.

Example:
```javascript
  toastPlugin.longshow ("Hello World", function() {
    // toast correctly displayed
  }, function() {
    // an error occured
  });
```
  
## Licence ##

The MIT License

Copyright (c) 2013 Pierre-Yves Orban

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in
all copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN
THE SOFTWARE.
