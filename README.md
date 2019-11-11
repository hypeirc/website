# HypeIRC Website

The website is live on:

* https://irc.dryware.org
* http://irc.h.dryware.org

## Requirements

* lessc
* cmark
* uglifyjs
* zsh

## Build Options

The `pagez` command has the following options:

* `-s`: Set the directory containing the website sources
* `-o`: Set the output directory to render the generated site
* `-j`: Set the path to the `uglifyjs` binary (default: `/usr/bin/uglifyjs`)
* `-l`: Set the path to the `lessc` binary (default: `/usr/bin/lessc`)
* `-m`: Set the path to the `cmark` binary (default: `/usr/bin/cmark`)

## Templates

The ones in pages/ are in markdown, the ones in html/ are — DUH — in HTML.

Both types support two types of expansions:

* %{foo} will expand into the value of $foo
* $( command ) will expand into the output of `command`

## Modules

Now writing code into the template is not pretty. Because of that, pagez
will source zsh code from mod/. Just drop a function into a file there and
call it from your template.

## Building the Site

To build the site run: `./pagez -s ./src -o ./public`
