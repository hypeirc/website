# HypeIRC Website

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

## Building the Site

To build the site run: `./pagez -s ./src -o ./public`

