[Link na originálne zadanie.](http://www.dcs.fmph.uniba.sk/~lukotka/pts2017du2.htm)

```
Domácu úlohu odovzdajte ako GITovský repozitár e-mailom na relatko@gmail.com. Do subjectu napiste
PTS DU2. Nezabudnite napisat svoje meno. Termín na odovzdanie úlohy je 4.4.2017 23:00

Naprogramujte terminálové "Človeče nehnevaj sa!". Môžte si upraviť pravidlá. Odporúčané úpravy
(zjednoduženia): po hodení 6-ky hr=ač nehádže ešte raz, po obkrúžení kolečka panáčikovia nejdu do
"domčeka", ale sa točia daľej (teda domček ani neexistuje). Program taktiež nemusí byť úplne user
friendly. Aktuálny stav hry má byť uložený ako jedna imutable premenná, a referencia na tento stav
má byť v podstate jedinou "verejnou" mutovatelnou premennou v programe. To samozrejme neznamená, že
v kóde nemajú byť mutable premenné, takéto premenné však majú existovať iba v lokálnom scope.
Súčasťou odovzdaného repozitára má byť základná používateľská dokumentácia, stručný popis designu a
aspoň základné testovacie programy. Ako si napríklad máte predstaviť terminálové človeče

Player 2 is on turn.
Dice: 4.
Player 0's pieces are on fields: 0:40 1:41 2:42 3:43
Player 1's pieces are on fields: 0:44 1:45 2:46 3:47
Player 2's pieces are on fields: 0:48 1:49 2:50 3:51
Player 3's pieces are on fields: 0:52 1:53 2:54 3:30
>pass
>throw
Player 3 is on turn.
Dice: 5.
Player 0's pieces are on fields: 0:40 1:41 2:42 3:43
Player 1's pieces are on fields: 0:44 1:45 2:46 3:47
Player 2's pieces are on fields: 0:48 1:49 2:50 3:51
Player 3's pieces are on fields: 0:52 1:53 2:54 3:30
>move 3
Player 0 is on turn.
Dice: 0.
Player 0's pieces are on fields: 0:40 1:41 2:42 3:43
Player 1's pieces are on fields: 0:44 1:45 2:46 3:47
Player 2's pieces are on fields: 0:48 1:49 2:50 3:51
Player 3's pieces are on fields: 0:52 1:53 2:54 3:35
```

### PTS 2017 - DU1

Kliknite na link na originálne zadanie. Toto je nadpis tej stránky (ten v hlavičke okna).

### ...(zjednoduženia): po hodení 6-ky hr=ač...

V zadaní je veľa preklepov a gramatických chýb, tu len poukážem na dve krásne. Ako sa vôbec dá
prehliadnuť to rovn=a sa?

### Aktuálny stav hry má byť uložený ako jedna imutable premenná, a referencia na tento stav má byť v podstate jedinou "verejnou" mutovatelnou premennou v programe.

Hm, takže stav má byť uložený v immutable premennej (btw, majú tam byť dve M)? Jednej? Takže máme
jeden immutable stav? A máme naňho mať referenciu? Mutable? Načo je mutable, keď stav je len jeden?
Či stav má byť mutable?

OK, chápem, týmto chcelo byť povedané, že máme mať jednu **mutable premennú obsahujúcu referenciu na
stav**. Stav nie je **immutable premenná**, lebo to nedáva zmysel, stav je len **immutable
hodnota**. Čiže musíme swapovať stavy. Takto naformulované to už dáva zmysel, ale vyžadovalo to istú
davku dôvtipu a empatie.

Ak ctený čitateľ nechápe, o čom som to trepal v predchádzajúcom odstavci, tak to znamená, že som
lepší ako ctený čitateľ.

### Player 0 is on turn.\nDice: 0.

Toto je výstrižok z ukážkovej hry úplne nehrateľného terminálového človeče. Na kocke padla nula.
Enough said. Not enought said. Player 0 is on turn. English 101.

### Zmysel

Čo nám táto úloha má dať? Naprogramuje to každý za najviac dve hodiny a nič sa pri tom nenaučí. Kto
to nenaprogramuje nepatrí na MATFYZ. Kto sa z toho niečo naučí, musel robiť niečo navyše, niečo, čo
zadanie v skutočnosti nepožadovalo, ale on je dostatočne cieľavedomý, aby to niečo navyše spravil.

Alebo sme sa mali naučiť používať jednu mutable/imutable/mutable/imutable/mutable/imutable...