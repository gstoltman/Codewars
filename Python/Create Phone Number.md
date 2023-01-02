### Write a function that accepts an array of 10 integers (between 0 and 9), that returns a string of those numbers in the form of a phone number.

```
def create_phone_number(n):
    strlist = [str(char) for char in n]
    strlist.insert(6, '-')    
    strlist.insert(3, ' ')
    strlist.insert(3, ')')
    strlist.insert(0, '(')    
    answer = ''.join(strlist)
    return answer
```
