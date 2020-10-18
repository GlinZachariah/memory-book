---
title: Data Types
linktitle: Data Types
toc: true
type: docs
draft: false
menu:
  basics:
    parent: Basics
    weight: 1

# Prev/next pager order (if `docs_section_pager` enabled in `params.toml`)
weight: 1
---

## Primitive Data Types

TYPE| DEFAULT_VALUE| WRAPPER_CLASS|
----|--------------|--------------|
int | 0| Integer |
float | 0.0f| Float |
boolean | false| -|
double |	0.0d| Double|
byte  | 0| -|
long  | 	0L| Long|
char | '\u0000'| Character|
-| -|BigInteger

> BigInteger is used when there is very large data more than Long to be stored.



### Mathethical Operators 
-	addition(\+)
-	subtraction(\-)
-	multiplication(\*)
-	division(/)

{{% alert note %}}
Shorthand operations can be performed using ( `<operator>=`) eg: result+=5 ==> [ result = result + 5]
{{% /alert %}}

### Increment Decrement Operators
-	`++` (Increment)
-	`--` (Decrement)

{{% alert note %}}
Autoboxing - Converting a primitive value into an object of the corresponding wrapper class is called autoboxing.eg. int to Integer
<br>
Unboxing - Converting an object of a wrapper type to its corresponding primitive value is called unboxing. eg. Integer to int.
{{% /alert %}}

### Wrapper Class Operations

> The methods given below are STATIC for more details refer subclass in the [Offical Docs](https://docs.oracle.com/javase/8/docs/api/java/lang/Number.html).

CLASS | METHOD | DESC |
------|--------|------|
Integer,Double,Long | MIN_VALUE | returns min value possible|
	,,	|MAX_VALUE	|	returns max value possible| 
	,,	|doubleValue() | returns double value |
	,,	| floatValue() | returns float value |
	,,  | toString(T i)| return String value|
Integer	| parseInt(String str)| parse string to Integer |
 Double | parseDouble(String str)| parse string to Double|
 Float  | parseFloat(String str) | prase string to Float |
 Double,Float	|isNaN(double d)| check if its not a number
Long    | parseLong(String str)| parse string to Long |


> The methods given below are NON STATIC for more details refer the [Offical Docs](https://docs.oracle.com/javase/8/docs/api/java/math/BigInteger.html).

CLASS | METHOD | DESC |
------|--------|------|
BigInteger| add(BigInteger i) | returns sum of two numbers|
	,,	|subtract(BigInteger i)| returns diff of two numbers|
	,,	| not() |returns value ie. (~this).|
	,,	|min(BigInteger val) |returns the minimum|
	,,	|max(BigInteger val) |returns the maximum|
	,,	|toString() | returns string


## Non-Primitive Data Types

TYPE| DEFAULT_VALUE|
----|--------------|
String | null|

### Declaration of String
```
String str = new String();
String st = "";

```

### String Methods
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
indexOf(int ch/String str,[int fromIndex])|Returns the index within this string of the first occurrence of the specified character/substring. Starting from the fromIndex.|
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