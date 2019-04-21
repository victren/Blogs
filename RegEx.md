
The value of dotAll is a Boolean and true if the "s" flag was used; otherwise, false. 
The "s" flag indicates that the dot special character (".") should additionally match 
the following line terminator ("newline") characters in a string, which it would not 
match otherwise:

U+000A LINE FEED (LF) ("\n")

U+000D CARRIAGE RETURN (CR) ("\r")

U+2028 LINE SEPARATOR

U+2029 PARAGRAPH SEPARATOR

This effectively means the dot will match any character on the Unicode Basic Multilingual Plane (BMP). 
To allow it to match astral characters, the "u" (unicode) flag should be used. 
Using both flags in conjunction allows the dot to match any Unicode character, without exceptions.

A line feed means moving one line forward. The code is \n . 
A carriage return means moving the cursor to the beginning of the line. The code is \r . 
