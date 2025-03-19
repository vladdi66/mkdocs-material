# Code Annotation Examples

### Codeblocks for you
some goes here `eval "$(ssh-agent -s)"` some more explanation and even more ...
some  extra text can go here . . .

### Plain Codeblock
Just a plain block of highlighted code

```
def index(request):
  return render(request, 'index.html')
//comment: somerandom code

```
### Python Codeblock
Here is some code with `py` at the start

```py
def index(request):
  return render(request, 'index.html')
```
#### With a Title

```py title="Sort a list of strings."
my_list = ["blue", "red", "green"]

my_list.sort() 
my_list = sorted(my_list, key=len)  

import locale
from functools import cmp_to_key
my_list = sorted(my_list, key=cmp_to_key(locale.strcoll)) 
```


#### With line numbers

```py title="Checking if a file exists." linenums="1"
#Checking if a file exists in two ways
#1- Using the OS module
import os 
exists = os.path.isfile('/path/to/file')

#2- Use the pathlib module for a better performance
from pathlib import Path
config = Path('/path/to/file') 
if config.is_file(): 
    pass

```

#### Highlighting lines

```py title="Using F strings." hl_lines="1 8 12" linenums="1"
 #Formatting strings with f string.
str_val = 'books'
num_val = 15
print(f'{num_val} {str_val}') # 15 books
print(f'{num_val % 2 = }') # 1
print(f'{str_val!r}') # books

 #Dealing with floats
price_val = 5.18362
print(f'{price_val:.2f}') # 5.18

 #Formatting dates
from datetime import datetime;
date_val = datetime.utcnow()
print(f'{date_val=:%Y-%m-%d}') # date_val=2023-12-09
```
