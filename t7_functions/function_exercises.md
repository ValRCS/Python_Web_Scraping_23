# Funkcijas - Darbs Klasē
## 1. Lielais rezultāts

Uzrakstiet funkciju add_mult, kurai nepieciešami trīs parametri/argumenti

Atgriež rezultātu, kas ir 2 mazāko argumentu summa reizināta ar lielāko argumenta vērtību.

PS Uzskatīsim, ka funkcijai vienmēr tiks padoti skaitliski parametri, varam tipus nepārbaudīt.

Iespējami dažādi risinājumi, piemēram ar list struktūru varētu būt tīri eleganti.

Piemērs add_mult(2,5,4) -> atgriezīs (2+4)*5 = 30

## 2. Palindroms

uzrakstiet funkciju is_palindrome(text)

kas atgriež bool True vai False atkarībā vai vārds vai teikums ir lasāms vienādi no abām pusēm.

PS no sākuma varat sākt ar viena vārda risinājumu, bet pilns risinājums ignorēs atstarpes(whitespace) un lielos/mazos burtus

```is_palindrome("Alus ari ira      sula") -> True```

## 3. Pilsēta

Pilsētā ir zināms skaits iedzīvotāju p0

Katru gadu nāk klāt procentuāls skaits perc

Katru gadu nāk klāt(vai aizbrauc) arī zināms skaits delta

Mums ir jāzina, kad(ja vispār) pilsēta sasniegs iedzīvotāju skaitu p

Uzrakstiet funkciju get_city_year(p0, perc, delta, p) kas atgriež gadus (pilnus) kad p tiks sasniegts.

Ja p nevar sasniegt, tad atgriežam -1

### Piemērs:

get_city_year(1000,2,50,1200) -> 3

1000 + 1000 * 0.02 + 50 => 1070 pēc 1.gada

1070 + 1070 * 0.02 + 50 => 1141 pēc 2.gada

1141 + 1141 * 0.02 + 50 => 1213 pēc 3.gada

PS. Ievērojam, ka padodam perc kā procentu kas jāpārvērš decimāl skaitlī.

Pārbaudam, vai strādā ar sekojošiem parametriem:

get_city_year(1000, 2, -50, 5000) -> -1 # samērā aktuāla problēma

get_city_year(1500, 5, 100, 5000) -> 15

get_city_year(1500000, 2.5, 10000, 2000000) -> 10