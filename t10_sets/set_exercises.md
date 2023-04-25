# Sets - kopas - patstāvīgais darbs

## Kopējie Elementi

Uzrakstiet funkciju,kas atgriež tuple ar kopējiem elementiem trijās virknēs. Virknes var būt list,tuple,string.

get_common_elements(seq1,seq2,seq3)

get_common_elements("abc",['a','b'],('b','c')) -> ('b',) # tuple are vienu element šim elementam seko komats

* atceramies, ka mēs varam pārveidot virknes uz set ar set(virkne), un set uz tuple ar tuple(myset)

PS Tiem, kas nav pirmo reizi ar pīpi uz jumta, padomāsim, vai varam uztaisīt funkciju, kas spēj apstrādat patvalīgu skaitu virkņu

##  Vai ir pangramma?

Uzrakstīt funkciju is_pangram, kas atgriež True, kad mytext parametrs satur visus burtus kas padoti a alfabetā.

Savadāk atgriežam False.

pangramma - teikums,vārdu virkne, kas satur visus alfabeta burtus - https://en.wikipedia.org/wiki/Pangram

Atstarpes ignorējam,un uzskatam ka lielais burts ir tikpat derīgs kā mazais, t.i. šeit A un a -> a

```def is_pangram(mytext, a='abcdefghijklmnopqrstuvwxyz'):
    '''
    '''
    return None # here it should return True or False
is_pangram("abcd foo") == False
is_pangram("The quick brown fox jumps over the lazy dog") == True
is_pangram("The five boxing wizards jump quickly") == True #ieverojam lielais T šeit```
PS. ar šo funkciju tad mēs varēsim pārbaudīt arī latviešu vai citu valodu pangramas, padodot a parametrā attiecīgā alfabēta burtus.