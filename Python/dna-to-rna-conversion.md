## Ribonucleic acid, RNA, is the primary messenger molecule in cells. RNA differs slightly from DNA its chemical structure and contains no Thymine. In RNA Thymine is replaced by another nucleic acid Uracil ('U'). Create a function which translates a given DNA string into RNA.

```
def dna_to_rna(dna):
    rnalist = ['U' if i == 'T' else i for i in dna]
    rnastring = ''.join(rnalist)
    return rnastring
```
