---
title: Mijn ideale media-center setup
date: 2016-06-16
categories:
  - kunst-creativiteit
tags:
  - kodi
  - media-center
  - nieuwsgroepen
  - nzbsd
  - raspberry-pi
  - sick-beard
  - synology
  - technologie
  - transmission
  - xbmc
lastmod: 2022-03-11T14:53:02.852Z
---

Voordat video-streaming de norm was, was het gangbaar om iedere film of aflevering handmatig te downloaden. Dat ging gepaard met heel wat gedoe: steeds moest je websites afspeuren naar het juiste torrent-bestandje, wachten tot de download klaar was, handmatig de juiste ondertiteling erbij zoeken (en hopen dat de ondertiteling gelijk liep met het beeld). De video keek je dan op je computer, waarvan het beeldscherm en geluid over het algemeen minder goed was dan die van je tv.

Altijd was ik op zoek naar manieren om dit proces prettiger te laten verlopen. Met succes! In 2012 had ik mijn setup compleet: Mijn favoriete films en series werden automatisch gedownload en gearchiveerd op een netwerkschijf. Vanuit mijn luie stoel kon ik in de woonkamer de TV aanzetten en werd me precies voorgeschoteld welke nieuwe video's er beschikbaar waren. Fantastisch :)

Mensen waren onder de indruk en vroegen me hoe ik dit voor elkaar gekregen had. Helaas was daar geen simpel antwoord op, want achter de schermen werkten diverse losse programma's en apparaten samen om dit te realiseren. Uiteindelijk heb ik een uitgebreide driedelige blogpost geschreven die als handleiding dient.

Nu, eind 2016, zijn veel van de software en hardware in de handleiding verouderd;  de hardware is verouderd: XMBC heet inmiddels KODI, er zijn diverse alternatieven te vinden voor de genoemde programma's en niet te vergeten: er zijn véél legale alternatieven op de markt die erg makkelijk werken! (denk aan [Netflix](https://www.netflix.com/nl/), [videoland](https://welkom.videoland.com/), [HBO](http://www.itshbo.nl/) of [Play van KPN](http://www.playvankpn.nl))

Hoewel verouderd, nog steeds nuttige informatie - de setup is bij mij nog steeds actief (in wat aangepaste vorm dan, wellicht dat ik dat ik ooit nog een update schrijf)

## [**Deel 1: Automatisch series/films downloaden (via nieuwsgroepen)**](http://www.stijnbiemans.nl/tech/automatisch-downloaden-via-nieuwsgroepen/)

Deel 1 gaat over de werking van nieuwsgroepen en de diverse programma's die je kunt gebruiken, zoals SickBeard, CouchPotato, Transmission en Sabnzbd. \[expand title="Meer lezen..." swaptitle="Sluit dit deel"  trigpos="below"\]Naast BitTorrent is kun je ook gebruik maken van nieuwsgroepen om films en series te downloaden. Als je nog niet bekend bent met dit systeem, lees dan even deze pagina om meer te weten te komen over dit systeem: [http://www.binaries4all.nl/beginners/](http://www.binaries4all.nl/beginners/)

De meeste internetproviders hebben een eigen nieuwsserver. Kijk op deze pagina met [serveradressen](https://www.binaries4all.nl/serveradressen/) om te zien of jouw provider ook een nieuwsserver heeft. Als je het adres van de nieuwsserver van jouw provider gevonden hebt (bijvoorbeeld nova.planet.nl), dan is deze stap succesvol afgerond. Biedt jouw provider geen nieuwsserver aan (of is de kwaliteit heel slecht), dan kan je een abonnement nemen bij een payserver ([meer informatie](https://www.binaries4all.nl/payservers/)). Payservers zijn niet gratis, maar zijn vele malen beter (bijvoorbeeld qua snelheid, retentie en compleetheid van de bestanden) dan een nieuwsserver van een provider.

Zelf heb ik ooit voor [blocknews.net](http://t.umblr.com/redirect?z=http%3A%2F%2Fwww.blocknews.net%2F&t=N2I1MWU1ZDIxZTk4Mzk2MTExMDExOWM1NzRjNzYwZjU4OTVmYjEyYSxaR3V0b0FwRg%3D%3D&b=t%3AwiMtAs-4wWCjU_32hq6glA&m=1) gekozen omdat je daar geen maandelijks abbonnement hoefde te kopen maar per “blocks” van een x-aantal gig kon kopen, een soort prepaid. Later ontdekte ik [deze](https://www.binaries4all.nl/payservers/) lijst van binaries4all, maar ik heb nooit meer vergelijkend warenonderzoek gedaan.

### **Sabnzbd - het download programma voor nieuwsgroepen**

Om te downloaden uit een binaries nieuwsgroep, heb je een nieuwsreader nodig. Oftewel: een programma dat een verbinding maakt met een nieuwsserver en de bestanden zal downloaden. Volg daarbij deze handleiding helemaal: [http://www.binaries4all.nl/sabnzbd/](http://www.binaries4all.nl/sabnzbd/)

### **Transmission – het downloadprogramma voor torrents**

Hoewel het meeste gedownload wordt van nieuwsgroepen met sabnzbd, zijn er soms nog dingen die je makkelijker via bittorrent vindt en download. Daarvoor gebruik ik Transmission, omdat sick beard en couch potato ook torrents naar transmission kunnen sturen. Uitleg op [http://www.binaries4all.nl/transmission/](http://www.binaries4all.nl/transmission/)

### **Sick Beard - Automatisch series downloaden**

Dit programma zoekt automatisch of er nieuwe afleveringen van de door jou gekozen series zijn. De nzb en torrent-bestanden stuurt ie dan door naar respectievelijk sabnzbd of transmission, eventueel met bijpassende ‘tag’. Alles staat perfect omschreven op [http://www.binaries4all.nl/sickbeard/](http://www.binaries4all.nl/sickbeard/)[.](http://t.umblr.com/redirect?z=http%3A%2F%2Fwww.binaries4all.nl%2Fsickbeard%2F&t=ZDIxMjc1MzcyYWI4MDIxZDU2M2Q4ZWRiM2QwNDg4MDQxODUyY2MyMixaR3V0b0FwRg%3D%3D&b=t%3AwiMtAs-4wWCjU_32hq6glA&m=1)

### **Couch Potato: Automatisch films downloaden**

Zelfde als Sick Beard, maar dan voor films. Simpel, wederom een handleiding volgen, hier: [http://www.binaries4all.nl/couchpotato/](http://www.binaries4all.nl/couchpotato/)

_Tip: Maak je gebruik van een Synology Disk Station om je bestanden op een netwerkschijf op te slaan? Dan kun je bovenstaande programma’s installeren op die Disk Station via [http://www.synocommunity.com/](http://www.synocommunity.com/)_

\[/expand\]

## [**Deel 2: De thuisserver als spil van je multimediasysteem**](http://www.stijnbiemans.nl/tech/back-end-de-thuisserver-als-spil-van-je-multimediasysteem/)

In deel 2 wordt ingegaan op de voordelen van een kleine thuisserver in je netwerk. In mijn geval bleek een NAS van Synology de beste keus.  \[expand title="Meer lezen..." swaptitle="Sluit dit deel"  trigpos="below"\] Alle programma's om automatisch te downloaden (zoals hierboven beschreven in deel 1) kun je gewoon op je pc of laptop installeren. Nadeel is dan dat je alles continu moet aan laten staan. Daarom is het relaxter om een thuisserver te installeren: een computer die altijd aanstaat voor twee belangrijke functies - Ten eerste om bestanden en printers te delen in het netwerk (zodat je alles vanaf iedere computer kan bereiken en gebruiken). Ten tweede kan deze server allerlei taken automatisch uitvoeren, zoals het vinden, downloaden en ordenen van nieuwe films en series!

Er zijn veel manieren om zo'n thuisserver te realiseren, bijvoorbeeld via een oude ongebruikte computer, een [raspberry pi](http://www.instructables.com/id/Ultimate-Pi-Based-Home-Server/) of een [android smartphone](http://lifehacker.com/5936339/servers-ultimate-turns-your-old-android-phone-into-a-tiny-multipurpose-server). Ik heb er voor gekozen om een [Synology Disk Station DS112j](http://www.synology.nl/products/product.php?product_name=DS112j&lang=nld) aan te schaffen. Deze netwerkschijf en thuis-server is energiezuinig, stil en krachtig genoeg om aan mijn digitale wensen te voldoen!

### **Voordelen:**

- Alle data (documenten, video's en muziek), op deze schijf zijn beschikbaar in mijn hele netwerk (dus op alle computers, tablets, telefoons en zelfs nieuwere tv's)
- Ook aangesloten randapperatuur (externe harde schijven, printers, etc) zijn beschikbaar voor alle computers in het netwerk.
- De mogelijkheid om allerlei programma's te installeren om (automatisch) te downloaden, zonder dat je je laptop aan hoeft te laten staan.
- Hij staat altijd aan dus download ook als ik m'n PC uitzet! Dat is energiezuiniger en stiller dan als mn computer altijd aan moet staan.
- Er zijn véél applicaties te installeren op de synology. Onder andere alle (download)programma's die ik beschrijf in [deel 1 van deze serie](http://www.stijnbiemans.nl/tech/automatisch-downloaden-via-nieuwsgroepen/). Kijk op  [http://www.synocommunity.com/](http://www.synocommunity.com/) voor meer info.

Uitgebreide uitleg van de Synology Disk Station als backend voor XBMC is [hier](http://www.robvanhamersveld.nl/2012/12/17/synology-nas-as-the-ultimate-xbmc-media-backend/) te lezen. In [deel 3 van deze serie](http://www.stijnbiemans.nl/tech/front-end-raspberry-pi-met-xbmc/) wordt verder ingegaan op het gebruik van XBMC via een Raspberry Pi op je TV.

\[/expand\]

## [**Deel 3: XBMC op je TV met Raspberry Pi**](http://www.stijnbiemans.nl/tech/front-end-raspberry-pi-met-xbmc/)

Nu je een manier hebt om al je favoriete films en series te downloaden en op te slaan, wil je natuurlijk ook een manier om deze videos zo goed mogelijk te bekijken! Hiervoor kun je een Raspberry Pi gebruiken die je aansluit op je TV. Hierop staat XBMC geinstalleerd, mooie en uitgebreide media-center software!  \[expand title="Meer lezen..." swaptitle="Sluit dit deel"  trigpos="below"\] Als je deel 1 en deel 2 uit deze serie gelezen hebt, heb je nu een manier om al je favoriete films en series te downloaden en op te slaan. Nu nog een manier om al dit moois om een makkelijke manier te bekijken. Daarvoor gebruik ik een Raspberry Pi met daarop XBMC.

### **Raspberry Pi**

De raspberry Pi is een volwaardige computer ter grootte van een bankpasje. Hoewel de Raspberry Pi ontwikkeld is voor educatieve doeleinden zijn de mogelijkheden eindeloos. Daarnaast is het een goedkope optie: De computer zelf is slechts $35,-! Omdat je er wel extra dingen bij nodig hebt (SDkaart voor geheugen, adapter voor de stroom, een hdmi-kabel om met het scherm te verbinden, een ethernetkabel voor netwerkverbinding en een omhulsel ter bescherming) Ben je vaak toch zo’n 70, 80 euro kwijt. Echter, als je al die dingen al hebt liggen ben je klaar voor zo’n 35,-

_tip: Bij PaxNova hebben ze een voordeelpakket waar je alles-in-een hebt voor 70 euro. Kopen kan o.a. hier: [http://paxnova.nl/raspberry-pi-model-b-voordeelpakket](http://paxnova.nl/raspberry-pi-model-b-voordeelpakket)_

###  **XBMC** 

XMBC is een gratis, krachtig en flexibel mediacenter-systeem. Die flexibiliteit heeft twee kanten. Het betekend dat als je iets wil, het bijna altijd mogelijk is in XBMC. Het nadeel is dat je op het begin even wegwijs moet worden in XBMC. Hieronder wat uitleg.

### **Installatie**

Installeren van nieuwe besturingssystemen op de Raspberry Pi is makkelijk via [NOOBS; New Out of Box Software](http://www.raspberrypi.org/archives/4100). Op de site van Raspberry Pi wordt alles uitgebreid uitgelegd.

Er zijn verschillende opties, zoals RaspBMC, openELEC en Xbian. Lifehacker heeft ze versies uitgebreid naast elkaar gelegd ([lees maar](http://lifehacker.com/raspberry-pi-xbmc-solutions-compared-raspbmc-vs-openel-1394239600)). Mijn voorkeur gaat uit naar openELEC, maar in wezen maakt het niet zo veel uit welke versie je kiest.

### **Bediening**

XBMC bedienen kan op vele manieren. de XBMC heeft een goede [wiki met uitleg](http://wiki.xbmc.org/index.php?title=Remote_controls#Smart_Phone_Remote).

Hieronder nog kort veelgebruikte opties:

- via toetsenbord en muis (Niet handig als je relaxt op de bank wil kijken, maar wel handig om tijdelijk te gebruiken om evt instellingen te veranderen)
- via je smartphone (Je moet wel XBMC Official Remote installeren voor [Android](https://play.google.com/store/apps/details?id=org.xbmc.android.remote) of [iPhone/iPad](https://itunes.apple.com/us/app/unofficial-official-xbmc-remote/id520480364?ls=1&mt=8) en instellingen aanpassen op [xbmc zelf](http://yatse.leetzone.org/redmine/projects/androidwidget/wiki/XbmcConfig#.UcwgHqEW3ew) en in de app)
- Via een infrarood-ontvanger en afstandsbediening (los kopen en aansluiten op een USBpoort)
- via de HDMI-CEC functie (als je TV het ondersteunt - [uitleg](http://www.avblog.nl/wat-is-hdmi-cec/))
- via flirc ([uitleg](http://vimeo.com/12542134#at=0) - [bestelpagina](https://www.modmypi.com/raspberry-pi-accessories/flirc))

### **Wegwijs worden in XBMC**

- Lees de [algemene en uitgebreide uitleg over XBMC](http://www.makeuseof.com/pages/xbmc-full-html). Veel nuttige info, dus goed doorlezen (ieder geval vanaf hoofdstuk 2.3)
- Op [deze ZDNET pagina](http://www.zdnet.nl/help/149317/verander-je-oude-pc-in-een-mediacenter-met-xbmc/) staan nog goede tips voor de Nederlandstalige gebruiker. Je kan er onder andere vinden hoe je XBMC in het Nederlands zet (_stap 1_), hoe je nieuwe media kan invoegen (_stap 5 en 6_), hoe je automatisch ondertitels kan laten downloaden (_stap 9_) en hoe je add-ons installeert (_stap 8_)
- Ook deze [Computer Totaal presentatie](http://computertotaal.nl/software/26623-mediacenter-inrichten-met-xbmc.html) geeft nog wat extra informatie en tips.

### **MPEG-2 and VC1 video codecs installeren**

Om te zorgen dat je alle videoformaten kan afspelen, moet je twee ‘codecs’ kopen en installeren. Op de website  “[The Only Raspberry Pi XBMC Tutorial You Will Ever Need](http://mymediaexperience.com/raspberry-pi-xbmc-with-raspbmc/)” wordt dat heel helder uitgelegd:

- Purchase MPEG-2 and VC1 codec license keys [here](http://www.raspberrypi.com/license-keys/)
- You will receive the license key from your email within 72 hours
- In Raspbmc, go to Programs > Raspbmc Settings > System Configuration (bij openELEC werkt het iets anders, daar kom ik nog op terug)
- Enter the license key from your email to MPEG-2 and/or VC1 codec under the Advanced system settings
- Reboot the system

### **Interessante addons:**

- [NOS](http://wiki.xbmc.org/index.php?title=Add-on:NOS)
- [Xbmc Online TV](http://www.rieter.net/content/) (Uitzending Gemist en meer!)
- [Nederland 24](http://wiki.xbmc.org/index.php?title=Add-on:NOS)
- [Trakt.tv](http://trakt.tv/downloads/xbmc) (registreren / scrobblen wat je kijkt, zoals Last.FM maar dan voor video)
- [Youtube](http://wiki.xbmc.org/index.php?title=Add-on:YouTube)
- [Vimeo](http://wiki.xbmc.org/index.php?title=Add-on:Vimeo)
- [TED Talks](http://wiki.xbmc.org/index.php?title=Add-on:TED_Talks)

\[/expand\]
