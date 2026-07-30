# Shirt Legends · shirtlegends.nl

One-pager voor de vintage-voetbalshirtshandel van Adrie. Alles zit in één bestand: `index.html`.

De shirtfoto's (Adries eigen topstukken), de Hanegem-schoenen mét signeerfoto, het shirtrek, de elftalfoto uit het familiearchief, de foto van Adrie met Van Hanegem, de sfeerbeelden uit Napels, Bilbao en De Kuip, het ingelijste Sneijder-shirt, het logo en de favicon zijn allemaal in het bestand zelf opgenomen. Alleen de grote hero-foto's (legendes) en de 1974-foto komen van Wikimedia Commons en vragen dus internet; een foto die daar niet laadt wordt automatisch overgeslagen.

## Live zetten

Elke push naar `main` is na ongeveer een minuut live op GitHub Pages. Instelling staat op Settings > Pages > Deploy from a branch > `main` / root.

## Taal (NL / EN)

Rechtsboven staat een vlaggetje: daarmee schakelt de bezoeker naar het Engels en terug. Alle Engelse teksten staan onderin `index.html` bij elkaar in het script, onder het kopje `VERTALINGEN`. Tekst wijzigen: de Nederlandse tekst in de HTML aanpassen én dezelfde key in die lijst. Directe Engelse link om te delen: `…/#en`.

## Afgerond in deze ronde

- [x] Foto-verwisseling hersteld: familiearchief toont nu de echte elftalfoto, bij "Ontmoeting" staat Adrie met Van Hanegem
- [x] Signeerfoto van Willem toegevoegd als derde beeld bij de adidas HANEGEM-schoenen
- [x] Sfeersectie "Onderweg" uitgebreid naar zes beelden (Napels, Bilbao, De Kuip)
- [x] Topstukken nu vast drie om drie (geen wees-kaart meer op brede schermen)
- [x] Zoekblok compacter, met "Interesse? Bekijk Instagram of Vinted"
- [x] Melding-mockup heet nu "Laatste drop van Shirt Legends"
- [x] Hero volgt Adries rijtje: Feyenoord 1970, Pelé, Ajax 1972, Oranje 1974, Rossi 1982 (PABLITO), Maradona 1986, EK '88, het gouden trio 1989, Pirlo
- [x] Alle em-dashes verwijderd (bouwcontrole aanwezig)

## Nog te doen voor livegang

- [ ] **Instagram-handle checken**: de link `instagram.com/retroshirts.insta` geeft "profiel niet beschikbaar". Mogelijk is het account hernoemd (er bestaat een `retroshirts.rdam`, niet geverifieerd). Juiste handle bij Adrie opvragen en dan in `index.html` overal `retroshirts.insta` vervangen (staat op vier plekken, zoek-vervang volstaat).
- [ ] **Domein koppelen**: bij de registrar een CNAME-record `www` naar `dawnoffreedom.github.io` (en voor het kale domein de vier GitHub Pages A-records), daarna in GitHub Settings > Pages het custom domain invullen en "Enforce HTTPS" aanvinken.
- [ ] **Bijschriften checken door Adrie**: klopt "Bilbao · San Mamés" bij de kleedkamerfoto? (comment in de HTML wijst de plek; weghalen kan ook). En de plaatsbepaling "Napels" bij de Maradona-beelden.
- [ ] **Maten en exacte seizoenen** bij de topstukken aanscherpen (comment in de HTML, vergeet de EN-vertaling niet).
- [ ] Eventueel later: strakkere foto van het ingelijste Sneijder-shirt en een og:image.

## Aandachtspunten

- De juichende Van Basten-foto (EK '88) staat bewust niet op de site: dat is een professionele persfoto met auteursrecht van een fotopersbureau. Het EK-'88-moment zit al in de hero via een rechtenvrije Anefo-foto van de huldiging.
- De foto's van Adrie met Van Hanegem en van het signeren staan er op uitdrukkelijk verzoek; het blijven persoonlijke foto's van een bekende Nederlander op een commerciële site. Bij twijfel: even aan Willem vragen.
- Napels-beelden zijn eigen reisfoto's van straatkunst; gangbaar als sfeerbeeld, formeel ligt het auteursrecht van een mural bij de maker.
- Pagina werkt zonder JavaScript; hero-wissel, animaties en taalknop vallen dan weg.
- Geen build-stap, geen dependencies. Aanpassen is: `index.html` bewerken, pushen, klaar.
