systools but fixed
========

Yes i think im reviving an old lib\n
fork of giuppe/systools for Haxe 4 and above\n
This should be fixed without any compiler issues now, if so then please open an issue in Github Issues.
This includes the stdio definitions fix and the uncalled fix.

### Status ###
The files are reupdated and are _mostly working_ for all platforms - which means that it should be working as well as normal systools.

### Neko usage with OpenFL ###
OpenFL will not include **systools.ndll** by default when building for the Neko or cpp platforms. To solve this you must include an additional line in your `project.xml` file, just after the `<haxelib name="systools" />` tag:
```xml
<ndll name="systools" haxelib="systools" />
```
