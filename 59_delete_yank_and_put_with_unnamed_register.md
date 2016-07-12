Let's say we made a mistake of typing this text:

Practica lvim

Start on the last character 'm'
`F space` - to search for space backwards
`x` - to cut
`p` - to paste

`xp` - transpose two chars

Similar concept can be used for lines

2) line two
1) line one
3) line three

Start on the first line
`dd` - to cut out the line
`p` - to insert

`ddp` - to transpose lines
`yyp` - to duplicate lines

## Using the unnamed register

collection = getCollection();
process(somethingInTheWay, target);

`yiw` - yanks the word collection into the register
`jww` - moved to the beginning of "collection"
`dw` - deletes the word
`P` - pastes before comma

But oops, try this instead of `dw`
`"_de` - deletes the word, but does not put it into register