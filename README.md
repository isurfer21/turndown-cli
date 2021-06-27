# turndown-cli

A command-line-interface tool for [turndown](https://github.com/domchristie/turndown) module. 

It converts the `.html` file into `.md` file. So basically, it is a CLI based HTML to Markdown converter tool.

## Install

You can install it via `npm`, but make sure your system have `node.js` installed prior to that.

```shell
% npm install td

```

## Usages

The help option shows all the relevant information regarding the usages of the app.

```shell
% td -h

Usages:
  td (-h|-v)
  td <source> (<target>)
  td (<option>=<choice>) <source> (<target>)

Parameters:
  source    HTML source filepath
  target    Markdown target filepath
  option    Any option from provided options
  choice    Any choice out of provided choices

Options:
  -t --head       Heading style
                  1) setext    2) atx
  -r --hr         Horizontal rule
                  1) *    2) -    3) _
  -b --bullet     Bullet list marker
                  1) *    2) -    3) +
  -c --code       Code block style
                  1) indented    2) fenced
  -f --fence      Fence style
                  1) `    2) ~
  -e --em         Em delimiter
                  1) _    2) *
  -s --strong     Strong delimiter
                  1) **    2) __
  -l --link       Link style
                  1) inlined    2) referenced
  -u --linkref    Link reference style
                  1) full    2) collapsed    3) shortcut
  -p --pre        Preformatted code
                  1) false    2) true

Note that the first choice is default for each options.

Examples:
  td -h
  td sample.html
  td sample.html sample.md
  td -t=2 -r=3 -c=2 -f=1 -s=2 sample.html


```