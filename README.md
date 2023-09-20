# HighLevelAssembler

## Summary
Low-level language programming is hard. Assembly language programming is hard. High-level languages were developed to make programming easier. If students are to learn the concepts of assembly language programming it may help to start by programming in a language that is halfway between the high-level language they are (one hopes) used to and the AQA assembly language instruction set. HighLevelAssembler (HLA) is a language that tries to be that 'bridge' language.

## The HLA language definition in EBNF
```
digit                         = "0" | "1" | "2" | "3" | "4" | "5" | "6" | "7" | "8" | "9" ;
letter                        = "A" | "B" | "C" | ... | "X" | "Y" | "Z" ;
number                        = digit, { digit } ;
label                         = letter, { letter } ;
register                      = "R0" | "R1" | ... "R14" | "R15" ;
memory reference              = "Memory[", (number | label ), "]" ;

labelled statement            = [ label, ":" ] statement ;
statement                     = load statement | store statement | arithmetic statement | logical statement | shift statement | conditional statement ;  
assignment                    = memory to register assignment | register to memory assignment ;
memory to register assignment = register "=" 
register to memory assignment =
```


# Contents
1. 
