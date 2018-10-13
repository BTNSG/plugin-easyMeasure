# easyMeasure.deactivate()

|                      | &nbsp; 
| -------------------- | ---------------------------------------------------------------
| __Type__             | [function](http://docs.coronalabs.com/api/type/Function.html)
| __Library__          | [easyMeasure.*](Readme.markdown)
| __Return value__     | None
| __See also__         | [easyMeasure.activate()](deactivate.markdown), [easyMeasure.unRequire()](unRequire.markdown)


## Overview

This deactivates the Runtime event listener that's used by the plugin to check for the trigger key being pressed. The plugin is activated by default when you `require` it. But in case you don't plan to use it for a while, you could save some memory by _deactivating_ the plugin and [bringing it back to life](activate.markdown) later. 

If you want to free up even more memory, you can also [unrequire](unRequire.markdown) the entire plugin and re-require it when you need to use it again.

## Syntax

	easyMeasure.deactivate( )


## Examples

``````lua
local easyMeasure = require 'plugin.easyMeasure' -- the plugin is activated by default. 

-- 2,032 lines of code later

easyMeasure.deactivate() -- this removes the plugin's Runtime listener

-- 5,421 lines later

easyMeasure.activate() -- this adds the plugin's Runtime listener back again


``````
