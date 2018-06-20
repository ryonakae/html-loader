# HTML Loader
Forked from [webpack-contrib/html-loader](https://github.com/webpack-contrib/html-loader).

# Added Options
## `ignore`
Type: `RegExp` Default: `undefined`

Skip processing of modules matching the regular expressions.  
In addition to ignoring module resolution, you can continue processing even if the original file does not exist.

It is effective when files exist only on the server, or when generating images dynamically with PHP.

```
// webpack.config.js
...
{
  loader: 'html-loader',
  options: {
    ignore: /no-exist-image\.png$/
  }
}
...
```