[Link na originálne zadanie.](http://www.dcs.fmph.uniba.sk/~lukotka/pts2017du1.htm)

```
Program uchovĂˇva zoznam uÄŤastnĂ­kov a ich aktuĂˇlny stav bodov v sĂştaĹľi.
Po spustenĂ­ si program od uĹľĂ­vateÄľa vypĂ˝ta heslo. Potom program ÄŤakĂˇ na prĂ­kazy od uĹľĂ­vateÄľa,
ktorĂ© nĂˇsledne vykonĂˇ.

Zoznam prĂ­kazov:

points <name> <number>
  PridĂˇ hrĂˇÄŤovi <name> <number> bodov. ÄŚĂ­slo mĂ´Ĺľe byĹĄ aj zĂˇpornĂ©.
  Ak hrĂˇÄŤ <name> eĹˇte nie je evidovanĂ˝ pridĂˇ ho do zoznamu s <number> bodmi.

reduce <number>
  ZnĂ­Ĺľi poÄŤet bodov kaĹľdĂ©ho hrĂˇÄŤa o <number>%. VĂ˝sledok sa zaokrĂşhli na celĂ© ÄŤĂ­sla nadol.

junior <name> 
  OznaÄŤĂ­, Ĺľe hrĂˇÄŤ <name> je junior

ranking 
  VypĂ­Ĺˇe celĂ© poradie. HrĂˇÄŤov zoradĂ­me podÄľa poÄŤtu bodov.

ranking junior
  VypĂ­Ĺˇe poradie medzi juniormi.

quit
  UkonÄŤĂ­ program.


Ak uĹľĂ­vateÄľ zadĂˇ prĂ­kazy points, reduce, category, a quit systĂ©m si najprv vypĂ˝ta password
a prĂ­kaz vykonĂˇ iba v prĂ­pade, Ĺľe password je sprĂˇvny. 
```

### Toto som zbadal na stránke. Nemyslím si, že to je problém len môjho prehliadača.

OK, takže keď si .txt zadanie stiahneme, tak už to vyzerá normálne.

```
Program uchováva zoznam učastníkov a ich aktuálny stav bodov v sútaži.
Po spustení si program od užívateľa vypýta heslo. Potom program čaká na príkazy od užívateľa,
ktoré následne vykoná.

Zoznam príkazov:

points <name> <number>
  Pridá hráčovi <name> <number> bodov. Číslo môže byť aj záporné.
  Ak hráč <name> ešte nie je evidovaný pridá ho do zoznamu s <number> bodmi.

reduce <number>
  Zníži počet bodov každého hráča o <number>%. Výsledok sa zaokrúhli na celé čísla nadol.

junior <name> 
  Označí, že hráč <name> je junior

ranking 
  Vypíše celé poradie. Hráčov zoradíme podľa počtu bodov.

ranking junior
  Vypíše poradie medzi juniormi.

quit
  Ukončí program.


Ak užívateľ zadá príkazy points, reduce, category, a quit systém si najprv vypýta password
a príkaz vykoná iba v prípade, že password je správny. 
```

### Po spustení si program od užívateľa vypýta heslo.

Čo to znamená? Vypýta si nové heslo, ktoré bude používať po zvyšok svojho behu? Alebo sa pokúsi o autentifikáciu, teda, opýta sa užívateľa na heslo, aby dokázal, že ho vie? Nikto nevie.

### Ak užívateľ zadá príkazy points, reduce, category...

Príkaz `category` neexistuje.

### Záver

Toto zadanie má prekvapivo málo nedostatkov.