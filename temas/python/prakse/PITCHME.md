## Ievads Python

---?color=linear-gradient(90deg, white 50%, black 50%)

@snap[west span-30 text-center]

#### Python valoda

#### repl.it vide

@snapend

@snap[north-east span-60 text-12]
@box[bg-green text-white box-padding](Ievads valodas sintaksē)
@snapend

@snap[east span-60 text-12]
@box[bg-blue text-white box-padding](Salīdzinājums ar JS)
@snapend

@snap[south-east span-60 text-12]
@box[bg-gold text-white box-padding](repl.it vide)
@snapend

---

### Sintakses īpatnības

- Atkāpēm (atstarpēm) ir nozīme ...
- ... jo bloki tiek apzīmēti ar atkāpi
- Piespiež ievērot formatēšanas labo stilu
- Koda redaktora funcionalitāte palīdz

---

## Kā to lietot

+++

@snap[north-west]
#### Datu struktūras
@snapend

```python
vards = "Labrīt, skolotāji!"
skaitlis = 10
masivs = ["viens", 2, "trīs", 3.14]
vardnica = {"diena": 24, "menesis": 10}
pareizi = True
nepareizi = False
nav = None
```

@snap[south span-100 text-10]

@[1](string)
@[2](skaitlis)
@[3](masīvs)
@[4](vardnica)
@[5,6](boolean)
@[7](empty value)
@snapend

+++

@snap[north-west]
#### Operatori
@snapend

```python
a = 1
b = (2 ** 5) - (2 * 2)
dalijums = 12 / 10      # == 1.2
vesela_dala = 12 // 10  # == 1
atlikums = 12 % 10      # == 2
```

@snap[south span-100 text-10]

@[1](piešķir vērtību)
@[2](saskaita, kāpina, atņem, reizina)
@[3](iegūst dalījuma rezultātu kā float)
@[4](iegūst dalījuma veselo daļu kā integer)
@[5](iegūst dalījuma atlikumu kā integer)

@snapend

+++

@snap[west span-50 text-center]
#### Python

```python
# Šis ir komentārs
print("Čau!")
```
@snapend

@snap[east span-50 text-center]

#### JavaScript

```javascript
// Šis ir komentārs
console.log("Čau!");
```

@snapend

+++

@snap[north span-100 text-smallcaps]
### Funkciju definēšana

@snapend

@snap[west span-50]

Python

```python
# definējam funkciju
def sveiciens(vards):
    print("Labrīt, " + vards)

# izsaucam funkciju
sveiciens("Evija")
```
@snapend

@snap[east span-50]

JavaScript

```javascript
// definējam funkciju
function sveiciens(vards) {
    console.log("Labrīt, " + vards);
}
//izsaucam funkciju
sveiciens("Evija");
```
@snapend

---

### Laiks praktizēties !

+++

### repl.it vide

@ul
- nekas nav jāinstalē
- pieejama caur pārlūkprogrammu
- atbalsta dažādas valodas
@ulend

+++

### Atbalsts mācību procesam:
  
@ul
- uzdevumi
- uzdevumu automātiskie testi
- pārbaudes darbi
- klases darba organizācija
@ulend

+++

## Atveram repl.it vietni

### Piesakāmies

+++

BILDE AR PIRMO LAPU

+++

BILDE AAR SETIINGIEM UN ROLES

+++

### Un tagad pabūsim skolēnu ādā

#### repl.it/classroom/join/.....

---

@snap[north span-100 text-smallcaps]
### Zarošanās
@snapend

@snap[west span-50]

Python

```python
def pozitivs(skaitlis):
    if skaitlis > 0:
        return True
    else:
        return False


```
@snapend

@snap[east span-50]

JavaScript

```javascript
function pozitivs(skaitlis) {
    if (skaitlis > 0) {
        return true;
    } else {
        return false;
    }
}
```
@snapend

+++

@snap[north-west]
#### Pilns if-elif-else zarošanās piemērs
@snapend

```python
def dalisana(skaititajs, saucejs):
    if skaititajs == 0:
        return 0
    elif saucejs == 0:
        return "Ar 0 dalīt nedrīkst!"
    else:
        return skaititajs /  saucejs
```

@snap[south span-100 text-10]

@[1](definējam funkciju ar diviem parametriem)
@[2,4,6](zarošanās nosacījumi)
@[2-3](pārbaudam pirmo nosacījumu)
@[4-5](pārbaudam citu nosacījumu)
@[6-7](izpildam visos citos gadījumos)

@snapend

+++

@snap[north-west]
#### Cikli (for .. in range ...)
@snapend

```python
for i in range(5):
    print(i)

for i in range(5, 11):
    print(i)

for i in range(2, 11, 2):
    print(i)
```

@snap[south span-100 text-10]
@[1](Cikls izpildās no 0 (pēc noklusējuma) līdz 4 (5 neieskaitot) ar soli 1)
@[2](Izdrukā 5 skaitļus - 0, 1, 2, 3, 4)
@[4](Cikls izpildās no 5 līdz 10 ar soli 1)
@[7](Cikls izpildās no 2 līdz 10 ar soli 2)
@snapend

+++

@snap[west span-50 text-center]
#### Python

```python
for i in range(5):
  print(i)

```
@snapend

@snap[east span-50 text-center]

#### JavaScript

```js
for (let i = 0; i < 5; i += 1) {
  console.log(i);  
}
```

@snapend

+++

@snap[north-west]
#### Cikli (for .. in ...) ar iterable datu struktūrām
@snapend

```python
vards = "zebra"
for burts in vards:
    print(burts)

masivs = ["viena", "maza", "turku", "pupa"]
for elements in masivs:
    print(elements)

for i in range(len(masivs)):
    print(i, masivs[i])
```

@snap[south span-100 text-10]
@[1,2](Cikls ņems pēc kārtas simbolus no string mainīgā)
@[3](Izdrukā simbolus (burtus) atsevišķi)
@[5,6](Cikls ņems masīva elementus pēc kārtas)
@[7](Izdrukā masīva elementus atsevišķi)
@[9](Var izmantot range un masīva vai string garumu)
@[10](Tādā gadijumā vērtībai jāpiekļūst izmantojot indeksu)
@snapend

+++

@snap[north-west]
#### Cikli (for .. in ...) ar vārdīcu
@snapend

```python
vardnica = {"viens": "one", "divi": "two", "trīs": "three"}

for atslega in vardnice:
    print(atslega, vardnica[atslega])

for atslega, vertiba in vardnica.items():
    print(atslega, vertiba)

```

+++

### Un tagad atkal pabūsim skolēnu ādā

#### repl.it/classroom/join/.....

---

## Darbības ar failiem

+++

#### Failu darbību vispārīgs apskats:

@ul
- atver failu
  - kur atrodas?
  - kāda veida (teksta vai binārs)
  - ko vēlas darīt (lasīt, rakstīt, pievienot)
- veic datu operāciju
  - nolasa
  - ieraksta
- aizver failu
@ulend

+++

### Failu darbības ar Python

```python
with open("dati.txt", "r") as f:
    dati = f.readlines()

for rinda in dati:
    print(rinda)
```

@snap[south span-100 text-10]
@[1](atver failu, norādot faila vārdu un atvēršanas veidu)
@[2](ielasa teksta faila saturu masīvā)
@[3](with bloks beidzies, fails tiek automātiski aizvērts)
@[4,5](dati ir pieejami, izdrukā teksta faila saturu)
@snapend

+++

```python
with open("jauns.txt", "w") as jauns:
    jauns.write("Izveidoju jaunu failu!")
```

```python
with open("jauns.txt", "a") as klaat:
    klaat.write("\nPievienoju jaunu rindiņu!\n)
```

```python
with open("bilde.png", "rb") as bilde:
    # kaut ko ar bināru failu ...
```

+++

### Darbības ar teksta failiem

@ul
- vienkārši teksta faili - *.txt
- tabulāri dati, atdalīti ar simbolu - *.csv
- formatēti dokumenti - *.doc
- web lapas - *.html
- json dokumenti - *.json
@ulend

+++

### *.txt

@ul
- var vienkārši lasīt izmantojot iebūvēto funkcionalitāti
- rindas ior atdalītas ar "\n"
- rakstot "\n" ir jāpievieno, ja grib jaunu rindu
@ulend
