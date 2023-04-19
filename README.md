# Syntax Highlighting for uxntal

This syntax defintion is **_not_** fully complete. 

This definition file was created to be used alongside Pandoc to add syntax highlighting to generated HTML documents. This is the first time I've created a file like this, so it's not perfect.

## Usage

````
# Markdown Example

```uxntal
( Devices )
|10 @Console
  &vector $2
  &read $1
  &pad $5
  &write $1
  &error $1

( Macros )
%EMIT { .Console/write DEO }
%NL { #0a EMIT }

( Main Program )
|0100
  LIT "H EMIT
  LIT "e EMIT
  LIT "l EMIT
  LIT "l EMIT
  LIT "o EMIT
  NL
```

Hello World
````

```sh
pandoc example.md --syntax-defintion=uxn.xml > example.html
```
