## Overview

*prettydump* is a Lua module for pretty printing Lua values, especially tables.  All data types are handled, though some write themselves out as comments (such as functions, userdata, and threads).

It is derived from former LuaPlus versions that had built-in pretty printing support.  Depending on setup, the *prettydump* goes to great lengths to not modify any of the internal Lua state.


## Example

<pre>
    local prettydump = require 'prettydump'

    local myTable = {
        Name = 'Joe',
        HitPoints = 100,
    }

    prettydump.dumpascii('output.lua', 'myTable', myTable)
</pre>



