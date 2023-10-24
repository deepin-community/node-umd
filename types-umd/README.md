# Installation
> `npm install --save @types/umd`

# Summary
This package contains type definitions for umd (https://github.com/ForbesLindesay/umd).

# Details
Files were exported from https://github.com/DefinitelyTyped/DefinitelyTyped/tree/master/types/umd.
## [index.d.ts](https://github.com/DefinitelyTyped/DefinitelyTyped/tree/master/types/umd/index.d.ts)
````ts
// Type definitions for umd 3.0
// Project: https://github.com/ForbesLindesay/umd
// Definitions by: TeamworkGuy2 <https://github.com/TeamworkGuy2>
// Definitions: https://github.com/DefinitelyTyped/DefinitelyTyped

/** Universal Module Definition for use in automated build systems
 * - simple synchronous wrapping of a string
 * - return style module support
 * - CommonJS support
 * - prevents internal UMDs from conflicting
 */
declare function Umd(name: string, src: string, options?: boolean | Umd.Options): string;

declare namespace Umd {

    interface Options {
        commonJS?: boolean | undefined;
    }

    function prelude(moduleName: string, options?: boolean | Options): string;

    function postlude(moduleName: string, options?: boolean | Options): string;
}

export = Umd;

````

### Additional Details
 * Last updated: Fri, 02 Jul 2021 18:04:48 GMT
 * Dependencies: none
 * Global values: none

# Credits
These definitions were written by [TeamworkGuy2](https://github.com/TeamworkGuy2).
