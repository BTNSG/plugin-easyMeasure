# easyMeasure.setKeyTrigger()

|                      | &nbsp; 
| -------------------- | ---------------------------------------------------------------
| __Type__             | [function](http://docs.coronalabs.com/api/type/Function.html)
| __Library__          | [easyMeasure.*](Readme.markdown)
| __Return value__     | None
| __Keywords__         | None



## Overview

_mouseHover_ works by cycling through all the child display objects of a particular group, checking to see if the cursor is hovering over any of them. We call this group the _scope_ of the _mouseHover_ plugin.

By default the scope is set to Corona's display [stage](https://docs.coronalabs.com/api/type/StageObject/index.html). However, if you only want to scan a specific display group's children for hover events and not the entire stage, you can change the scope by calling mouseHover.setScope() and passing it the specific display group.

## Syntax

	easyMeasure.setKeyTrigger( keyName )

##### keyName <small>(required)</small>
_[keyName](https://docs.coronalabs.com/api/event/key/keyName.html)._ The string representing the key that will trigger easyMeasure on/off.

## Example

``````lua
local easyMeasure = require 'plugin.easyMeasure'

easyMeasure.setKeyTrigger('m')
``````
