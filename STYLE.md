# Node.js Offset Fire Syntax Style Guide

1. Use lowerCamelCase for all variables and constants phrases. Separate logical expressions with periods.
2. Use #~objectKey.diminutive for all object key holding variables and constants.
3. Use fn, global and module objects to scope all variables and constants and easily prevent memory-leak issues from creeping in.
4. Use NAMESPACE.lib.ClassName as a prefix for all variables and constants in the global and module namespaces.
5. Double-space all lines.
6. Use one of the pre-approved comment prefixes to make your code readable. Add clarity with appended terse English sentence(s).
   - // A-Z VARIABLES.
   - // A-Z VARIABLES. Dependent.
   - // ERROR? !@#$.
   - // INTERSECTION.
   - // LOGIC.
   - // TRAFFIC COP.

```
// LOGIC. System interface. License.

global[ "HWAJS.lib.System.boot.license" ] = function ( ) {

  // A-Z VARIABLES.

  let fn = new Object ( );

  // ERROR? !@#$. License missing.

  if ( global[ "HWAJS.lib.System.constant.settings.license" ] !== "tm" ) {

    global[ "HWAJS.lib.System.log" ] ( "// BOOT. ERROR? !@#$. License missing." );

    process.exit ( );

  }

  global[ "HWAJS.lib.System.log" ] ( "// BOOT. System license applied." );

}
```
