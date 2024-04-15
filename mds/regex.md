#### GROUPS AND RANGES
|||
|-|-|
`[0-7]`|Digit from 0 to 7
`.`|Any character except new line (\n)
`(...)`|Group
`[abc]`|Range (a or b or c)
`[^abc]`|Not (a or b or c)
`[A-Q]`|Upper case letter from A to Q
`(a|b)`|a or b
`(?:...)`|Passive (non-capturing) group
`[a-q]`|Lower case letter from a to q
`\x`|Group/­sub­pattern number "­x"
#### PATTERN MODIFIERS
|||
|-|-|
`x *`|Allow comments and whitespace in pattern
`e *`|Evaluate replac­ement
`U *`|Ungreedy pattern
`g`|Global match
`i *`|Case-insensitive
`m *`|Multiple lines
`s *`|Treat string as single line
#### CHARACTER CLASSES
|||
|-|-|
`\w`|Word
`\c`|Control character
`\s`|White space
`\S`|Not white space
`\d`|Digit
`\D`|Not digit
`\W`|Not word
`\x`|Hexade­cimal digit
`\O`|Octal digit
#### STRING REPLACEMENT
|||
|-|-|
`\2`|"­xyz­" in /^(abc(xyz))$/
`\1`|"­xyz­" in /^(?:abc)(xyz)$/
`\``|Before matched string
`\'`|After matched string
`\+`|Last matched string
`\&`|Entire matched string
`\n`|nth non-passive group
#### SPECIAL CHARACTERS
|||
|-|-|
`\xxx`|Octal character xxx
`\xhh`|Hex character hh
`\n`|New line
`\r`|Carriage return
`\t`|Tab
`\v`|Vertical tab
`\f`|Form feed
#### QUANTIFIERS
|||
|-|-|
`+`|1 or more {3,} 3 or more
`?`|0 or 1 {3,5} 3, 4 or 5
`*`|0 or more {3} Exactly 3
#### ESCAPE SEQUENCES
|||
|-|-|
`\Q`|Begin literal sequence
`\E`|End literal sequence
`\`|Escape following character
#### POSIX
|||
|-|-|
`[:xdigit:]`|Hexade­cimal digits
`[:space:]`|Blank characters
`[:cntrl:]`|Control characters
`[:upper:]`|Upper case letters
`[:lower:]`|Lower case letters
`[:alpha:]`|All letters
`[:alnum:]`|Digits and letters
`[:digit:]`|Digits
`[:graph:]`|Printed characters
`[:print:]`|Printed characters and spaces
`[:punct:]`|Punctu­ation
`[:blank:]`|Space and tab
`[:word:]`|Digits, letters and underscore
#### ASSERTIONS
|||
|-|-|
`?<=`|Lookbehind assertion
`?!= or ?<!`|Negative lookbehind
`?>`|Once-only Subexp­ression
`?()`|Condition [if then]
`?()|`|Condition [if then else]
`?#`|Comment
`?=`|Lookahead assertion
`?!`|Negative lookahead
#### ANCHORS
|||
|-|-|
`\b`|Word boundary.
`\B`|Not word boundary.
`\<`|Start of word.
`\>`|End of word.
`^`|Start of string, or start of line in multi-line pattern.
`\A`|Start of string.
`$`|End of string, or end of line in multi-line pattern.
`\Z`|End of string.
