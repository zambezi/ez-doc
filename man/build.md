Building documentation
======================

It's easy to get started with ez-doc. All you need are two files in your project:

- README.md
- SUMMARY.md

The first is an introduction to your project, and the second is summary of your documentation – you can think of it as a table of contents. The summary can contain anything really, but at minimum it should contain a list of links. This list is your table of contents, and will be extracted to generate the navigation for your site.

As an example, you may take a look at [this project's summary](../SUMMARY.md):

```markdown
Summary
=======

- [Building docs](man/build.md)
- [Serving locally](man/serve.md)
```

Aside from being used for navigation, the summary also designates which files to process for the site generation. Any file that's linked to will be processed, which means aside from generating the necessary html, any local links to other processed files will be rewritten to their generated counterparts.

However, only markdown syntax will be processed – html embedded in the markdown documents is left as-is.

Usage
-----

To build your documentation, simply run the following at the root of your project:

```sh
ez-doc build
```

The `build` command will simply build your documentation and place it in the `_book` directory. If there are no errors, it will exit successfully without writing anything to stdout. If there are errors, they will be printed to stderr and ez-doc will exit with a non-zero exit code.