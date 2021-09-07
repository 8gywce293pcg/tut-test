### @explicitHints false

## Introduksjon @unplugged
Her vil du lære å kode våre kule LED displayer til å vise en regnbue!


## Steg 1: Definer noen neopixler @fullscreen
 Trykk på ``||Neopixel||`` fra blokkmenyen.

 Klikk og dra inn blokken ``||sett strip til||`` og slipp den inni ``||basic:ved start||`` blokken
 Sett pin til ``||P0||`` og antall LED til ``||768||`` la format stå som ``||RGB (GRB)||``.
```blocks
let strip = neopixel.create(DigitalPin.P0, 768, NeoPixelMode.RGB)
```


## Steg 2: Still inn lysstyrken
Trykk på ``||Mer||`` fra blokkmenyen.

Klikk og dra inn blokken ``||strip.setBrightness(255)||`` plasser den nederst og sett verdien til ``||50||``.
```blocks
let strip = neopixel.create(DigitalPin.P0, 768, NeoPixelMode.RGB)
strip.setBrightness(50)
```
## Viktig! @unplugged
Har du satt brightness verdien til ``||50||``? Hvis verdien er over ``||50||`` kan Displayet slutte å fungere.

## Steg 3: Lag en regnbue
Trykk på ``||Neopixel||`` fra blokkmenyen.

Klikk og dra inn blokken ``||strip.showRainbow||`` plasser den nederst og sett verdiene fra ``||1||`` til ``||768||`` 
```blocks
let strip = neopixel.create(DigitalPin.P0, 768, NeoPixelMode.RGB)
strip.setBrightness(50)
strip.showRainbow(1, 768)
```

## Steg 4: Send informasjon til Neopixlene
Trykk på ``||Neopixel||`` fra blokkmenyen.

 Klikk og dra inn blokken ``||strip.show()||`` plasser den nederst.
```blocks
let strip = neopixel.create(DigitalPin.P0, 768, NeoPixelMode.RGB)
strip.setBrightness(50)
strip.showRainbow(1, 768)
strip.show()
```

## Steg 5
Trykk ``|Last ned|`` for å teste koden din på LED Displayet!