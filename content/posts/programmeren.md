---
author:
  name: "Dimitri van Ooik"
date: 2023-4-5
linktitle: Creating a New Theme
type:
- post
- posts
title: Progammeren
weight: 10
series:
- Vakken
---


## Wat ik heb gedaan in python


- Hello world

  het schrijft Hello world
```python
print("Hello world")
```

- Hello User

  Een programma dat de gebruiker om een naam vraagt. 
  En hoi zegt tegen de naam van de gebruiker.
```python
naam = input("wat is je naam?")
print("Hallo", naam)
```

- Dobelspel

    Het dobbelspel is een spell waarbij je 2 spelers hebt die 2 dobbelstenen gooien, en de gene die het hoogst gooit wint of als je twee eenen gooit.
```python
Antwoord = 1
Spelen = 1


while Spelen == 1:
    print("_" * 80)
    a = random.randint(1, 6)
    b = random.randint(1, 6)
    c = random.randint(1, 6)
    d = random.randint(1, 6)

    Speler1 = a + c
    Speler2 = b + d

    if Speler1 == Speler2:
        print("Het is gelijkspel.")
    elif Speler1 == 2:
        print("Speler 1 heeft gewonnen doormiddel van snake eyes")
    elif Speler2 == 2:
        print("Speler 2 heeft gewonnen doormiddel van snake eyes")
    elif Speler1 > Speler2:
        print("Speler 1 heeft gewonnen.")
    elif Speler2 > Speler1:
        print("Speler 2 heeft gewonnen.")

    print("")
    print("Speler 1 heeft", a, "en", c, "gegooid")
    print("Speler 2 heeft", b, "en", d, "gegooid")
    Antwoord = 1

    while Antwoord == 1:
        Spel = input("wil je nog eens spelen? ")
        if Spel == "ja":
            print("Veel plezier met spelen.")
            Antwoord = 2
        elif Spel == "nee":
            print("Fijne dag.")
            Spelen = 2
            Antwoord = 2
        else:
            print("Ik snap niet wat je typte zeg ja of nee alsjeblieft.")

```

- Olympische medailles

    Het genereerd een willekeurig getal, en dat is je plaats en afhankelijk van je plaats krijg je een medaille.
```python
import random

plaats = random.randint(1,5)

if plaats == 1:
    print("Goud")
elif plaats == 2:
    print("zilver")
elif plaats == 3:
    print("Brons")
elif plaats == 4:
    print("Niets!")
elif plaats == 5:
    print("Niets")
```

- Hoger/lager

Het progamma genereerd een willekeurig nummer.   
Dan typ jij een nummer in en dan verteld het programma of het willekeurige getal hoger of lager is totdat je het goed hebt.

```python
import random


def hoger_lager_spel():
    print("welkom bij hoger en lager")
    nummer = random.randint(1, 100)
    while True:
        guess = int(input("raad een nummer tussen de 1 en 100:  "))
        if guess < nummer:
            print("te laag probeer opnieuw.")
        elif guess > nummer:
            print("te hoog probeer opnieuw.")
        else:
            print(f"gefeliciteerd je hebt het nummer geraden")
            break


hoger_lager_spel()
```
