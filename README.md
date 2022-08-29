# REGEX

# Summary 

There are two ways of creating a new RegExp object, by using the literal syntax, or by using the RegExp() constructor.

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
An Anchor in regex shows the position of the beginning of the string and its ending .

The caret ^ is positioned before the first character in the string. For example in our line of code:

/^(https?:\/\/)?([\da-z\.-]+)\.([a-z\.]{2,6})([\/\w \.-]*)*\/?$/
the caret could be found after the forward slash used in the literal syntax indicating that the string starts from the opening parenthesis and not at the beginning of the line of code.

Similarly, the dollar sign $ shows the ending of the string and is to be found at the end of the code line.

### Quantifiers

### Grouping Constructs

### Bracket Expressions

### Character Classes

### The OR Operator

### Flags

### Character Escapes

## Author

A short section about the author with a link to the author's GitHub profile (replace with your information and a link to your profile)