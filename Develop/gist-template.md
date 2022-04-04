# Email REGEX

## Summary

The regex I have chosen is a fairly common one. It is used to search for matches in an email. So whenever you log in to a site that requires an email, or when you are signing up, this function is going to be used, to make sure you have entered a valid email address. 

## Table of Contents

- [Anchors](#anchors)
- [Quantifiers](#quantifiers)
- [Character Classes](#character-classes)
- [Flags](#flags)
- [Grouping and Capturing](#grouping-and-capturing)
- [Bracket Expressions](#bracket-expressions)
- [Greedy and Lazy Match](#greedy-and-lazy-match)
- [Look-ahead and Look-behind](#look-ahead-and-look-behind)

## Regex Components

    /^([a-z0-9_\.-]+)@([\da-z\.-]+)\.([a-z\.]{2,6})$/

### Anchors

    Anchors are tokens use to match and compare strings within JavaScript. There are two main anchor tokens "^" and "$". The "^" token is used at the beginning of a string while the "$" token is used at the end. In this case these two anchors are at the beginning and end of a string of characters that we are using to see if an email matches the criteria we have provided.

### Quantifiers

    Quantifiers are used to specify the amount of specific characters in a certain string. They are most commonly used to check the amount of numbers, letters in a string. However they can also be used to generate a string, using the quantifiers you specify the amount of numbers, letters, and characters you want in that string. The Qauntifiers in this function are used at the end "{2,6}" this is indictating the length of the final substring, so in this case the final substring has to be at least 2 characters long, and no more that 6 characters long. 


### Character Classes

    Character classes are used to specify which characters you are looking for in a function. So you would have a-z for lowercase letters A-Z for uppercase letters, and 0-9 for numbers. These character classes are used in conjunction with everything discussed so far. You can seein the function below the character classes are inside the brackets. 

   [a-z0-9_\.-][\da-z\.-][a-z\.]

### Flags

    Flags allow for advanced searching when looking for matches with a function. They can be used to search globally, multi-line, case-sensative indicies, and many more. They are used by using a single character in your regular expression. Some flags include "g" for global-search, "m" for multi-line search,"i" for case-sensative indicies. In this string we use the "d" flag when we check for matches in the email name. Since email name won't have any numbers, and may have only one capital letter, we use this flag here. 

    [\da-z\.-]


### Grouping and Capturing

    Grouping is very important in this regex function, because we are looking to match three distinct substrings within the entire function. However there are certain character in between those strings that will stay the same, no matter what, like "@" and ".". It is important that these are handled correctly or the function wouldn't be able to run

### Bracket Expressions

    We use brackets in our function to separate out the different substrings we are looking for. So in the first bracket "[a-z0-9_\.-]" we are looking for the email name, before the "@". The next bracket "[\da-z\.-]" we are looking for the name of the actual email provider, so "gmail", or "hotmail". In the last bracket "[a-z\.]" we are looking for that .com, or .in. 

### Greedy and Lazy Match

    In a Regex function, Greedy means looking for as many matches as possible, and we see that highlighted in our Regex function in the second bracket "/da-z" The "/" used in conjuction with the "d" it will look for as many matches as possible in that string. 


## Author

    I am a "junior developer in-training" and I wrote this tutorial to help people just like me learn a little more about REGEX, and speifically this expression used to match email addresses. This would be one of the most commonly used. 

    You can find more of my work here!: https://github.com/Thoma77s?tab=repositories
