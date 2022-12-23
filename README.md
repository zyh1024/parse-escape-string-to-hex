# parse-escape-string-to-hex
parse escape string(c-char-sequence) to hex

## Grammar：
~~~
c-char-sequence:	 
 	c-char
 	c-char-sequence c-char

c-char:	 
 	any member of the source character set except the double quote ", backslash \, or new-line character
 	escape-sequence

escape-sequence:	 
 	simple-escape-sequence
 	octal-escape-sequence

simple-escape-sequence:	 
 	\'
 	\"
 	\?
 	\\
 	\a
 	\b
 	\f
 	\n
 	\r
 	\t
 	\v

octal-escape-sequence:	 
 	\ octal-digit octal-digit octal-digit

octal-digit:	 
 	0
 	1
 	2
 	3
 	4
 	5
 	6
 	7
~~~
