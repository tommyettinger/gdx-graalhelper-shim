# gdx-graalhelper-shim
Fills in [gdx-graalhelper](https://github.com/Berstanio/gdx-graalhelper)'s annotations when it isn't available.

...That's it, that's all this does. It provides two annotations and doesn't do anything with
them. This allows projects to compile with those annotations in use even if Graal-related code
isn't being used or depended upon. The package for the two empty annotations is the same as the
package used by gdx-graalhelper, but the contents of the annotations are the same in that. So,
even if this package accidentally overwrites the two duplicate files in gdx-graalhelper, it 
should still work exactly the same.

This has one release currently, 1.2.1, and should release in lockstep with Berstanio's gdx-graalhelper.

## Install

In your core module's dependencies:

```groovy
implementation 'com.github.tommyettinger:gdx-graalhelper-shim:1.2.1'
```

## License
Apache License 2.0. For some reason. I guess because that's what gdx-graalhelper uses.