# easyMeasure.activate()

|                      | &nbsp; 
| -------------------- | ---------------------------------------------------------------
| __Type__             | [function](http://docs.coronalabs.com/api/type/Function.html)
| __Library__          | [easyMeasure.*](Readme.markdown)
| __Return value__     | None
| __See also__         | [easyMeasure.deactivate()](deactivate.markdown)


## Overview

This activates the Runtime key event listener that's used by the plugin to check for the trigger key being pressed. Note that the plugin is activated by default when you `require` it. You'd only ever have to call this function if you had previously deactivated the plugin by using [easyMeasure.deactivate()](deactivate.markdown)



## Syntax

	easyMeasure.activate( )


## Examples

``````lua
local easyMeasure = require 'plugin.easyMeasure' -- the plugin is activated by default. 

-- 2,032 lines of code later

easyMeasure.deactivate() -- this removes the plugin's Runtime listener

-- 5,421 lines later

easyMeasure.activate() -- this adds the plugin's Runtime listener back again


``````
