# Numbers
Pretty similar to standard Python.
```
# Addition
1 + 1 #=> 2

# Subtraction
2 - 1 #=> 1

# Multiplication
2 * 2 #=> 4

# Division
10 / 5 #=> 2

# Exponent
2 ** 2 #=> 4
3 ** 4 #=> 81

# Modulus (find the remainder of division)
8 % 2 #=> 0  (8 / 2 = 4; no remainder)
10 % 4 #=> 2  (10 / 4 = 2 with a remainder of 2)

```
### Integers and Floats
The 2 main types of numbers in Ruby.
- Integers: 1, 39, -200
- Floats: 10.0, -2.3
```
17 / 5 #=> 3, not 3.4
17 / 5.0 #=> 3.4
```
### Useful Number Methods
Convert integers to floats with
```
# To convert an integer to a float:
13.to_f #=> 13.0

# To convert a float to an integer:
13.0.to_i #=> 13
13.9.to_i #=> 13
```
Decimal points are cut off when converting from float to integer.

Check if a number is even or odd with:
```
6.even? #=> true
7.even? #=> false

6.odd? #=> false
7.odd? #=> true

```

# Strings
Strings can be formed with either "" or '' quotation marks aka string literals.
### Concatenation
```
# With the plus operator:
"Welcome " + "to " + "Odin!" #=> "Welcome to Odin!"

# With the shovel operator:
"Welcome " << "to " << "Odin!" #=> "Welcome to Odin!"

# With the concat method:
"Welcome ".concat("to ").concat("Odin!") #=> "Welcome to Odin!"
```

### Substrings
You can access strings within strings by:
```
"hello"[0] #=> "h"
"hello"[0..1] #=> "he"
"hello"[0,4] #=> "hell"
"hello"[-1] #=> "o"
```

### Escape Characters
```
\\  #=> Need a backslash in your string?
\b  #=> Backspace
\r  #=> Carriage return, for those of you that love typewriters
\n  #=> Newline. You'll likely use this one the most.
\s  #=> Space
\t  #=> Tab
\"  #=> Double quotation mark
\'  #=> Single quotation mark
```

### String Interpolation
Allows you to create a string with placeholder variables
```
name = "Odin"

puts "Hello, #{name}" #=> "Hello, Odin"
puts 'Hello, #{name}' #=> "Hello, #{name}"
```

### Common String Methods
Capitalizing the first letter:
```
"hello".capitalize #=> "Hello"
```
Seeing if a string has a certain substring:
```
"hello".include?("lo") #=> true

"hello".include?("z") #=> false
```
Making all letters of a string uppercase:
```
"hello".upcase #=> "HELLO"
```
Making all letters of a string lowercase:
```
"Hello".downcase #=> "hello"
```
Checking if a string is empty:
```
"hello".empty? #=> false

"".empty? #=> true
```
Finding length of a string:
```
"hello".length #=> 5
```
Reversing a string:
```
"hello".reverse #=> "olleh"
```
Splitting a string by a certain character:
```
"hello world".split #=> ["hello", "world"]

"hello".split("") #=> ["h", "e", "l", "l", "o"]
```
Stripping a string of whitespace:
```
" hello, world   ".strip #=> "hello, world"
```
### Other String Methods
```
"he77o".sub("7", "l") #=> "hel7o"

"he77o".gsub("7", "l") #=> "hello"

"hello".insert(-1, " dude") #=> "hello dude"

"hello world".delete("l") #=> "heo word"

"!".prepend("hello, ", "world") #=> "hello, world!"
```

### Converting Objects to Strings
```
5.to_s #=> "5"

nil.to_s #=> ""

:symbol.to_s #=> "symbol"
```

# Symbols
Strings caan be changes (mutable), but symbols are only stored in memory once.

To create a symbol:
```
:my_symbol
```

### Symbols vs Strings
```
"string" == "string" #=> true

"string".object_id == "string".object_id #=> false

:symbol.object_id == :symbol.object_id #=> true
```

# Booleans
These are the basic true and false values.
```
true
false
```
### Nil
"nil" represents "nothing". Everything in Ruby has a return value. When a piece of code doesn’t have anything to return, it will return nil.
```
nil
```