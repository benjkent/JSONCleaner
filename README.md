# JSONCleaner
# Uses Regular Expression to find instances of 
- \n
- \ where they preceed another \
- \ where they preceed /
- \ where they preceed ""
- \ where they preceed <

### The purpose is the identification of escape characters present in a JSON response body comprised of Html.

``` \\n|\\(?=\\)|\\(?=\/)|\\(?=\"")|\\(?=\<)/gm ```

# Branch FindAndReplace: enhances the expression to remove additional backslashes.
``` \\n|\\(?=\\)|\\(?=\/)|\\(?=\"")|\\(?=\<)|(?<=\=)\\|(?<=[a-z])\\|(?<=[0-9])\\|/gm ```

- \ where they follow =
- \ where they follow a-z characters
- \ where they follow 0-9 characters
### FindAndReplace also prints the output of the resulting replacement, rather omission of the found characters: backslashes \
