# IOT: onderzoeksrapport Bluetooth & Bluetooth Low Energy

![BLUETOOTH](https://simpeleuitleg.nl/images/artikelen/48_1.jpg "Bluetooth Picture")

Bluetooth is een open standaard voor draadloze verbindingen tussen apparaten op korte afstand. Dankzij bluetooth kunnen bijvoorbeeld adresgegevens tussen mobiele telefoons worden uitgewisseld, kan snel vanaf een handheld computer worden geprint, of kan een mobiele telefoon worden uitgerust met een draadloze headset.


## Ontstaan Bluetooth

Het Zweedse bedrijf Ericsson ontwikkelde in 1994 de toepassing Bluetooth. Met deze toepassing kunnen verschillende apparaten, bijvoorbeeld mobiele telefoons, over een korte afstand verbinding met elkaar maken. Met Bluetooth kunnen bijvoorbeeld adresgegevens of ringtones tussen mobiele telefoons worden uitgewisseld.

Het Zweedse bedrijf Ericsson dat de toepassing ontwikkelde besloot een oude Deense koning te eren: Harald Blauwtand (ca. 910-986).

Deze Harald werd in 940 koning van de Denen, verenigde veel elkaar bestrijdende stammen en heerste ook enige tijd over Noorwegen.

In Scandinavië is hij onder meer bekend omdat hij de verspreiding van het christendom hier bevorderde. De toepassing werd naar deze koning vernoemd: Bluetooth is Engels voor Blauwtand.

## Werking van Bluetooth

Bluetooth-netwerk bestaat uit een Personal Area Network (PAN) of een piconet dat minimaal 2 tot maximaal 8 Bluetooth-peer-apparaten bevat - meestal een enkele master en maximaal 7 slaves. 
Een master is het apparaat dat communicatie met andere apparaten initieert. Het master-apparaat regelt de communicatieverbinding en het verkeer tussen zichzelf en de daarmee verbonden slave-apparaten. Een slave-apparaat is het apparaat dat reageert op het master-apparaat. Slave-apparaten moeten hun zend- / ontvangsttijdstip synchroniseren met die van de meesters. 

Bovendien worden transmissies door slave-apparaten beheerd door het master-apparaat (dwz het master-apparaat dicteert wanneer een slave-apparaat mag verzenden). In het bijzonder mag een slaaf alleen met zijn uitzendingen beginnen in een tijdslot onmiddellijk volgend op het tijdslot waarin het door de meester werd geadresseerd,

![BLUETOOTH](https://www.elprocus.com/wp-content/uploads/2013/08/Bluetooth.png "Bluetooth Diagram Picture")

De frequentiehoppenreeks wordt bepaald door het Bluetooth-apparaatadres (BD_ADDR) van het masterapparaat. Het master-apparaat verzendt eerst een radiosignaal waarin binnen de reeks adressen om respons van de specifieke slave-apparaten wordt gevraagd. De slaven reageren en synchroniseren hun hopfrequentie en klok met die van het masterapparaat.

## Verschillende versies

Bluetooth is doorheen de jaren enorm verbeterd en vooral nog veelzijdiger gemaakt. Momenteel zitten we aan Bluetooth 5.0. De verschillende versies vereisen telkens nieuwe chips, dus het is niet zo dat je Bluetooth kunt updaten. 

![BLUETOOTH](https://www.tabletsmagazine.nl/wp-content/uploads/2016/08/bluetooth-5-770x300.jpg "Bluetooth 5.0 picture")

De laatste versies zijn vooral aangepast voor IoT- en smarthome-toestellen. 
Een belangrijke verbetering kwam er in versie 4.0 of _Bluetooth Low Energy_, toen een nieuwe, zuinige modus werd geïntroduceerd. Deze zorgt er bijvoorbeeld voor dat Bluetooth-toestellen veel zuiniger werken, vooral als ze niet actief gebruikt worden.

Hoewel bluetooth een standaard is, zijn er feitelijk twee soorten bluetooth: Basic Rate (BR) en Low Energy (LE). Het klassieke BR heeft een snelheid van 721,2 Kbit/s en is in versie 2.0 uitgebreid met het optionele EDR dat een snelheid van 2.1 Mbit/s mogelijk maakt. Daarnaast kan door het klassieke bluetooth sinds versie 3.0 optioneel een veel hogere snelheid van 24 Mbit/s gebruikt worden. De data wordt dan niet via de bluetooth-verbinding, maar via een 802.11-verbinding verzonden. Dit is de radiotechnologie die ook voor wifi gebruikt wordt.

## Bluetooth Low Energy

Bluetooth Low Energy (BLE) is een draadloze technologie die de afgelopen jaren enorm populair is geworden in de categorie WPAN (Wireless Personal Area Network) en is inmiddels een standaardtechnologie geworden. Bluetooth Low Energy was beschikbaar om deze superioriteit te bereiken over andere WPAN’s (ZigBee, IEEE802.15.4 etc.) vanwege zijn drie verschillende voordelen:

- Laag vermogensverbruik
- Mobile App Connectivity
- Gratis gateway naar het Internet

### Werking van BLE

De Electronic Product Code in de chip is meestal een 96-bits datastring. De eerste 8 bits van deze string vormen de header. In de header staat omschreven welk protocol er gebruikt wordt. De volgende 28-bits identificeren de organisatie welke de data op de tag beheerd. De organisatie is gekoppeld aan een ID nummer uitgegeven door de GS1. Dit nummer staat in deze 28-bits. De volgende 24-bits vormen de “object-class”. De “object-class” identificeert het type product. De laatste 38-bits vormen dan het unieke nummer voor tag.

![BLUETOOTH](https://meuleman.io/wp-content/uploads/2017/08/BLE-diagram-e1501846951397.png "Bluetooth Low Energy")


## Laag vermogensgebruik

Draadloze communicatie heeft altijd de neiging om veel energie te verbruiken tijdens het verzenden en ontvangen van data. Met een groot energieverbruik zijn veel batterijen nodig om deze apparaten te voeden. Dit is vaak het knelpunt bij het ontwerpen van kleine draadloze apparaten. Bluetooth Low Energy is ontworpen om dit probleem aan te pakken. De belangrijkste reden voor het ontwerp van het BLE-protocol is het lage energieverbruik, zodat draadloze apparaten kunnen worden gevoed door kleine knoopcelbatterijen en daarnaast ook nog eens jarenlang mee kunnen gaan.

### Temperatuursensor met Bluetooth Low Energy

We geven een voorbeeld om te laten zien hoe energiezuinig Bluetooth Low Energy is. Neem een temperatuursensor met BLE die ergens geplaatst is in een slaapkamer. Deze sensor stuurt elke minuut de temperatuur door via Bluetooth Low Energy naar elk BLE-apparaat in de buurt, zoals een tablet, mobiel, pc of een ander apparaat. Dit betekent dat de sensor dagelijks 60 x 24 = 1440 berichten moet sturen.

Voor een temperatuursensor is dat heel vaak, aangezien de temperatuur zelden zo snel verandert in een slaapkamer. Met deze frequenties zou een BLE-transceiver een gemiddeld stroomverbruik van ongeveer 6 uA verbruiken. Dus met een knoopcelbatterij van 620 mAh halen we een theoretische levensduur tot wel 12 jaar! Als de sensor de temperatuur elke seconde verstuurt, dus dagelijks dus 86.400 berichten, dan gaat het toestel nog steeds 2,3 jaar mee!

##  Mobiele App Connectiviteit 

Naast het feit dat Bluetooth Low Energy energiezuinig, is het andere voordeel het gemak waarmee draagbare apparaten draadloos aan elkaar gekoppeld kunnen worden, zoals mobiele telefoons en tablets. De meeste draagbare apparaten worden tegenwoordig uitgerust met BLE-technologie en daarmee kunnen ze direct worden verbonden met elk ander BLE-apparaat. Bovendien kan door middel van mobiele apps (iPhone / Android), eenvoudig en toegankelijk data uit BLE-apparaten worden gevisualiseerd en kan het apparaat worden geconfigureerd.

### Thermostaat met Bluetooth Low Energy

Laten we het eerste voorbeeld uitbreiden naar een thermostaat. Via een mobiele app kunnen we met Bluetooth Low Energy eenvoudig de temperatuur bekijken en de kamertemperatuur aanpassen wanneer we in de kamer zijn. Wanneer we de kamer binnenlopen kan de mobiele app eenvoudig verbinding maken met de thermostaat en de temperatuurwaarde continu meten. De mobiele app kan ook de temperatuurinstellingen terugzenden naar de thermostaat. Er is geen extra infrastructuur nodig om toegang te krijgen tot de thermostaat.  Deze eenvoudige bediening via een mobiele app plus een laag energieverbruik is alleen mogelijk met Bluetooth Low Energy.

##  Gratis gateway naar het internet

Sensoren moeten vaak informatie naar de cloud sturen voor opslag en analyse. Hiervoor hebben WPAN’s een gateweay-apparaat nodig als tussenstation tussen het Internet (bijv. via WiFi/Ethernet) en de lokale draadloze technologie.

Aangezien BLE-apparaten eenvoudig kunnen worden aangesloten op draadloze apparaten die al via WiFi of GSM via internet zijn verbonden, hebben BLE-netwerken geen extra gateway-apparaat nodig. Deze draadloze apparaten fungeren dus als een gratis gateway naar het internet voor het BLE-netwerk, wat zorgt voor gebruiksgemak en geen extra kosten.  Alle andere WPAN’s hebben een extra gateway-apparaat nodig.

De architectuur van een dergelijk systeem wordt in onderstaande figuur weergegeven. Met de enorme data snelheid van Bluetooth Low Energy (tot wel 2 Mbps) wordt de data van één dag binnen 10 seconden verstuurt. De levensduur van het apparaat wordt niet beïnvloed, want het aantal berichten dat wordt verzonden blijft hetzelfde, ook wanneer er wordt gelogd of periodiek wordt verstuurt.


### Thermostaat met Bluetooth Low Energy en de cloud

Stel we willen bij de thermostaat in het vorige voorbeeld alle temperatuurdata van één dag verzamelen en naar de cloud sturen voor verdere verwerking. Een optie is om een apparaat in de buurt te hebben die continu verbonden is met de thermostaat en de real-time data doorstuurt naar de cloud.

Als dit niet mogelijk is, kan de thermostaat ook de data van een dag opslaan totdat je er een draadloos apparaat op aansluit. Dit kan gerealiseerd worden door slechts een extra functie in de mobiele app toe te voegen die de temperatuurgegevens logt en naar de cloud stuurt. Dus wanneer een smartphone verbinding maakt met de thermostaat, heeft het ook de mogelijkheid om de gegevens te loggen.

## Toepassingen

Bluetooth is met name populair in de IoT consumentenmarkt, waar het onder meer huizen en draagbare devices en accessoires met het internet verbindt. Mogelijke toepassingen zijn:
- **Smart homes**    

- **Airpods & headsets**

- **Afstandsbediening**

- **Smartphones**

- **Draadloze muis of toetsenbord**

- **Muziekbox**

- **Sensoren**

 En nog veel meer...

## Voordelen van de technologie

- Het kan snelle, simpele ad-hoc verbindingen leggen zonder noodzaak voor kabels of een uitgebreide installatie – devices hoeven alleen maar te ‘pairen’ waarna data al verzonden kan worden.
 
- Laag energieverbruik.

- Weliswaar enkel geschikt voor verbindingen op korte afstand, maar het vereist geen visueel contact: dergelijke verbindingen kunnen ook door muren of om hoeken gaan.

- Kan zowel voice als data versturen en ontvangen, met minimale storing en maximale beveiliging dankzij het gebruik van FHSS, waardoor het verspringt tussen verschillende beschikbare frequenties.

- Wijdverspreid: het is inmiddels een breed geïmplementeerde standaard voor dataverzending op korte afstand, die door verreweg de meeste devices ondersteund wordt en in veel consumentenproducten gebruikt wordt.

## Nadelen van de technologie

- Ondanks het relatief lage energieverbruik van bluetooth, blijft het probleem van draadloze technologie dat je de apparaten tussendoor moet opladen. Vooral bij telefoons die constant hun bluetooth aan hebben staan, gaat de batterij snel leeg.

- Je kunt zelf in je bluetooth instellingen zien welke bluetooth apparaten actief zijn. Dit is hartstikke handig om je luidspreker te vinden, maar deze informatie kan ook gebruikt worden als wapen. Hackers zien binnen enkele seconden welke apparaten zich om hen heen bevinden, en bepalen vanuit daar wie ze willen aanvallen.


## Gevaren met Bluetooth

Bluetooth is altijd op zoek naar apparaten om een verbinding mee te maken.
Wanneer er een verbinding wordt gemaakt, kan een hacker gevoelige of persoonlijke informatie van je apparaten aflezen en stelen.

Een hacker kan op afstand onderdelen van je apparaat besturen, instellingen veranderen en afkijken wat er op je scherm gebeurt.
Deze kan zo smsen of telefoongesprekken starten zonder dat je er iets van weet.

Maar dit is enkel mogenlijk als een hacker op een afstand is van 15 meter, anders kan deze het signaal niet ontvangen.


## Toekomst van Bluetooth

Bluetooth was tot nu toe verbindingen leggen tussen apparaten, maar het is dus de bedoeling dat deze breder gaat ingezet worden, deze zullen ook meer gericht worden op internet of things.

Zo heeft BLE (Bluetooth Low Energy) een hogere snelheid en kan het bereik 4 keer zo groot worden.

Bluetooth is dus ook veel geschikter voor beacons (energiezuinige bluetoothzenders).
Deze kunnen geplaats worden in gebouwen, dit is handig om te weten wie zich waar bevind in een gebouw.

Voor smarthomes is dit handig om te weten welke kamer de persoon zich bevindt.


## Bronnen

[elprocus - Hoe werkt Bluetooth](https://www.elprocus.com/how-does-bluetooth-work/)

[Meuleman - BLE populair](https://blog.meuleman.io/3-redenen-waarom-bluetooth-low-energy-zo-populair-is-geworden)

[Wikipedia - Bluetooth](https://nl.wikipedia.org/wiki/Bluetooth)

[Radar Avorotros - Wat is Bluetooth](https://radar.avrotros.nl/hulp-tips/hulpartikelen/item/bluetooth-wat-is-het-hoe-werkt-het-en-wat-heb-je-eraan/)

[Mediamarkt - Wat is bluetooth](https://blog.mediamarkt.be/mobiel-digitaal/wat-is-bluetooth/)

[InternetofThingsNederland - Bluetooth/Zigbee](https://internetofthingsnederland.nl/kennisbank/netwerken/bluetooth-zigbee/)

[VPNgids - Bluetooth wat zijn de gevaren?](https://www.vpngids.nl/privacy/devices/bluetooth-gevaren/)

[pcmweb - de geschiedenis en toekomst](https://pcmweb.nl/artikelen/audio/de-geschiedenis-en-toekomst-van-bluetooth/)

[Want - Binnen 10 sec gehackt](https://www.want.nl/bluetooth-gevaren-hack-blueborne/)