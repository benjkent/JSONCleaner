﻿# JSONCleaner
# Uses Regular Expression to find instances of 
- \n
- \ where they preceed another \
- \ where they preceed /
- \ where they preceed ""
- \ where they preceed <

### The purpose is the identification of escape characters present in a JSON response body comprised of Html.

``` \\n|\\(?=\\)|\\(?=\/)|\\(?=\"")|\\(?=\<)/gm ```

