Serving documentation locally
=============================

In addition to [building documentation](build.md), ez-doc can also serve up the generated `_book` directory. It's useful to serve documentation locally in order to visualize the end result. To do so, simply run the following at the root of your project:

```sh
ez-doc serve
```

This should start a server at [http://localhost:4000]().

Serving the documentation like this is not meant for production use; for that you should rather just use a static server and serve up the files as-is in the `_book` directory. The generated `_book` directory is optimized for serving using [GitHub pages](https://pages.github.com), however any web server capable of serving static files should be able to run with it.