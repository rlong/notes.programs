

Short Cuts
==========

Editing
-------


* `CTRL-K CTRL-C`: comment out selected block
* `CTRL-K CTRL-U`: uncomment out selected block
* `CTRL-R CTRL-R`: rename symbol

Navigation
----------

* `CTRL-F12`: Navigate into symbol (show options if ambiguous)
* `CTRL--`: Navigate back
* `CTRL-SHIFT--`: Navigate forward


Debugging
---------

* `F5`: continue
* `F9`: toggle breakpoint


Regions
-------

* `CTRL`-`M`-`L`: Expand all regions

Class View
==========

* `View` -> `Class View`

Synchronize Class View
----------------------

* [My Technical Blog: Synchronize Class View in Visual Studio 2010](http://techshangrila.blogspot.com.au/2014/05/synchronize-class-view-in-visual-studio.html)
* [.net - Visual Studio - Automatically refresh class view when changing class - Stack Overflow](http://stackoverflow.com/questions/546113/visual-studio-automatically-refresh-class-view-when-changing-class)



* `Tools` -> `Options` -> `Environment` -> `Keyboard`
* bind `Ctrl`+`Shift`+`C` to `View.SynchronizeClassView`

Shelvesets
==========

* Select the Shelve button in Pending Changes
* Give the shelveset a meaningful name
* You can choose to keep the changes locally via the check-box.
* Click on the shelve button


EDMX
====

generating result types for stored procedures (only use on read-only stored procedures):
```
SET FMTONLY OFF; -- http://stackoverflow.com/questions/7128747/ef4-the-selected-stored-procedure-returns-no-columns
```

