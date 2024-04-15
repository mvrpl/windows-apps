#### METHODS STRINGS
|||
|-|-|
`'STRING'.center(10)`|Centralizes string space of 10 characters
`'   '.isspace()`|Checks if the string contains only spaces
`'STRING/STRING2'.split('/')`|Separates in list based on character
`'STRING'.isupper()`|Validates the string this all in upper.
`'STRING'.capitalize()`|Changes string to first upper rest to lower.
#### DATA TYPES
|||
|-|-|
`float`|Floating-point number.
`long`|Full greater than 32-bits.
`int`|Full 32-bit.
`complex`|Number complex.
`dict`|Dictionary.
`list`|Sequence changeable.
`tuple`|Sequence immutable.
`str`|Sequence of characters.
`bool`|Boolean.
#### FORMAT DATES
|||
|-|-|
`%x`|Date.
`%X`|Hour.
`%A`|Day (monday).
`%I`|12 noon (leading zeros) (01 to 12).
`%M`|Minute (00-59).
`%m`|Months (01 to 12).
`%U`|Week number (00-53).
`%Y`|Year four digits.
`%a`|Day abbreviation (mon).
`%b`|Abbreviated month (jan).
`%d`|Day (leading zeros) (01-31).
`%j`|Day of the year (001-366).
`%Z`|Timezone.
`%H`|24 hours (leading zeros) (00-23).
`%p`|Am or pm.
`%w`|The weekday number (0-6).
`%f`|Milliseconds.
`%%`|Literally%.
`%B`|Name of the month (january).
`%c`|Date and time.
`%S`|Seconds (00-59).
`%y`|Two year digits.
#### UTILS
|||
|-|-|
`print ''.join(['\\x'+char.encode('hex') for char in 'Hello World\x0a'])`|Convert unicode characters in HEX.
