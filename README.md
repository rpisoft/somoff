# Som off?
Vlastný nastenný WIFI vypínač

## Ako vznikol somoff?
Nápad vznikol ako lacnejšie vyriešit chytrú domacnosť oproti existujúcim značkám na trhu, ale hlavne k spokojnosti.

Vačšina dostupných blbostí ma vlastnú aplikaciu a len tažko sa dopracujete k tomu, aby ste všetky prvky ovládali z rovnakej aplikácie a to aj bez prítomnosti internetu. Použitý materiál je aj na báze čo máme v dielni odležané :-) resp. niektoré veci si vyžadujú menšiu zručnosť a trpezlivosť. Nobelovu cenu ani certifikát kvality za toto nečakám, urobil som to preto, lebo to **ide urobiť**, tak sa chcem podeliť so skúsenosťami a tiež rád uvítám vylepšenia. Netreba zabúdať, že forma elektroliečby z 220V môže mať nežiadúce následky, **takže opatrne s izolovaním káblov**. Rámček vypínača som vytlačil na 3D tlačiarni, ale nič nebráni tomu aby sa použilo telo aj zo starého vypínača. Princíp asi nie je nutné vysvetľovať, všetko to vopchať do krabice, može sa lokálne prepínať, možnosť nahratia ľubovolného software Lua, Arduino, Tasmota, ESPHome, ESPEasy a ovládať na diaľku.

<img src="https://github.com/rpisoft/somoff/blob/main/images/somoff.jpg" alt="Vypinac" width="320"/><img src="https://github.com/rpisoft/somoff/blob/main/images/need2.jpg" alt="Elektronika" width="320" height="306" /><img src="https://github.com/rpisoft/somoff/blob/main/images/1610343015971.gif" alt="Vypinac" width="320" height="306"/>

## Ako na to?
Relátko zapina GPIO0 na module, takže na GPIO3 som pripojil TP233 dotykový senzor. Pretože relátko má v sebe zabudovaný regulátor na 3.3V kôli ESP01, kradnúť môzeme napätie rovno z neho, Ja som to urobil zo spodnej časti, kde som pripájkoval kábliky.

![ESP 01](https://github.com/rpisoft/somoff/blob/main/images/ESP-01-ESP8266-pinout-gpio-pin.png)

Pretože súdruhovia vyhůtali modul tak, že miesto bootovania sa má spustiť sériová komunikácia na čipe (podotýkam nešlo to ani keď som to dostal) tak sa musí urobiť menšia kozmetická úprava. Ak máte šťastie, tak dostanete relátko s modrou led a tak vypínač môže žiariť národnými farbami (biela, červená, modrá) a ak nie aj tak sa svet nezrúti.
<img src="https://github.com/rpisoft/somoff/blob/main/images/fix5relay1.0.jpg" alt="Relatko"/> 

## Potrebné veci
* [Mini 5v AC-DC zdroj](https://techfun.sk/produkt/ac-dc-napatovy-zdroj/)
* [ESP-01 modul](https://techfun.sk/produkt/wifi-modul-esp8266/)
* [USB adapter na programovanie](https://techfun.sk/produkt/esp8266-serial-wifi-adapter/)
* [5v Relatko](https://rlx.sk/sk/iot-the-internet-of-things/6227-esp8266-esp-01esp-01s-relay-wifi-smart-control-module-for-arduinoraspberry-pi-er-esp11002r.html)
* [Kábliky 10 cm](https://techfun.sk/produkt/kabliky-40-kusov-10-cm-m-f/)
* [Dotykový modul TP223](https://techfun.sk/produkt/kapacitne-dotykove-tlacidlo-ttp223/)
* [Tavné tyčinky](https://techfun.sk/produkt/napln-do-tavnej-pistole/)
* [Tavná pištoľ](https://techfun.sk/produkt/tavna-pistol-40w-s-606/)
* [Cin](https://techfun.sk/produkt/cin-13g-0-8-mm/)
* [Pajka](https://techfun.sk/produkt/hrotova-spajkovacka-60w-s-nastavitelnou-teplotou/)
* Svrkovnica
* Kábel 0,75mm
* Obojstranné lepiaca páska



