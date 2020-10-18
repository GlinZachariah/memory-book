---
title: Non-Primitive DataTypes
linktitle: Non-Primitive DataTypes
toc: true
type: docs
draft: false
menu:
  datatypes:
    parent: DataTypes
    weight: 2

# Prev/next pager order (if `docs_section_pager` enabled in `params.toml`)
weight: 1
---


TYPE| DEFAULT_VALUE|
----|--------------|
String | null|

## Declaration of String
`String str = new String();`
`String st = "";`

### Methods
METHOD |DESC |
-------|-----|
charAt(int index)|Returns the char value at the specified index.|
compareTo(String anotherString)|Compares two strings lexicographically.|
compareToIgnoreCase(String str)|Compares two strings lexicographically, ignoring case differences.|
concat(String str)|Concatenates the specified string to the end of this string.
contains(CharSequence s)|Returns true if and only if this string contains the specified sequence of char values.|
equals(Object anObject)|Compares this string to the specified object.|
equalsIgnoreCase(String anotherString)|Compares this String to another String, ignoring case considerations.|
String.format(String format, Object... args)|Returns a formatted string using the specified format string and arguments.|
indexOf(int ch|String str,[int fromIndex])|Returns the index within this string of the first occurrence of the specified character/substring. Starting from the fromIndex.|
isEmpty()|Returns true if, and only if, length() is 0.|
length()|Returns the length of this string.|
matches(String regex)|Tells whether or not this string matches the given regular expression.|
replace(char oldChar, char newChar)|Returns a string resulting from replacing all occurrences of oldChar in this string with newChar.|
replace(CharSequence target, CharSequence replacement) | Replaces each substring of this string that matches the literal target sequence with the specified literal replacement sequence.|
split(String regex)|Splits this string around matches of the given regular expression.|
startsWith(String prefix)|Tests if this string starts with the specified prefix.|
substring(int beginIndex,[int endIndex]) | Returns a string that is a substring of this string.|
toCharArray()|Converts this string to a new character array.|
toLowerCase()|Converts all of the characters in this String to lower case.|
toUpperCase() |Converts all of the characters in this String to upper case.|
trim()|Returns a string whose value is this string, with any leading and trailing whitespace removed.|
String.valueOf(T i)| returns string for given type T.|