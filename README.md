ez-doc
======

The Zambezi documentation site generator is a command line tool to generate Zambezi style documentation from markdown source files.

Installation
------------

Install the CLI tool using npm; either globally or as a local dependency. If you're going to use ez-doc as part of your project build process, it is recommended you install it as a local dependendency:

```sh
npm install --save-dev ez-doc
```

Or, if you'd rather have access to ez-doc globally:

```sh
npm install -g ez-doc
```

Usage
-----

To generate docs, you will need at minimum two files in your project:

- README.md
- SUMMARY.md

The former is the usual introduction to your project, but the latter – SUMMARY.md – might be new to you. It is the file that lets ez-doc know the structure of your documentation; put a list of links in there, and ez-doc will use this to extract navigation information for your documentation site. For more information, see the section on [building your documentation](man/build.md).

---

[License](LICENSE)