# replaceAll-Shim
This will add the replaceAll method to the string prototype, so you can use it exactly as you would with ECMA-262 and all need to be done after support was added to your env is to remove the require at the top!


# Usage:

All you have to do is to `require` the package on the top of your file after you installed the package (`npm i replaceAll-Shim`),
```
require('replaceAll-Shim');
```

then you can use `replaceAll` method [as you would](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String/replaceAll) if ECMA-262 was supported in your environment as the method will be added to the String prototype:

```
'aabbcc'.replaceAll('b', '.');
// 'aa..cc'
```