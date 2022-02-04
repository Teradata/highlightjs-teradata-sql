# highlightjs-teradata-sql
Highlight.js language definition for Teradata SQL.

For more about highlight.js, see https://highlightjs.org/.

For more about Teradata, see https://teradata.com/

## Usage

Include the `highlight.js` script in your webpage or node app, load up this module and apply it to `hljs`.

### Website
If you're not using a build system and just want to embed this in your webpage:

```html
<script src="/path/to/highlight.pack.js"></script>
<script src="/path/to/highlightjs-teradata-sql/teradata.js"></script>
<script>
  hljs.registerLanguage('teradata-sql', window.hljsDefineTeradataSql);
  hljs.initHighlightingOnLoad();
</script>
```

### Node.js
If you're using webpack / rollup / browserify / node:

```javascript
var hljs = require('highlightjs');
var hljsDefineRpmSpecfile = require('highlightjs-teradata-sql');

hljsDefineRpmSpecfile(hljs);
hljs.initHighlightingOnLoad();
```
