# Som off?
Vlastný nastenný WIFI vypínač

## Ako vznikol somoff?
Napad vznikol ako lacnejsie vyriesit chytru domacnost oproti existujucim znackam na trhu, hlavne k spokojnosti.

Vačšina dostupných blbostí ma vlastnú aplikaciu a len tažko sa dopracujete k tomu, aby ste všetky prvky ovládali z rovnakej aplikície a to aj bez prítomnosti internetu. Použitý materiál je aj na báze čo mame v dielni odležané :-) resp. niektoré veci si vyžadujú menšiu zručnosť a trpezlivosť. Nobelovu cenu ani certifikát kvality za toto nečakám, urobil som to preto, to lebo to **ide urobiť**, tak sa chcem podeliť so skúsenosťami a tiež rád privítám vylepšenia. Netreba zabúdať, že forma elektroliečby z 220V môže mať aj nežiadúce následky, **takže opatrne s izolovaním káblov**. Rámček vypínača som vytlačil na 3D tlačiarni, ale nič nebráni tomu aby použilo telo aj zo starého vypínača.

![Vypinac](https://github.com/rpisoft/somoff/blob/main/images/somoff.jpg)

Relátko zapina GPIO0 na module, takže na GPIO3 som pripojil TP233 dotykový senzor. Pretože relátko má v sebe zabudovaný regulátor na 3.3V kôli ESP01, kradnúť môzeme napätie rovno z neho, Ja som to urobil zo spodnej časti, kde som pripájkoval kábliky.

![ESP 01](https://github.com/rpisoft/somoff/blob/main/images/ESP-01-ESP8266-pinout-gpio-pin.png)



