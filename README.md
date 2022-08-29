# REGEX

# Summary 

There are two main ways of created a Regex object; either by using literal syntax, the second way is by using the RegExp() constructor.

The literal syntax (/pattern/) uses forward slashes to wrap the regular expression pattern and does not use quotation marks, whereas the constructor syntax ("pattern") uses quotation marks and is not enclosed between slashes.

One way Regex could be used is to validate user input.

I'll be using this line of code throughout my tutorial:

/^(https?:\/\/)?([\da-z\.-]+)\.([a-z\.]{2,6})([\/\w \.-]*)*\/?$/


# Table of Contents

- [Anchors](#anchors)
- [Quantifiers](#quantifiers)
- [Grouping Constructs](#grouping-constructs)
- [Bracket Expressions](#bracket-expressions)
- [Character Classes](#character-classes)
- [The OR Operator](#the-or-operator)
- [Flags](#flags)
- [Character Escapes](#character-escapes)


## Regex Components

# Anchors
An anchor in regex represents the position of the string from the beginning to its .end.
The caret ^ is positioned before the first character in the string. For example in our line of code:

/^(https?:\/\/)?([\da-z\.-]+)\.([a-z\.]{2,6})([\/\w \.-]*)*\/?$/

The caret is found after the forward slash used in the literal syntax, this indicates that the string starts from the opening parenthesis and not at the beginning line of code. 

Similarly, the dollar sign $ shows the ending of the string and is to be found at the end of the code line.

### Quantifiers
Quantifiers shows how many instances a character is present in the line of code. Quantifiers can be applied to the individual characters and classes contained by the parentheses.

### Grouping Constructs
Regex uses parenthesis to group substrings of an input string to combine a sequence of literals and pattern characters.

There are a few different types of grouping constructors:

* x|y -> Matches either "x" or "y".
* /(foo)/ -> Capturing group. Matches and remembers the match character.
* (?:x) -> Non-capturing group. Does not remember the match.
* [xyz] -> Character class. Matches any one of the characters in the range.
 * a-c] -> You can specify the range of characters by using a hyphen. But if the hyphen is at the beginning or ending of the square brackets then it is taken as a 
 literal hyphen.

For example in our code: [a-z\.] the hyphen is found in the middle of the square brackets so it is a character, whereas [\/\w \.-] in this code block the hyphen is found at the end of the square bracket making the hyphen a literal hyphen and not a character class.

### Bracket Expressions
Bracket Expressions are characters enclosed by a square bracket matching any character within the brackets.


### Character Classes
Character classes are what we call the square brackets that surround a string/ pattern of characters. The character class always matches at least one of the characters found inside the square brackets. For example in our code, there are 3 character class instances ([\da-z\.-]+), ([a-z\.]{2,6}), ([\/\w \.-]*). For each of these character class contents at least one of its letters or numbers matches the original URL string.

We could further break down the code inside the square brackets:

* [abc] -> Matches any one of these characters a, b or c.
* [^abc] -> Matches any other character apart from a, b or c.
* [a-z] -> Matches any character from lowercase a to lowercase z.
* [A-Z] -> Matches any character from uppercase A to uppercase Z.
* [a-Z] -> Matches any character from lowercase a to uppercase Z.
* [0-9] -> Matches any single digit from 0-9.
* [a-z 0-9] -> Matches a single character from a-z or 0-9.

### The OR Operator
The or expression give the operator to use either one function or the other. The common regular expression for this operators is the(|).

### Flags
Flags in regex are a form of optional parameters that a user could add to an expression to change the search method.

i -> Ignores casing. Makes expression case-insensitive.
g -> Global. Makes expression search for all occurrences in the global.
s -> Dot All. Makes the wild character . match newlines.
m -> Multiline. Makes the boundary characters ^ and $ match the beginning and ending of every single line instead of the beginning and ending of the whole string.
y -> Sticky. Makes the expression start its searching from the index indicated in its lastIndex property.
u -> Unicode. Makes the expression assume individual characters as code points and matches 32-bit characters.

### Character Escapes
Escape character is a character that invokes an alternative interpretation on the following characters in a sequence. The "" character is the expression that denotes a specific character is a escaped character. For example:

* \d => Matches any digit.
* \D => Matches any non-digit.
*\f => Matches a form feed.

## Author

Amina Hayat

contact me: https://github.com/aminahayat, hayat.amina@hotmail.com

