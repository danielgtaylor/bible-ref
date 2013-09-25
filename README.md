Bible Reference Utilities
=========================
Utilities for handling Bible references, such as normalizing book names. This project started as a component of the [BibViz Project](http://github.com/danielgtaylor/bibviz), an interactive visualization of [Bible contradictions](http://bibviz.com/), violence, and misogyny in the Bible. It was spun off as it might be useful to others.

Usage
-----
Install the library via NPM:

```bash
npm install bible-ref
```

Then, once installed you can `require` and use it:

```javascript
var bref = require('bible-ref');

console.log(bref.bookNames);

console.log(bref.bookNormalize('1CO 1:1-4'));
```

Reference
---------

### bookNames
A list of book names in the Bible, e.g. `['Genesis', 'Exodus', ...]`.

### bookNormalize(ref)
Normalize the book name in a Bible reference.

```javascript
bref.bookNormalize('1CO')
>>> '1 Corinthians'

bref.bookNormalize('1CO 2:1')
>>> '1 Corinthians 2:1'

bref.bookNormalize('1 Corinthians 2:1')
>>> '1 Corinthians 2:1'
```

License
-------
This work is copyright 2013 Daniel G. Taylor and licensed under an MIT-style license.
