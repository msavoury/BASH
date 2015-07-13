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
### Colors
Shells often support 16-color mode and 256-color mode. Below are the charts for both 16 and 256 color modes

### 16-color
**Foreground**: 30-37 and 90-97

**Background**: 40-49 (no 48) and 100-107

### 256-color
**Foreground** (text)

For using one of the 256 colors on the foreground (text color), the control sequence is ”<Esc>[38;5;ColorNumberm” where ColorNumber is one of the following colors: (1-256)

**Background**

For using one of the 256 colors on the background, the control sequence is ”<Esc>[48;5;ColorNumberm” where ColorNumber is one of the following colors:
