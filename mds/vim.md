#### BASIC
|||
|-|-|
`:w!`|Write file and exit vim.
`:q`|Out of vim.
`:w`|Saved file.
`:wqa`|Save and exit flaps
`:qa`|Out of vim with all open tabs.
`:qa!`|Force output of vim with all open tabs.
`:e filename`|Open file for editing.
#### TEXT BOX
|||
|-|-|
`VU`|Change entire line to maiscula.
`:%s/\<./\u&/g`|Defines first letter of each word in uppercase.
`:%s/.*/\u&`|Sets first letter of each line to uppercase letters.
`:%s/\<./\l&/g`|Defines first letter of each word in miniscula.
`:%s/.*/\l&`|Sets first letter of each line to lowercase letters.
`gu`|Change selection to lowercase.
`gU`|Change selection to uppercase.
`g~`|Switch box selection.
`Vu`|Change entire line to tiny.
#### READ / WRITE FILES
|||
|-|-|
`:1,10 w texto.txt`|Saved lines 1 to 10 in text.txt.
`:1,10 w >> texto.txt`|Adds lines 1 to 10 to text.txt.
`:23r texto.txt`|Insert the contents of text.txt file on line 23.
`:r texto.txt`|Insert content of text.txt file in the current.
#### MARKINGS
|||
|-|-|
`mk`|Mark current position as 'k'.
`:marks`|Shows all markings.
`'k`|Move cursor to mark 'k'.
#### INDENT
|||
|-|-|
`[VISUAL SELECTION] shift+<`|Indent back.
`[VISUAL SELECTION] shift+>`|Indents.
`:%retab!4`|Changes tabulation for tab size 4.
#### CCP
|||
|-|-|
`yiw`|Copy word at the cursor.
`viw`|Visual copy word at the cursor.
#### EDITION
|||
|-|-|
`:%d`|Clean content.
`:g!/Dave\|John/d`|Delete line does not contain or dave john
`:%!column -t`|Turns text into columns.
`r`|Replaces single character.
`J`|Joint line below the current one.
`cc`|Change (replace) the entire line.
`cw`|Change (replace) to the end of the word.
`vim +X texto.txt`|Password file.
#### SUBSTITUTIONS
|||
|-|-|
`:%s/\r//g`|Delete \ r files crlf (^ m).
`:%s/old/new/gw`|Replace all occurrences with confirmation.
`:%s/\<./\u&/g`|Capitalize word.
`:%s/\(STRING\)/\=system("awk '{printf tolower($0)}' <<<".submatch(1))/g`|Replace STRING to string, using AWK tolower() function.
`:%s/DATE/\=system("echo -n $(date +\"%Y%m%d\")")/g`|Replace DATE match with YYYYMMDD from system.
`:%s/^\(.*\)\n\1$/\1/`|Delete rows that appear twice.
`:%s#<[^>]\+>##g`|Delete html tags, but keep the text.
`:s/Bill/Steve/`|Replace the first occurrence of bill by steve on the current line.
`:2,35s/old/new/g`|Replace all occurrences between the lines 2:35
`:5,$s/old/new/g`|Replace all occurrences of 5 to eof line.
`:%s/\d\+/\=(submatch(0)+1)/g`|Sum found numbers.
`:%s!\~!\= expand($HOME)!g`|Substitutes ~ to / home / user.
`:%s/STRING/\=system('echo -n "'.submatch(0).'+1"')`|Replace STRING to STRING+1 with system.
`:s/Bill/Steve/g`|Replace bill by steve on the current line.
`:%s/Bill/Steve/g`|Replace bill by steve throughout the file.
`:v/string/d`|Delete all lines that do not contain 'string'.
`:%s/\([A-Z]\)/\L\1\e/g`|Turns capital letters to lowercase.
`:g/string/d`|Delete all lines containing 'string'.
`:%s/ *$//g`|Delete all blank spaces
`:s/Bill/\02/g`|Bill seeks and uses the search value to replace and add 2 on the front.
`:%s/\([a-z]\)/\U\1\e/g`|Changes to lowercase capital letters.
`:%s/\v(\S+)/\=expand(submatch(1))/g`|Substitutes ~ to / home / user.
#### ABAS
|||
|-|-|
`:tabfirst`|Goes to first tab.
`gt`|Next tab.
`:tabnew`|Creates new tab.
`:tabdo %s/foo/bar/g`|Run a command on all tabs.
`:tablast`|Go to last tab.
#### DIFFERENCES
|||
|-|-|
`vim -d <(ls /home) <(ls /tmp)`|Differences of two folders.
`]c`|Next difference.
`[c`|Previous difference.
`do`|Get difference.
`dp`|Puts difference.
`:diffupdate`|Scan files again looking for differences.
`vim -d arquivo1.txt arquivo2.txt`|Shows differences between files.
#### EXTRAS
|||
|-|-|
`:%s/^/\=printf('%-2d', line('.'))`|Add the line number at the beginning of the line.
`:%!python -c "import sys;entrada=sys.stdin.read().strip().split('\n');print '\n'.join([linha for linha in entrada])"`|Change lines with python.
#### SEARCH
|||
|-|-|
`?word`|Search 'word' from the bottom up.
`/word`|Search 'word' from top to bottom.
`/^\n\{3}`|Find three empty lines.
`/\<\d\d\d\d\>`|Look exactly 4 digits.
`/fred\|joe`|Search 'fred' or 'joe'.
`/jo[ha]n`|Search 'john' or 'joan'.
`*`|Word hightlight the cursor.
