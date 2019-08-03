If you prefer reading this information in Russian,
you find it in the separate file [README_RU.md](README_RU.md).

# Russian Gblorb

Blorb files are a way to package IF games and their associated
resources into a single file. A resource in this case is usually
either a picture or a sound effect. The game file itself can also be
considered to be a resource. By bundling your game and its pictures
and sounds into a single file, you make it much easier to distribute
the game -- instead of multiple files, your game is now held in just
one file.

Of course, this really only makes sense if game interpreters exist
that can play games directly from Blorb files. If you are reading
this, it's likely that you've already determined that a Blorb-aware
interpreter exists for the game system that you are using. Otherwise,
you should check this before going much further.

Gblorb is a small program that lets you create Blorb files from your
game files and resources. It can also list the resources in a Blorb
file, and extract each into a separate disk file for you.

This is a version of Gblorb with an interface translated into Russian.

## Build

To build Gblorb you will need the Inform 6 compiler
and the Inform 6 standart library with the infglk.h header file.

Use something like the following command to compile the gblorb.inf:

```shell
inform +library +language_name=Russian -G -Cu $DICT_CHAR_SIZE=4 $MAX_UNICODE_CHARS=128 $MAX_EXPRESSION_NODES=1000 $MAX_STATIC_DATA=80000 gblorb.inf gblorb.ulx
```

## Original project

The original version of Gblorb was written by Simon Baldwin
and is available in the Interactive Fiction Archive at the link
https://ifarchive.org/if-archive/programming/blorb/gblorb.zip
