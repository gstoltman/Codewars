## Check to see if a string has the same amount of 'x's and 'o's. The method must return a boolean and be case insensitive. The string can contain any char.

```
def xo(s):
    xlist = [char for char in s if (char == "x" or char == "X")]
    olist = [char for char in s if (char == "o" or char == "O")]        
    if len(xlist) == len(olist):
        return True
    else:
        return False
```
