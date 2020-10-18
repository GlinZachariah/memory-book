---
title: Primitive DataTypes
linktitle: Primitive DataTypes
toc: true
type: docs
draft: false
menu:
  example:
    parent: DataTypes
    weight: 1

# Prev/next pager order (if `docs_section_pager` enabled in `params.toml`)
weight: 1
---

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

> Shorthand operations can be performed using ( `<operator>=`) eg: result+=5 ==> [ result = result + 5]

### Increment Decrement Operators
-	++ (Increment)
-	--- (Decrement)


> Autoboxing - Converting a primitive value into an object of the corresponding wrapper class is called autoboxing.eg. int to Integer

> Unboxing - Converting an object of a wrapper type to its corresponding primitive value is called unboxing. eg. Integer to int.

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


> The methods given below are NONSTATIC for more details refer subclass in the [Offical Docs](https://docs.oracle.com/javase/8/docs/api/java/math/BigInteger.html).

CLASS | METHOD | DESC |
------|--------|------|
BigInteger| add(BigInteger i) | returns sum of two numbers|
	,,	|subtract(BigInteger i)| returns diff of two numbers|
	,,	| not() |returns value ie. (~this).|
	,,	|min(BigInteger val) |returns the minimum|
	,,	|max(BigInteger val) |returns the maximum|
	,,	|toString() | returns string

