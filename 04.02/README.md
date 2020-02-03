# 04.02
## Tunni teemad
### Arvutisüsteemi ja Operatsiooni süsteemi struktuur ja seos
#### Tähtsad punktid
* Arvutisüsteem
* Operatsioonisüsteem
* Operatsioonisüsteemi ülesanded
* Operatsioonisüsteemi osad
* Kasutajate rollid

Nende punktidega tutvu [antud materjalis](http://enos.itcollege.ee/~kloodus/osadmin/Loeng2015/loeng01%20-%20OS%20sissejuhatus.pdf)

## Ülesanded lahendamiseks
### Ettevalmistus
* Kui soovid kasutada oma arvuti, siis paigalda ette [Oracle Virtual Box](https://www.virtualbox.org/)
* Kui kasutad sülearvuti, ära unusta lubada CPU virtualiseerimine, muidu sul ei oleks võimalik virtualiseerida 64-bittilised süsteemid!

### Ülesanne 1 - VM loomine
Loo virtuaalmasin (VM) järgmiste parameetritega:

| tunnus | väärtus | 
| ------------- |:------------------:|
| Masina nimi |  OSA |
| Süsteemi tüüp|  Linux|
| Versioon (Distributiiv) |  Debian, 64 bitti  |
| RAM | 1024 MB | 
| HDD | 8 GB, Dynamically allocated | 
| Network | NAT | 

Masina loomise etapid on [Step1-Step3 antud juhendis](http://www.brianlinkletter.com/installing-debian-linux-in-a-virtualbox-virtual-machine/) 

### Ülesanne 2 - OS Paigaldamine
Paigalda loodud VM-le Debian 10 järgmiste parameetritega:

| tunnus | väärtus | 
| ------------- |:------------------:|
| süsteemi tüüp |ilma graafikat |
| hosti nimi |  osa-omaeesnimi|
| domeeni nimi |  puudub |
| kasutajanimi|  kasutaja|
| kasutaja parool |  qwerty |
| root kasutaja parool | qwerty | 
| kõvakettas |kasutatakse täismahus süsteemi failidele| 
| partitsioneerimine | hetkel ei ole vaja, kõik jagatakse automaatselt süsteemi poolt | 
| paigaldatav tarkvara | SSH ja põhiutiliidid | 

Kus leida ISO fail ja mis moodi toimub paigaldamine - jälgi [antud juhendist](https://www.howtoforge.com/tutorial/debian-minimal-server/)

### Ülesanne 3 - Käsurida
Logi sisse loodud VM-sse eelmises ülesannes määratud kasutaja ja parooli abil.

Tutvu käsurea struktuuriga ja tööpõhimõttega oma süsteemi põhjal. Toetu [antud materjali leheküljele 2-7](https://drive.google.com/file/d/1l1UDSeOPP4GxEyRYEzLorM8NyskDo3ig/view?usp=sharing).

### Ülesanne 4 - Navigatsioon süsteemis
Uuri oma süsteemi failisüsteemi struktuur. Toetu [antud materjali leheküljele 7-12, 19-22](https://drive.google.com/file/d/1l1UDSeOPP4GxEyRYEzLorM8NyskDo3ig/view?usp=sharing).

### Ülesanne 5 - Manipulatsioonid failidega ja kaustadega
Antud ülesanne lahendamiseks tuleb kasutada järgmised käsud
```
pwd, mkdir, touch, nano, more, cp, mv, man
```

Toetu [antud materjali leheküljele 25-32](https://drive.google.com/file/d/1l1UDSeOPP4GxEyRYEzLorM8NyskDo3ig/view?usp=sharing).

1) kontrolli kas oled `kasutaja` kodukataloogis
2) loo `kasutaja` kodukataloogis kaust nimega `osa`
3) loo `osa` kataloogis kaust nimega `yl5`
4) loo `yl5` kataloogis fail nimega `info.orig`
5) sisesta `info.orig` faili sisse järgmine info:
    ```
    Oma Ees ja Perenimi
    Kursuse tähis
    ```
6) ja salvesta antud faili sisu
7) proovi väljastada `info.orig` faili sisu ekraanil ilma tektsiredaktorit
kasutamata
8) proovi kopeerida `info.orig` fail samasse kausta ning koopia faili nimeks on fail nimega `info.cp`
9) proovi nimetada `info.orig` fail `info.originaal` failiks
10) loo `yl5` kataloogis kaust nimega `info_failid`
11) proovi `info.cp` fail `info_failid` kataloogi sisse
12) proovi kustutada `info.originaal` fail

### Ülesanne 6 - Manipulatsioonid failidega ja kaustadega
Antud ülesanne lahendamiseks tuleb kasutada järgmised käsud
```
mkdir, touch, nano, more, cp, mv, rm
```

Toetu [antud materjali leheküljele 25-32](https://drive.google.com/file/d/1l1UDSeOPP4GxEyRYEzLorM8NyskDo3ig/view?usp=sharing).

Kõik järgmised tegevused soorita `kasutaja` kodukataloogis `osa` kataloogis
1) loo `osa` kataloogis kaust nimega `yl6`
2) loo `yl6` kataloogis fail nimega `andmed`
3) sisesta `andmed` faili sisse järgmine info
    ```
    Ees Perenimi
   ```
4) ja salvesta antud faili sisu
5) kontrolli faili sisu - väljasta ekraanil
6) proovi kopeerida `andmed` fail samasse kausta nimega `andmed.cp`
7) proovi nimetada andmed fail `andmed.eespere` failiks
8) loo kataloog nimega `andmed`
9) proovi `andmed.eespere` ja `andmed.cp` liigutada `andmed` kataloogi sisse
10) nimeta ümber kataloog `andmed` - uueks nimeks on `andmed.d`
11) Loo `andmed.d` kataloogi koopia nimega `andmed.d.cp` (miks ei toimi lihtsalt `cp` käsk?)
12) Kustuta `andmed.d` kataloogi sees olevad failid
13) Kustuta `andmed.d` kataloog ka
14) Nimeta `andmed.d.cp` ümber - kataloogi nimeks on `andmed.d`

### Ülesanne 7 - Väljundi filtreerimine ja suunamine
Antud ülesanne lahendamiseks tuleb kasutada järgmised käsud
```
cut, cp, tr, paste
```
1) loo `osa` kataloogis kaust nimega `yl7`
2) Kopeeri `andmed.d` kataloogi fail `andmed.eespere` `yl7` kataloogi sisse
3) Tutvu `cut` käsu võimalustega. Toetu antud materjali leheküljele 282. 
4) Tutuvu suunamisvõimalustega - toetu antud materjali leheküljedele 53-62.
5) Lõika `andmed.eespere` faili väljundist oma `Eesnimi` ja salvesta faili nimega `andmed.ees`
6) Lõika `andmed.eespere` faili väljundist oma `Perenimi` ja salvesta faili nimega `andmed.pere`
7) Tutvu `tr` käsu võimalustega. Toetu antud materjali leheküljele 294.
8) Muuda mõlema loodud faili väljundist suured sümbolid väikesteks ja salvesta tulemused analoogselt failidesse `andmed.ees.v` ja `andmed.pere.v`
9) Tutvu `paste` käsu võimalustega. Toetu antud materjali leheküljele 285.
10) Kleebi `andmed.pere.v` ja `andmed.ees.v` väljundid omavahel kokku, eraldajaks on `.` (punkt) ja tulemus salevesta faili nimega `kasutaja`.

### Ülesanne 8 - Väljundi filtreerimine konveieriga
Antud ülesanne lahendamiseks tuleb kasutada järgmised käsud
```
cut, sort, uniq, wc, |
```

Toetu antud materjali leheküljele 53-62.

1) loo `osa` kataloogis kaust nimega `yl8`
2) Tutvu `/etc/passwd` faili sisuga
3) Lõika 7. väli antud faili sisust, veergude eraldajaks antud failis on `:`
5) Järgmiste punktide lahendamiseks tuleb kasutada konveierit (`|`) 
6) Sorteeri lõigatud sisu tähestiku järjekorras
7) Eemalda väljundist korduvad read
8) Loe kokku, mitu ridu on jäänud väljundis
9) Salvesta tulemus faili nimega `koorikud` (<i>shells</i>)

### Ülesanne 9 - käsurea ajaloo salvestamine
1) Käsureas sisestatud käsude nimekiri on võimalik saada `history` käsu abil. Toetu antud materjali leheküljele 84-85.
2) Salvesta tulemus faili nimega `04.02` `osa`kataloogi.

