# Intro til NeoPixel - lys

    ```template
let strip = neopixel.create(DigitalPin.P2, 5, NeoPixelMode.RGB)
strip.showColor(neopixel.colors(NeoPixelColors.Blue))
```

## Steg 1 - Hva er NeoPixler ? @showdialog

NeoPixler er en av mange ulike typer programmerbare LED - lys. 

![animert gif av neopixelring](https://d14xnrffmhx4ml.cloudfront.net/1660675041/smarthus-veiledning-neopixelring.gif)

    Inni hvert piksel er en mikroprosessor som kan styre farge og lysstyrke. 
Med riktige kommandoer går det an å lage vakre fargemønstre.



## Steg 2 - Trekk ut USB - ledningen før du begynner å koble! @showdialog
** Viktig! Les dette før du begynner **

    Utstyret kan bli ødelagt om ledningene sklir eller kortslutter, så vær ** helt ** sikker på at det ikke er strøm i systemet når du skal koble til eller fra noe.

## Steg 3 - Hvordan koble lysene til micro: biten @showdialog

![bilde av ledninger koblet på microbit](https://d14xnrffmhx4ml.cloudfront.net/1660675040/smarthus-veiledning-neopixel-ledninger.jpg)

    Fra høyre til venstre skal det være svart på ** GND **, rød på ** 3V **, og så hvit / gul på ** 2 **.


## Steg 4 - Last ned koden

Last ned eksempel - programmet til micro: biten og sjekk om det blir liv i lysene.

```blocks
let strip = neopixel.create(DigitalPin.P2, 5, NeoPixelMode.RGB)
strip.showColor(neopixel.colors(NeoPixelColors.Blue))
```

## Steg 5 - Flott! 

Hvis det ble lys: Hurra! Prøv å forandre fargen på lysene.


## Steg 6 - Analyse av koden @showdialog

Det vi har gjort nå, er å legge inn kode som forklarer micro: biten at den er koblet til en NeoPixel - stripe:

![forklaringsbilde av NeoPixel - koden](https://d14xnrffmhx4ml.cloudfront.net/1661765390/smarthus-veiledning-neopixel-forklaring.png)
    Fra nå av, hver gang vi sier at det skal skje noe med variabelen "**strip" **, vet programmet at det er lyslenken på Pin 2 vi mener, og at den har 5 lys.


## Steg 7 -- Kule greier

I Neopixel - menyen til venstre finner du et knippe kommandoblokker som er fine å starte med.

    Oppdrag: Bruk noen minutter på å pusle sammen blokkene på ulike måter, og lag * kjempefine farger *.

Når du føler deg fornøyd, kan du trykke på "Avslutt / Finish" for å gå tilbake til vanlig MakeCode med flere blokker.

```ghost
let strip = neopixel.create(DigitalPin.P2, 5, NeoPixelMode.RGB)
strip.shift(1)
strip.rotate(1)
strip.setPixelColor(0, neopixel.rgb(255, 255, 255))
strip.show()
strip.clear()
basic.forever(function () {
	
})
basic.forever(function () {
    basic.pause(100)
})

```



> Åpne denne siden på [https://broccolisurprise.github.io/smarthus---intro-til-neopixel-lys/](https://broccolisurprise.github.io/smarthus---intro-til-neopixel-lys/)

## Bruk som utvidelse

Dette kodeområdet kan bli lagt til som en **utvidelse** i MakeCode.

* åpne [https://makecode.microbit.org/](https://makecode.microbit.org/)
* klikk på **Nytt prosjekt**
* klikk på **Utvidelser** i menyen under tannhjulet
* søk etter **https://github.com/broccolisurprise/smarthus---intro-til-neopixel-lys** og importér

## Rediger dette prosjektet ![Bygg statusmerke](https://github.com/broccolisurprise/smarthus---intro-til-neopixel-lys/workflows/MakeCode/badge.svg)

For å redigere dette kodeområdet i MakeCode.

* åpne [https://makecode.microbit.org/](https://makecode.microbit.org/)
* klikk på **Importer** og så på **Importér URL**
* lim inn **https://github.com/broccolisurprise/smarthus---intro-til-neopixel-lys** og klikk på importér

## Forhåndsvisning av blokker

Dette bildet viser blokk-koden fra den siste oppdateringen i hovedgrenen.
Dette bildet kan ta noen minutter å oppdatere.

![En opptegnet visning av blokkene](https://github.com/broccolisurprise/smarthus---intro-til-neopixel-lys/raw/master/.github/makecode/blocks.png)

#### Metadata (brukes for søk, visualisering)

* for PXT/microbit
<script src="https://makecode.com/gh-pages-embed.js"></script><script>makeCodeRender("{{ site.makecode.home_url }}", "{{ site.github.owner_name }}/{{ site.github.repository_name }}");</script>
