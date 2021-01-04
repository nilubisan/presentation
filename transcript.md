A regular expression ("regex")  is a pattern describing a certain amount of text. It provides a very powerful way to manipulate text  in a very compact syntax. For example, it can be used to verify whether the format of data i.e. name, email, phone number, etc. entered by the user is correct or not.
One of the most interesting features is that once you’ve learned the syntax, you can actually use this tool in almost all programming languages with the slightest distinctions about the support of the most advanced features and syntax versions.

If you are not a programmer, you can use regular expressions in many situations as well. They make finding information a lot (lot) easier. There are many text editors and search and replace tools with decent regex support. Now on slide you can see a simple example of regular expression. It finds both spellings of the word gray in one operation, instead of two. 

To see the real benefit of using regular expression let’s suppose we have a string and we need to check if this string contains alpha-numeric characters. So here is typical function without using regex. At first it checks whether it’s empty string or not, then we run a for-loop and on each iteration we match every character of string by using Unicode codes.
As you can see, the purpose of this function is just one little thing – to check if the string contains any numerals or letter and to do this we have to write this heavyweight and awkward code. 

But there is a better solution. Instead of loops, iterations and character by character checks we can automate our process. As you can see on the slide by using regular expressions, the same functionality as shown in the previous slide can be achieved by one simple line of code. 

Regular expressions are useful in any scenario that benefits from full or partial pattern matches on strings. These are some common use cases:
verify the structure of strings
extract substrings from structured strings
search / replace / rearrange parts of the string
split a string into tokens
All of these tasks come up regularly when doing some data preparation work.

Regular expressions can be useful in many areas when it comes to find, replace text by some pattern. Regex are used in
  search engines
  word processors and text editors
  many programming languages as powerful development tool

Looking at this example may be overwhelming. However, once you understand the basic syntax of how regex commands operate you can read this example just as if you are reading simple sentence. So let’s go over basic concepts of regular expressions on the example of JavaScript Regexp

At first let’s look at JavaScript's built-in methods for pattern-matching. There  are 6 methods to work with regexp. The methods exec() and test() are RegExp methods which is JavaScript built-in (bilt-in) object. 
Exec() and test() take a string as a parameter, whereas the methods search(), replace(), match() and split() are String methods that take a regular expression as a parameter.

Flags are optional parameters. They make it search in a different way. Each flag is denoted by a single alphabetic character.

There are only 6 of them in JavaScript:
For example, the flag g, which stands for global, used to extend the searching to find all matches for a given expression, instead of stopping on the first match.

Square brackets surrounding a pattern of characters are called a character class. They are used for generic search, such as to search any digit or any character.Character classes are one of the most commonly used features of regular expressions.

Character ranges matches any character in the set. To define a range of characters we use the hyphen character inside a character class,
For instance, [a-z] is a character in range from a to z, and [0-9] is a digit from 0 to 9.

There are certain situations where you want to match at the beginning or end of string. To do this you can use anchors. Two common anchors are caret (^) which represent the start of the string, and the dollar ($) sign which represent the end of the string.

\b is an anchor like the caret (^) and the dollar sign ($). It matches a position that is called a “word boundary”.

There are three positions that qualify as word boundaries:
Before the first character in a string if the first character is a word character
After the last character in a string if the last character is a word character
Between two characters in a string if one is a word character and the other is not

With quantifiers we can specify how many times a character in a regular expression should match. Quantifiers can be applied to the alone characters, as well as classes of characters, and groups of characters contained by the parentheses.

By placing part of a regular expression inside parentheses, we can group that part together. This allows us to apply a quantifier to the entire group.

Alternation is expressed with a vertical bar and essentially is used as a logical operator “OR”. We can use alternation to match a single regular expression out of several possible regular expressions.
For example, the regexp /fox|dog|cat/ matches the string "fox", or the string "dog", or the string "cat".