retools
========

___Systools, but fixed for newer versions.___

fork of giuppe/systools for Haxe 4 and above

This should be fixed without any compiler issues now, if so then please open an issue in Github Issues.

This includes the stdio definitions fix and the uncalled fix.

### Status ###
The files are reupdated and are _mostly working_ for all platforms - which means that it should be working as well as normal systools.
The files have been updated for newer Haxe versions. If it doesn't work, make a PR fixing the issue or put the issue in Github issues.

### How to use ###
Git this repo using `haxelib git systools https://github.com/haya3218/retools`.
Once you've done that, if youre using normal haxe add `-lib systools` to your project.
If youre using OpenFL on the other hand, see the instruction down below.

### Neko usage with OpenFL ###
OpenFL will not include **systools.ndll** by default when building for the Neko or cpp platforms. To solve this you must include an additional line in your `project.xml` file, just after the `<haxelib name="systools" />` tag:
```xml
<ndll name="systools" haxelib="systools" />
```
Then do `lime rebuild systools [system currently using]`
.
