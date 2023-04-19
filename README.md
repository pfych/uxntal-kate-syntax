# Syntax Highlighting for uxntal

This syntax defintion is **_not_** fully complete. 

## Goals

I like to take notes when learning a programming language, this is the first time my notes on my site havent had syntax highlighting. So _obviously_ instead of learning the language I should write syntax defintions for it...

Please feel free to open Issues and PRs! I've likely made mistakes...

## Usage

This definition file was created to be used alongside Pandoc to add syntax highlighting to generated HTML documents.

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

![Default syntax colours](https://user-images.githubusercontent.com/11114594/232969093-4715a503-d726-4d9c-968d-2454694cdb3d.png)

The colours in the image are the default Pandoc CSS styles, colours can be easily changed with a bit of CSS wizzardry.
