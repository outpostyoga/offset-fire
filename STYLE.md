# Node.js Offset Fire Syntax Style Guide

1. Use lowerCamelCase for all variables and constants phrases. Separate logical expressions with periods.
2. Use #~objectKey.diminutive for all object key holding variables and constants.
3. Use fn, global and module objects to scope all variables and constants and easily prevent memory-leak issues from creeping in.
4. Use NAMESPACE.lib.ClassName as a prefix for all variables and constants in the global and module namespaces.
5. Double-space all lines. Indent using two-spaces.
   * Exempt nested callback functions. Indent a nested callback funtion two-spaces immediately underneath the open function call.
7. Use one of the pre-approved comment prefixes to make your code readable. Add clarity with appended terse English sentence(s).
   - // A-Z VARIABLES.
   - // A-Z VARIABLES. Dependent.
   - // BOOT..
   - // ERROR? !@#$.
   - // INTERSECTION.
   - // LOGIC.
   - // RESEARCH. https://wikipedia.org
   - // TRAFFIC COP.
8. Space-seperate all syntax except array and object accessors like [ ] and .
9. Use strict equality evaluations (x === y) for all expressions.
   * Exempt x == undefined in order to support JSON import (which turns undefined into null).
10. Prioritize readability over assembly level performance improvements.
11. Use Flatpacked objects for everything possible. Use "{}." and "[]." for non-compliant variables.

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
