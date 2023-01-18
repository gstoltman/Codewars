## In this kata you are required to, given a string, replace every letter with its position in the alphabet.

## If anything in the text isn't a letter, ignore it and don't return it.

## "a" = 1, "b" = 2, etc.

```
def alphabet_position(text):
    alphabet = 'abcdefghijklmnopqrstuvwxyz'
    alph_list = [i for i in alphabet]
    alph_dict = {i:count+1 for count, i in enumerate(alph_list)}
    value_flipped_list = [str(alph_dict[i]) for i in text.lower() if i.isalpha()]
    value_flipped_list_as_string = ' '.join(value_flipped_list)
    return value_flipped_list_as_string
```
