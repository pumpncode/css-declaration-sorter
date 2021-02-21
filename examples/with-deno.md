# With Deno

```js
import postcss from 'https://deno.land/x/postcss/mod.js'
import cssDeclarationSorter from './main-deno.mjs';

const css = 'a { z-index: 0; border: 0; }';

postcss([cssDeclarationSorter])
  .process(css)
  .then(console.info);
```

