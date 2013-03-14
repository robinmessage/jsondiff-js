# jsondiff.js

Library to generate JSON Patches in JavaScript, from two differing json obejcts.

See also:
* http://tools.ietf.org/html/draft-ietf-appsawg-json-patch-08
* https://github.com/bruth/jsonpatch-js

Original code written by Byron Ruth here:
* https://gist.github.com/bruth/4715999

jsondiff.js works as in the browser as a script, as a Node module and as an
AMD module.

## Install

**Bower**

```
bower install json-diff
```

**NPM**

```
npm install json-diff-patch
```

## Methods

**`jsonpatch.diff(obj1, obj2)`**

Generates a patch based on the differences bewtween obj1 and obj2 such that:

```
patch = jsondiff.diff(obj1, obj2);
jsonpatch.apply(obj1, patch);
//obj1 and obj2 will now be equal.
```
