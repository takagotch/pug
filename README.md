###### pug convert to html
---
https://pughtml.com/





---


### pug
---
https://github.com/pugjs/pug

```
npm install pug
npm install pug-cli -g
pug --help

pug --client --no-debug filename.pug
```

```
doctype html
html(lang="en")
  head
    title= pageTitle
    script(type='text/javascript').
      if (foo) bar(1 + 5)
  body
    h1 Pug - node template engine
    #container.col
      if youAreUsingPug
        p You are amazing
      else
       p Get on it!
     p.
       Pug is a terse and simple templating language with a
       strong focus on performance and powerful features.

```

```js
var pug = require('pug');
var fn = pug.compile(locals);
var html = fn(locals);
var html = pug.render('string of pug', merge(options, locals));
var html = pug.renderFile('filename.pug', merge(options, locals));


```

