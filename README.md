# Som off?
Vlastný nastenný WIFI vypínač

## Ako vznikol somoff?
Napad vznikol ako lacnejsie vyriesit chytru domacnost oproti existujucim znackam na trhu, hlavne k spokojnosti.

Vačšina dostupných blbostí ma vlastnú aplikaciu a len tažko sa dopracujete k tomu, aby ste všetky prvky ovládali z rovnakej aplikácie a to aj bez prítomnosti internetu. Použitý materiál je aj na báze čo máme v dielni odležané :-) resp. niektoré veci si vyžadujú menšiu zručnosť a trpezlivosť. Nobelovu cenu ani certifikát kvality za toto nečakám, urobil som to preto, lebo to **ide urobiť**, tak sa chcem podeliť so skúsenosťami a tiež rád uvítám vylepšenia. Netreba zabúdať, že forma elektroliečby z 220V môže mať nežiadúce následky, **takže opatrne s izolovaním káblov**. Rámček vypínača som vytlačil na 3D tlačiarni, ale nič nebráni tomu aby sa použilo telo aj zo starého vypínača. Princíp asi nie je nutné vysvetľovať, všetko to vopchať do krabice, može sa lokálne prepínať, možnosť nahratia ľubovolného software Lua, Arduino, Tasmota, ESPHome, ESPEasy a ovládať na diaľku.

<img src="https://github.com/rpisoft/somoff/blob/main/images/somoff.jpg" alt="Vypinac" width="320"/><img src="https://github.com/rpisoft/somoff/blob/main/images/need2.jpg" alt="Elektronika" width="320" height="306" /><img src="https://github.com/rpisoft/somoff/blob/main/images/1610343015971.gif" alt="Vypinac" width="320" height="306"/>

Relátko zapina GPIO0 na module, takže na GPIO3 som pripojil TP233 dotykový senzor. Pretože relátko má v sebe zabudovaný regulátor na 3.3V kôli ESP01, kradnúť môzeme napätie rovno z neho, Ja som to urobil zo spodnej časti, kde som pripájkoval kábliky.

![ESP 01](https://github.com/rpisoft/somoff/blob/main/images/ESP-01-ESP8266-pinout-gpio-pin.png)

Pretože súdruhovia vyhůtali modul tak, že miesto bootovania sa má spustiť sériová komunikácia na čipe (podotýkam nešlo to ani keď som to dostal) tak sa musí urobiť menšia kozmetická úprava.
<img src="https://github.com/rpisoft/somoff/blob/main/images/fix5relay1.0.jpg" alt="Relatko"/> 



