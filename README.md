systools but fixed
========

fork of neko-systools ( https://code.google.com/p/neko-systools ) for Haxe 4 and above


### Status ###
The files are reupdated and are _mostly working_ for all platforms - which means that it should be working as well as normal systools.

### Neko usage with OpenFL ###
OpenFL will not include **systools.ndll** by default when building for the Neko or cpp platforms. To solve this you must include an additional line in your `project.xml` file, just after the `<haxelib name="systools" />` tag:
```xml
<ndll name="systools" haxelib="systools" />
```
