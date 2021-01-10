# Som off?
Moj nastenný WIFI vypínač

## Ako vznikol somoff?
Napad vznikol ako lacnejsie vyriesit chytru domacnost oproti existujucim znackam na trhu, hlavne k spokojnosti.

Vacsina dostupnych blbosti ma vlastnu aplikaciu a len tazko sa dopracujete k tomu, aby ste vsetky prvky ovladali z rovnakej aplikacie a to aj bez pritomnosti internetu. Pouzity material je na baze co mame v dielni odlezane :-) resp. niektore veci si vyzaduju mensiu zrucnost a trpezlivost. Nobelovu cenu za toto asi neziskate, ovsem nezabudajte, ze forma z elektroliecby z 220V moze mat neziaduce nasledky. Takze opatrne s izolovanim kablov.

![Vypinac](https://github.com/rpisoft/somoff/blob/main/images/somoff.jpg)

Relatko zapina GPIO0 na module, ale podla nakresu vidiet, ze je tam este rezeva. Takze na GPIO3 som pripojil TP233 dotykovy senzor. Pretoze relatko ma v sebe zabudovany regulator na 3.3V koli ESP01 kradnut mozeme napatie z neho, Ja som to urobil zo spodnej casti, kde sa pripajkovali kabliky.

![ESP 01](https://github.com/rpisoft/somoff/blob/main/images/ESP-01-ESP8266-pinout-gpio-pin.png)

