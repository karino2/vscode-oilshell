# oilshell-extension README

This is a VS Code extension for [Oil](http://www.oilshell.org/) shell script.

![oil syntax highlight](images/demo.png)


## Features

- Basic colorring support

## For contributor

If you want to add grammar, please also add example of that script in tests/test.oil.

## Basic concept

Basically, this extension treats the script as command mode.
If the extension can easily figure out and narrow down the region of Expression Mode with regexp, treat it as Expression Mode.
For example, it isn't easy to narrow down Subexpression region when square bracket nesting. In this case, treat Expression Mode only until the first closing square bracket.
In doubt, go to command mode.