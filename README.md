# BASH

## Overview
BASH allows for the usage of colors and font styles in the output by means of escape sequences.  The general format is:
```
<escape-sequence><font code>The following text will have the preceding codes' properties
```
### Escape sequences
The following values are valid escape sequences

- ```\e``` 
- ```\033``` 
- ```\x1B``` 


### Codes
The following values are valid font codes (more to come later):

**Font Styles**
- ```[0m``` - Normal Text
- ```[1m``` - Bold Text
- ```[2m``` - Dim Text
- ```[4m``` - Underlined Text
- ```[7m``` - Inverted Text

####Example
```
This text would appear normal \e[01mand this text would appear bold, \e[0mand this text would appear normal again
```
