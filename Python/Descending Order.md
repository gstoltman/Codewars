## Your task is to make a function that can take any non-negative integer as an argument and return it with its digits in descending order. Essentially, rearrange the digits to create the highest possible number.
```
def descending_order(num):

    intlist = []

    for char in str(num):
        if char.isdigit():
            intchar = int(char)
            intlist.append(intchar)

    intlist = sorted(intlist, reverse=True)

    concatlist = int(''.join(str(number) for number in intlist))
    
    return concatlist
```
