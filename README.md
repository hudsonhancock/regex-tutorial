# Regex, The Most Useful Jibberish Ever!

Daunting at first, Regex is a powerful tool where you can search for specific characters within a string. There’s a ton that you can do with Regular Expressions. Two primary uses for regex are validating strings and find-and-replace functionality.

## Summary

Briefly summarize the regex you will be describing and what you will explain. Include a code snippet of the regex. Replace this text with your summary.

## Table of Contents

- [Syntax](#syntax)
- [Flags](#flags)
- [Special Symbols](#special-symbols)
- [Methods](#methods)
- [Validation](#validation)

### Syntax
Okay, so all regex are written inside of two forward slashes. (i.e. /dog/g).
Then, a flag is included after the closing forward slash. Here are the flags that can be used: (g, i, m, s, u, y).

### Flags
The first flag, ‘g’. Including the g after the expression, will make the search global. That means it will find all instances of the included characters within the string.

The ‘i’ flag stands for Case Insensitive. When i is included, you will find a character set even if the case isn’t matched. (i.e. The, the). For instructions on all the flags, check out regexr.com.

### Special Symbols
+
You’re probably used to the plus symbol being used to add or concatenate strings. Well, in regular expressions, the plus symbol is used to mean more than one. For example, the regex /e+/g would return all instances of e. Even if it was a double ee. (Tree, the).

?
The question mark makes whatever character before it, optional. The expression /ea?/g, would find all instances of e and all instances of a that are directly adjacent to an e.

*
The start is an extension of the question mark. It finds all instances of the character before it, even if it’s multiple instances. For instance, out the word tree, the regex /re*/g would return ‘ree’. In contrast, including a question mark would return only the first e after the r. 

.
The period matches everything. It’s very powerful. A period before a character will return the character that follows, along with the preceding character. /.a/g, will return all instances of a, along with whatever precedes it. 

\
What if you want to find a period? What if you don’t want to use a period with all its powerful glory? Well, that’s when the backslash comes into play. The backslash tells the regular expression that whatever follows is just a boring character, not a supercharged “find everything” period.

\w
What if you want to find all words? Well used the \w. Curious how to find whatever isn’t a word, well keep reading! A way to make this even more useful is by including curly braces. We can include a minimum and maximum value, separated by a comma, within curly braces to find all words that fit specific length criteria. Here’s what it looks like: /\w{2,4}/. This will return all words that have a length between 2 and 4. 

\s
This will find all whitespace! How neat.

There are so many different ways to target the types of characters you want within a string. For a complete list of characters, visit https://developer.mozilla.org/en-US/docs/Web/JavaScript/Guide/Regular_Expressions/Cheatsheet.

### Methods
There are many helpful methods you can use to search strings. Check out this chart from MDN.
[alt text](http://url/to/img.png)

### Validation
Here is how Regex can be used for form validation!
[alt text](http://url/to/img.png)

## Author

This was written by Hudson Hancock, a web developer who lives in Atlanta, GA. You can visit my github profile [here](https://github.com/hudsonhancock)
