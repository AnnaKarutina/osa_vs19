# 11.02
## Tunni teemad
### Failisüsteemi struktuur, otsing failisüsteemis ja väljundites
#### Tähtsad punktid
* Failisüsteemi metamärgid
* Otsing failisüsteemis
* Otsing väljundites

Nende punktidega tutvu [antud materjalis](http://enos.itcollege.ee/~kloodus/osadmin/Loeng2015/loeng01%20-%20OS%20sissejuhatus.pdf)

## Ülesanded lahendamiseks

### Ülesanne 10 - Kordamine
1) Korda failisüsteemis struktuuri ja kasutatavad failide tüübid toetudes [antud materjalile](https://tldp.org/LDP/intro-linux/html/sect_03_01.html)
2) Kontrolli, millised failisüsteemi põhikataloogid olemas ka sinu masinas
3) Kontrolli, millised failisüsteemi põhikataloogid on puudu sinu masinas

### Ülesanne 11 - Metamärgid
Antud ülesanne lahendamiseks tuleb kasutada järgmised käsud
```
mkdir, touch, ls
```
Toetu [antud materjali leheküljele 25-27](https://drive.google.com/file/d/1l1UDSeOPP4GxEyRYEzLorM8NyskDo3ig/view?usp=sharing).

1) loo `osa` kataloogis kaust nimega `yl11`
2) loo `yl11` kaustas järgmiste nimedega failid:  `siga`, `lehm`, `lammas`, `kana`, `kukk`, `kass`, `hiireke`, `koer`, `part`, `hobune`, `.karbes`, `.sipelgas`

Kasutades `ls` käsu ja metamärkide kombinatsioonid:
3) Näita kõik failid, mis algavad `l`-ga
4) Näita kõik failid, mis algavad `k`-ga
5) Näita kõik failid, mis lõpevad `s`-ga
6) Näita kõik failid, mis algavad `k`-ga ja lõpevad kas `a`-ga või `k`-ga
7) Näita kõik failid, mille nimi on `4`-sümboline, `5`-sümboline jne
8) Näita kõik failid, mis algavad `.`-ga

### Ülesanne 12 - Metamärgid
Antud ülesanne lahendamiseks tuleb kasutada järgmised käsud
```
mkdir, touch, ls, cp, mv
```
Toetu [antud materjali leheküljele 25-27](https://drive.google.com/file/d/1l1UDSeOPP4GxEyRYEzLorM8NyskDo3ig/view?usp=sharing).

1) loo `osa` kataloogis kaust nimega `yl12`
2) loo `yl12` kaustas järgmiste nimedega failid:  `fail1`, `fail2`, `fail3`, `fail4`, `fail10`, `fail12`, `Ptk1.txt`, `ptk2.txt`, `ptk3`, `Ptk4`, `.login`

Kasutades sobiliku käsu ja metamärkide kombinatsioonid:
3) Näita nende hulgas kõik failid, mille nimed algavad `f`-ga
4) loo yl10 kataloogis kaust nimega `kataloog`
4) Näita nende hulgas kõik failid, mille nimed lõpevad täpselt ühe numbriga. Proovi ühe käsuga metamärkide abil kopeerida kõik need failid `kataloog` kausta sisse. 
5) Näita nende hulgas kõik failid, mille nimed lõpevad täpselt kahe numbriga. Proovi ühe käsuga metamärkide abil liigutada kõik need failid `kataloog` kausta sisse.
6) Näita nende hulgas kõik failid, mille nimed algavad suure või väikese p-ga. Proovi ühe käsuga metamärkide abil kopeerida kõik need failid `kataloog` kausta sisse.
7) Näita nende hulgas kõik failid, mille nimed algavad suure või väikese `p`-ga ja lõpevad `txt`-ga. Proovi ühe käsuga metamärkide abil kopeerida kõik need failid `kataloog` kausta sisse.
8) Näita nende hulgas ainult `.login` fail.

### Ülesanne 13 - Otsing failisüsteemis
Antud ülesanne lahendamiseks tuleb kasutada järgmised käsud
```
find
```

Toetu [antud materjali leheküljele 213-229](https://drive.google.com/file/d/1l1UDSeOPP4GxEyRYEzLorM8NyskDo3ig/view?usp=sharing).

1) Otsi kõik elemendid `/usr` kaustas, mis lõpevad `.txt` laiendiga
2) Väljasta, mitu on elemendi leidsid eelmises punktis (arvesta, et iga leitud elemendi kirjeldamiseks on üks rida väljundis)
3) Otsi kõik elemendid `/usr` kaustas, mis lõpevad `.html` laiendiga
4) Väljasta, mitu on elemendi leidsid eelmises punktis
5) Otsi kõik elemendid `/etc` kaustas, mis lõpevad `.d` laiendiga
6) Väljasta, mitu on elemendi leidsid eelmises punktis
3) Mitu on `.d` lõpuga faile `/etc` kaustas?
4) Mitu on `.d` lõpuga kataloogi `/etc` kaustas?


### Ülesanne 14 - Otsing failisüsteemis
Antud ülesanne lahendamiseks tuleb kasutada järgmised käsud
```
find
```

Toetu [antud materjali leheküljele 213-229](https://drive.google.com/file/d/1l1UDSeOPP4GxEyRYEzLorM8NyskDo3ig/view?usp=sharing).

1) loo `osa` kataloogis kaust nimega `yl14`
2) Otsi kõik elemendid `/usr` kaustas, mis lõpevad `.html` laiendiga ja kopeeri need `yl14` kataloogi sisse
3) Mitu elemendi leidsid ja mitu sai kopeeritud. Proovi ära seletada põhjus.

### Ülesanne 15 - Otsing väljundis
Antud ülesanne lahendamiseks tuleb kasutada järgmised käsud
```
wget, grep
```

Toetu [antud materjali leheküljedele 205 ja 247-264](https://drive.google.com/file/d/1l1UDSeOPP4GxEyRYEzLorM8NyskDo3ig/view?usp=sharing).

1) loo `osa` kataloogis kaust nimega `yl15`
2) lae alla antud kataloogi sisse fail [http://anna.ikt.khk.ee/anna.karutina/osa/database](http://anna.ikt.khk.ee/anna.karutina/osa/database)

Antud faili sisu struktuur:

* 1.veerg - müügiosakonna paiknemine
* 2.veerg - müügiosakonna paiknemine (initsiaalide kujul)
* 3.veerg - müügiosakonna juhataja
* 4.-7.veerud - erinevad numbrid - komaga ja täisarvud, mis tähistavad mingid 

3) Leia kõik read, kus on olemas `NW`
4) Leia kõik read, mis algavad väikese `n` tähega (kooli arvutite klaviatuuril `^` märk on `AltGr + Ä` ja tühik)
5) Leia kõik read, mis lõpevad numbriga `4`
6) Leia read, kus olemas `TB Savage` müügsijuhi osakonna kirjeldus
7) Leia kõik read, kus olemas number punktiga `5.`
8) Leia kõik read, kus olemas `.5`
9) Leia read, mis algavad kas `w`-ga või `e`-ga
10) Leia read, kus esineb 2 suvalit suurt tähti, tühik, 1 suur täht
11) Leia kõik read, kus olemas suvaline väike täht, mis korratakse 9 korda järjest

### Ülesanne 16 - Otsing väljundis ja `grep` käsu vajalikud võtmed
Antud ülesanne lahendamiseks tuleb kasutada järgmised käsud
```
grep
```

Toetu [antud materjali leheküljedele 247-264](https://drive.google.com/file/d/1l1UDSeOPP4GxEyRYEzLorM8NyskDo3ig/view?usp=sharing).

1) loo `osa` kataloogis kaust nimega `yl16`
2) lae uuesti alla antud kataloogi sisse fail [http://anna.ikt.khk.ee/anna.karutina/osa/database](http://anna.ikt.khk.ee/anna.karutina/osa/database)
1) Leia read, mis algavad `south` sõnaosaga, väljasta lisaks reale ka `rea number`
2) Leia read, kus `pat` võib olla kas suurte või väikeste tähtedega kirjas
3) Leia read, kus ei esine `Suan Chin`
4) Leia, mitu on rida, mis sisaldavad sõnaosa `west`
5) Leia read, kus `north` on eraldi sõna
 
### Ülesanne 17 - Otsing väljundis ja `grep` käsu vajalikud võtmed
Antud ülesanne lahendamiseks tuleb kasutada järgmised käsud
```
wget, grep
```

Toetu [antud materjali leheküljedele 247-264](https://drive.google.com/file/d/1l1UDSeOPP4GxEyRYEzLorM8NyskDo3ig/view?usp=sharing).

1) loo `osa` kataloogis kaust nimega `yl17`
2) lae uuesti alla antud kataloogi sisse fail [http://anna.ikt.khk.ee/anna.karutina/osa/datebook](http://anna.ikt.khk.ee/anna.karutina/osa/datebook)

Antud faili struktuuri kohta:
* see on tabel, kus veerud on eraldatud `:` märgiga
* `Eesnimi Perenimi:telefon:aadress:sünnikuupäev:tulu`
* antud failis sünnikuupäev on kujul `KK/PP/AA`

3) Leia kõik read, mis sisaldavad `Sun`-iga
4) Leia kõik read, mis algavad `J`-st
5) Leia kõik read, mis lõpevad `700`-ga
6) Leia kõik read, mis sisaldavad detsembris olev sünnikuupäev
7) Leia kõik read, kus telefoninumbrid algavad `408`-ga
8) Leia kõik read, kus olemas järgmine sümbolite järjend: 
`suur täht, 4 väikest tähti, koma, tühik, suur täht`
9) Leia kõik read, kus perenimi algab kas `K` või `k` tähega
10) Leia kõik read, kus tulu koosneb täpselt `6`-st numbrist
11) Väljasta eelmises punktis leitud read koos reanumbriga
12) Leia kõik read, mis sisaldavad `Lincoln` või `lincoln`


### Ülesanne 18 - käsurea ajaloo salvestamine
1) Käsureas sisestatud käsude nimekiri on võimalik saada `history` käsu abil. Toetu [antud](https://drive.google.com/file/d/1l1UDSeOPP4GxEyRYEzLorM8NyskDo3ig/view?usp=sharing)] materjali leheküljele 84-85.
2) Salvesta tulemus faili nimega `11.02` `osa` kataloogi.

