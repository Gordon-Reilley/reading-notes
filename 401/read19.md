# Automation

## Python Regular Expressions Tutorial

- **Regular Expressions**, often shortened as `regex`, are a sequence of characters used to check whether a pattern exists in a given text (string) or not.
- If you've ever used search engines, search and replace tools of word processors and text editors - you've already seen regular expressions in use. 
- They are used at the server side to validate the format of email addresses or passwords during registration, used for parsing text data files to find, replace, or delete certain string, etc. 
- They help in manipulating textual data, which is often a prerequisite for data science projects involving text mining.
- Start with importing `re` - Python library that supports regular expressions.
- Very useful functions provided by the re library:
  - `compile()` 
  - `search()` 
  - `findall()` 
  - `sub()` for search and replace 
  - `split()`
- The re library in Python provides several functions that make it a skill worth mastering.
- You can easily tackle many basic patterns in Python using ordinary characters. Ordinary characters are the simplest regular expressions. They match themselves exactly and do not have a special meaning in their regular expression syntax.
- The `match()` function returns a match object if the text matches the pattern. Otherwise, it returns `None`.
- The `r` is called a raw string literal. It changes how the string literal is interpreted. Such literals are stored as they appear.
- For example, `\` is just a backslash when prefixed with an r rather than being interpreted as an escape sequence.
- Sometimes, the syntax involves backslash-escaped characters, and to prevent these characters from being interpreted as escape sequences; you use the raw r prefix.
- Special characters are characters that do not match themselves as seen but have a special meaning when used in a regular expression. 
- With the `search()`, you scan through the given string/sequence, looking for the first location where the regular expression produces a match.
- The `group()` returns the string matched by the re. You will see both these functions in more detail later.
- `$` - Matches the end of string. This is helpful if you want to make sure a document/sentence ends with certain characters.
- `\` - Backslash. Perhaps, the most diverse metacharacter!!:

  - If the character following the backslash is a recognized escape character, then the special meaning of the term is taken 
  - Else if the character following the `\` is not a recognized escape character, then the `\` is treated like any other character and passed through.
  - `\` can be used in front of all the metacharacters to remove their special meaning.
### Things I want to know more about

- Want to get more practice with regex so I don't have to rely on the internet as much for solutions.
### Sources

- <https://pymotw.com/3/shutil/>
- <https://www.datacamp.com/tutorial/python-regular-expression-tutorial>
- <https://www.youtube.com/watch?v=qbW6FRbaSl0&t=69s>

[Back To Home](../README.md)