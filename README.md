# JSONCleaner
# Uses Regular Expression to find instances of 
- \n
- \ where they preceed another \
- \ where they preceed /
- \ where they preceed ""
- \ where they preceed <
- \ where they follow =
- \ where they follow a-z characters
- \ where they follow 0-9 characters

### Prints the output of the resulting replacement, rather omission, of the found characters: backslashes \

### The purpose is the identification of escape characters present in a JSON response body comprised of Html.

``` \\n|\\(?=\\)|\\(?=\/)|\\(?=\"")|\\(?=\<)|(?<=\=)\\|(?<=[a-z])\\|(?<=[0-9])\\|/gm ```





