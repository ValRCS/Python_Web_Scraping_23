# Dictionaries - Darbs Klasē

## 1. Simbolu biežums

* 1a. Uzrakstīt funkciju: get_char_count(text), kas saņem string un izvada vārdnīcu ar atsevišķu burtu lietojumu skaitu.

get_char_count("hubba bubba") -> {'h': 1, 'u': 2, 'b': 5, 'a': 2, ' ': 1} # vārdnīcas secībai nav nozīme, un visam alfabetam nav jābut

* 1b. Uzrakstīt funkciju: get_digit_dict(num), kas saņem veselu skaitli kā parametru(var būt ļoti liels

funkcija  izvada ciparu izmantojumu skaitlī vārdnīcas formā

Ievada 599637003 -> {'0':2, '1':0,....'7'':1,'8':0,'9':2} # rādam visiem cipariem izmantojamību

Ieverojam ka cipariskās atslēgas ir stringi

PS 1a un 1b var atrisināt ar vienu un to pašu funkciju 1b vajadzībām nedaudz pielāgojot 1a kodu.

 Var būt arī risinājums ar Counter but tas galīgi nav obligāti, lai gan ir ļoti eleganti :)


## 2. Vārdnīcu labotājs

Uzrakstīt replace_dict_value(d, bad_val, good_val), kas atgriež vārdnīcu ar nomainītām vērtībām

Funkcijas parametri ir vārdnīca d, kas jāapstrādā, un vērtības bad_val kura jānomaina uz good_val

replace_dict_value({'a':5,'b':6,'c':5}, 5, 10) -> {'a':10,'b':6,'c':10} , jo 5 bija vērtība, kas jānomaina.


## 3. Vārdnīcu tīrītājs

* 3.a  Uzrakstīt clean_dict_value(d, bad_val), kas atgriež attīrītu vārdnīcu

Funkcijas parametri ir vārdnīca d, kas jāapstrādā, un vērtība  bad_val no kuras jāatbrīvojas kopā ar ar tās atslēgu.

clean_dict_value({'a':5,'b':6,'c':5}, 5) -> {'b':6} , jo 5 bija vērtība gan a gan c atslēgām no kurām jāatbrīvojas.

* 3.b Uzrakstīt clean_dict_values(d, v_list), kas atgriež attīrītu vārdnīcu

Funkcijas parametri ir vārdnīca d, kas jāapstrādā, un vērtību saraksts v_list no kurām jāatbrīvojas.

clean_dict_values({'a':5,'b':6,'c':5}, [3,4,5]) -> {'b':6} , jo 5 bija vieno no vērtībām no kurām jāatbrīvojas.

PS. Tīram mēs are del d['a'] protams tikai tad ja atslēga 'a' eksistē.

!! Mainot vārdnīcas izmēru mēs nedrīkstam vienlaicīgi pa šo vārdnīcu staigāt(iterate)!

Divi varianti: vai nu staigājam pa kopiju my_dict.copy.items(), vai arī būvējam jaunu vārdnīcu.