# Boustrophedon Challenge

## Learning Objectives

* Task 1: Use `node` to execute a file of JavaScript; to run a REPL
* Task 2: Configure a directory ready for using Node and NPM
* Task 3: Discover documentation in Node docs for working with filesystem
* Task 4: Build a simple Unix-based utility using Node + NPM and JavaScript
* Task 5: Extend a simple Unix application with an NPM-based package

## Summary

"Boustrophe-what?!" you're asking yourself. [Boustrophedon][] is a Greek word
describing how fields were plowed. In Boustrophedon letters and words go left
to right until the end of the line. At that point they reverse, and go right to
left.

Consider:

    Love, love will tear us
    apart again.

A boustrophedonic representation would be:

    Love, love will tear us
                niaga trapa

It's surprising how after a few lines your eyes get used to reading
this way.

We want to create a Node application that takes a standard text and
Boustrophdon-izes it.

## Releases

### Release 0:  Ensure your Node and NPM environment

Ensure you have `node` installed
Ensure you have `yarn` installed
Discover the version of `node` you're running

Store these answers in a file called PREWORK.txt. Commit that file before
moving on.

### Release 1: Get Some Data

Get some data to test. We'd recommend 4-8 lines of text.

### Create and Commit your `.gitignore`

Create a `.gitignore` to keep downloaded modules from being added. Also, ignore
your file with test text. We don't need to store the history of that. Once
finished, commit this file.

### Release 2: Implement boustcat.js

`boustcat.js` is like `cat` but it displays even-numbered lines
boustrophedonically. You might find it handy to try implementing a simple `cat`
clone first and then iterate to include the boustrophedon.

Keep in mind that JavaScript doesn't have a reverse function so you're going to
have to re-implement it yourself!

It should be invoked as: `node boustcat.js source-file.txt`

### Release 3: Add Color

As boustrophedon was actually practiced in the ancient world, they created
custom letter forms of reversed letters! We can't actually write that in this
challenge because...well..we don't know where to find those glyphs on our
keyboard!

Since we're not going to use the reversed letters, how about we make our
reversed lines look different. Let's color them in an interesting way. Look
at the [colors NPM package][colors] for ideas. The inverse capability might be
really interesting!

## Stretch Release Ideas

1. Add color configuration to a `config.js` file
1. If you get idea #1 working, see if the user has a `~/.boustrc` file. By Unix
  convention, many custom configuration data are specified in `.*rc` files in
  the user's home directory (e.g. `.bashrc`, `.zshrc`, `.xinitrc`, etc.). Make
  `boustcat.js` respect a config found there by default.
1. Find a way to bring reversed letterforms to the console! It didn't seem
   possible to the humble author of this idea, but maybe you can figure out
   an approach!
   
## Conclusion

You've done something very important. You've bootstrapped your development
environment in a new language and have delivered an application that uses all
the core pieces of development in that language: node, npm, git,
community-supported packages, etc. This may seem like a trivial moment, but it
is phenomenally important.

Also realize that with this knowledge you can take any challenge from any other
phase / module / coding book and try to re-implement it in Node. Could you port
a Sudoku solver? An anagram finder? Developers tend to develop "pet projects"
that they re-implement again and again to get a "feel" for the language they're
using. Build your own preferences!

[Boustrophedon]: https://en.wikipedia.org/wiki/Boustrophedon
[colors]: https://www.npmjs.com/package/colors
