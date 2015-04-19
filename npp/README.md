
## Syntax Highlighters for NP++


 + ***algol68g.xml***

    A horrible syntax file for a horrible language.

    Please note:
        
      + Only supports simple names, i.e., whitespace isn't supported. This goes double for stdlib functions. I simply haven't found a way to express it in UDL yet, and I don't think it's possible at all.

      + Some things are rather hacky, for example `COMMENT ... END COMMENT` are implemented by simply only recognizing `COMMENT` as star- and end-block of a block-comment. Hashtag-based comment-blocks (`#`) work just fine, of course.

 + ***asm_improved.xml***

    An attempt to cover most common assembly language families, including GNU as, nasm/yasm, masm, and co.  
    Works, more or less.

 + ***awk.xml***
 
    Pretty standard stuff, but makes no attempt to highlight supposed "local" variables of awk; they're already beyond funky as is (delimited by space, of all things!), so you'll have to do without them. Sorry.

    Regex literals are *somewhat* recognized. And by "somewhat", I mean in a horrible, broken way.

 + ***brainfuck.xml***

    The worlds most lazy syntax highlighter.

 + ***crystal.xml***

    Since it's already pretty similar to Ruby, it was easy enough to implement.  
    Alas, UDL doesn't support regular expressions (or so I've been told), so matching regex-literals won't work. If you need them, take a look at the awk highlighter.

 + ***fortran90.xml***

    Similar to Algol, some things are *not* supported in this highlighter; specifically, code lacking whitespace delimiters. So code like `CO N TI NUE` won't be recognized.
    

 + ***go.xml***

    Found no problems so far. It's a pretty ~~primitive and stupid~~ simple language, after all.

 + ***julia.xml***

    Sort of finished, eventually. Maybe.

 + ***nim.xml***

    Same as with julia.
