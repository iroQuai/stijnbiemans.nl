---
title: "Pi-Hole: Nooit meer online advertenties zien!"
date: 2017-02-15
draft: false
categories:
  - kunst-creativiteit
tags:
  - advertenties
  - pi-hole
  - raspberry-pi
  - raspbian
  - technologie
lastmod: 2022-03-11T14:54:26.084Z
image: /images/pi-hole-banner.png
---

Het internet staat er vol mee: online advertenties. Reclame op internet is big business: bijna iedere gratis online dienst (app/website) heeft op z'n minst één vorm van reclame ingebouwd. Zelfs in de menu's van sommige smart TV's is reclame verwerkt!  [Gratis diensten moeten op één of andere manier toch bekostigd worden](https://decorrespondent.nl/1150/jouw-aandacht-wordt-talloze-malen-per-dag-aan-de-hoogste-bieder-verkocht/98105873250-89aa2cc6).

Om te zorgen dat je nooit meer last hebt van al die digitale reclames, zijn er oplossingen! Je kan bijvoorbeeld een [ad-blocker installeren in je browser](https://adblockplus.org/nl/). Maar als je al je apparaten in je netwerk reclame-vrij wil hebben (dus ook je smartphone, tablet, spelcomputer en smart-tv), dan is een centrale ad-blocker veel handiger. Er zijn dure commerciële oplossingen beschikbaar, maar voor nog geen 20 euro bereik je met een Raspberry Pi hetzelfde, als je [Pi-Hole](http://www.pi-hole.net) installeert.

**Wat is Pi-Hole?**

In het kort: Pi-hole is een _advertising-aware_ dns- en webserver bedoeld om te draaien op een Raspberry Pi in jouw netwerk. Wanneer er een verzoek binnenkomt om een reclamedomein te resolven, zal Pi-hole dit ombuigen naar zichzelf zodat jouw client geen enkele connectie maakt met het reclamenetwerk.

Als je bovenstaande alinea niet helemaal begrijpt, geeft niks. Kijk gewoon onderstaand filmpje! ALs je meer achtergrond informatie wil, lees dan de [uitleg van PCMweb](http://www.pcmweb.nl/workshop/advertenties-blokkeren-met-je-raspberry-pi.html)  (hoewel je hun uitleg niet moet volgen, want die is niet meer up-to-date)

https://www.youtube.com/watch?v=vKWjx1AQYgs

**Dit wil ik ook! Wat moet ik doen?**

1. Pak je Raspberry Pi. Als je er nog geen hebt, koop er een. Er zijn [verschillende versies](https://www.raspberrypi.org/products/) beschikbaar. De twee meest logische keuzes zijn een Raspberry Pi 3, of een Raspberry Pi Zero (de Zero is goedkoper en kleiner, maar zonder ethernetpoort. Als je voor de Zero gaat, koop dan in ieder geval [ook de adapters](https://shop.pimoroni.com/products/raspberry-pi-zero) erbij en ik zou ik [deze USB-hub met ethernetpoort](https://shop.pimoroni.com/products/three-port-usb-hub-with-ethernet-and-microb-connector) adviseren)
2. Installeer Raspbian (volg [deze handleiding](https://raspberrytips.nl/raspberry-pi-installeren/) om te zorgen dat je helemaal up-do-date bent!)
3. Installeer Pi-Hole door in de terminal het volgende commando in te voeren: _curl -sSL https://install.pi-hole.net | bash_
4. Nadat je de installatie-wizard hebt doorlopen moet je de DNS-gegevens aanpassen op de apparaten waarvoor je het wil gebruiken ([Zo pas je DNSgegevens aan per apparaat](https://www.consumentenbond.nl/alles-in-1/alternatieve-dns-instellen)). Je kan er ook voor kiezen om de DNS-gegevens in je router aan te passen, zodat _alle_ apparaten in je netwerk gebruik kunnen maken van Pi-Hole (zelfs je smart-TV en nieuwe apparaten die verbinding maken met je netwerk).  ([Zo pas je je DNS-gegevens aan op je router](https://www.lifewire.com/how-to-change-dns-servers-on-most-popular-routers-2617995))
5. Klaar!
