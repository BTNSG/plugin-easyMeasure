# easyMeasure: Plugin API Docs

|                      | &nbsp; 
| -------------------- | ---------------------------------------------------------------
| __Type__             | [Plugin](https://docs.coronalabs.com/plugin/)
| __Corona Store__     | [easyMeasure](http://store.coronalabs.com/plugin/easyMeasure)



## Overview

Hi there! Welcome to the documentation for [Easy Measure](http://store.coronalabs.com/plugin/easyMeasure). Easy Measure is a plugin for the [Corona](https://coronalabs.com/products/corona-sdk/) Simulator. 

Needing to repeatedly reload our Corona project to see if we'd coded our UI positions, sizes and angles correctly was a bit of a pain. So we made this plugin as a helper to measure and call out these values in Corona simulator via the mouse cursor and keyboard.


## Syntax
``````lua

	local easyMeasure = require "plugin.easyMeasure"

``````

### Functions

##### [easyMeasure.setTriggerKey()](setTriggerKey.markdown)

##### [easyMeasure.activate()](activate.markdown)

##### [easyMeasure.deactivate()](deactivate.markdown)

##### [easyMeasure.unRequire()](unRequire.markdown)



## Setting up

In order to use this plugin, you need to activate the plugin at the [Corona Store](http://store.coronalabs.com/plugin/easyMeasure).

Add the following entry into a `plugins` table of your `build.settings` like so:

``````
settings =
{
	plugins =
	{
		["plugin.easyMeasure"] =
		{
			-- required
			publisherId = "sg.btn",
		},
	},		
}
``````
Since the plugin is meant for use on the Simulator, remove the above entry from `build.settings` before building your app executable.

## How it works

1. `require` the plugin in the Simulator while developing your app. 
2. Hit 'c' on the keyboard and move the mouse around to call out positions (absolute and relative to screen size)
3. Click and drag on the screen with 'c' pressed to get the dimensions and the diagonal angle of the resulting rectangle.


## Gotchas

* This uses Corona's 'mouse' events. All the gotchas of mouse events apply. 

* This is meant as a Simulator helper. The plugin will deliberately NOT activate on device builds.


### Support

If you have any questions about Easy Measure, feel free to [drop us an email](mailto://info@btn.sg)


## Compatibility

| Platform                     | Supported
| ---------------------------- | ---------------------------- 
| Corona Simulator (Mac)       | YES
| Corona Simulator (Win)       | YES

