# easyMeasure.setKeyTrigger()

|                      | &nbsp; 
| -------------------- | ---------------------------------------------------------------
| __Type__             | [function](http://docs.coronalabs.com/api/type/Function.html)
| __Library__          | [easyMeasure.*](Readme.markdown)
| __Return value__     | None
| __Keywords__         | None



## Overview

The key 'c' is used as a default trigger key for _easyMeasure_. However, you can change this if you so wish using this method.

## Syntax

	easyMeasure.setKeyTrigger( keyName )

##### keyName <small>(required)</small>
_[keyName](https://docs.coronalabs.com/api/event/key/keyName.html)._ The string representing the key that will trigger easyMeasure on/off.

## Example

``````lua
local easyMeasure = require 'plugin.easyMeasure'

easyMeasure.setKeyTrigger('m')
``````
