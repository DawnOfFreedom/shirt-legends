# Shirt Legends · shirtlegends.nl

One-pager voor de vintage-voetbalshirtshandel van Adrie. Alles zit in één bestand: `index.html`.

Alle foto's van Adrie zelf (topstukken, Hanegem-schoenen mét signeerfoto, het rek, familiearchief, De Boer, Van Hanegem, het ingelijste EK '88-shirt met originele tickets, de sfeerbeelden uit Rome, Napels, Bilbao, Valencia en De Kuip) zitten in het bestand zelf. Alleen de grote hero-foto's en de 1974-foto komen van Wikimedia Commons; een foto die daar niet laadt wordt automatisch overgeslagen.

## Live zetten

Elke push naar `main` is na ongeveer een minuut live op GitHub Pages (Settings > Pages > `main` / root).

## Taal (NL / EN)

Vlaggetje rechtsboven schakelt naar Engels. Alle Engelse teksten staan onderin `index.html` onder `VERTALINGEN`. Directe Engelse link: `…/#en`.

## Afgerond in deze ronde (feedback Adrie, 31 juli)

- [x] Inlijsten: het ingelijste EK '88-shirt (Nº 12, met de originele tickets Düsseldorf en de finale) in plaats van Sneijder, plus de Van Basten-foto van dat moment eronder
- [x] Sfeersectie: Kuip-tifo, de grote Maradona-muurschildering en het Valencia-museum erin; kleedkamerfoto eruit
- [x] Bijschriften gecorrigeerd: Rome · Batigol, Bilbao · het museum van Athletic, Napels · Diego (D10S weg op verzoek)
- [x] Nieuwe, betere foto's van De Boer-ontmoeting en Adrie met Van Hanegem
- [x] "Veertig jaar voetbal" in de collectie-strip, "mancave" aan elkaar, "op jacht" in de zoektekst
- [x] Inkoop duidelijker (tip van Karen): blok "Shirts liggen? Wij nemen ze over." met WhatsApp-link
- [x] Contact: zichtbare WhatsApp- en mailknoppen met Adries nummer (+31 6 20 13 63 19)

## Afgerond in de layout-ronde

- [x] Verhaal-kop over de volle breedte, tekst en foto's eronder in twee kolommen
- [x] Inlijstfoto's naast elkaar (geen groot leeg vlak meer)
- [x] Hanegem-schoenfoto opnieuw gemaakt: nette crop in plaats van wegpoetsen
- [x] Voorhoofden terug in beeld op de Van Hanegem-foto
- [x] WhatsApp-knop in de navigatie, WhatsApp en Mail in de footer
- [x] "Shirts liggen? Wij nemen ze over." ook als regel in het zoekblok
- [x] Mobiel doorlopen: nav compact onder 520px, alle grids klappen netjes terug

## Afgerond in de laatste ronde

- [x] "Wij nemen ze graag over!" (kop en zoekblok)
- [x] Mockup-melding "Laatste drop" verwijderd: er is geen live Vinted-koppeling, dus niets verzinnen
- [x] Inlijsten in Onderweg-stijl: tekst bovenaan, de twee foto's groot naast elkaar eronder
- [x] Hanegem-schoenfoto's vervangen door de onbewerkte originelen (zijaanzicht met witte hak en de stempel-close-up)

## Nog te doen voor livegang

- [x] **Instagram-handle**: account bleek hernoemd naar `instagram.com/shirtlegends.nl` (731 volgers); alle links bijgewerkt.
- [ ] **Domein koppelen**: CNAME `www` naar `dawnoffreedom.github.io` plus de vier GitHub Pages A-records voor het kale domein; daarna custom domain invullen in GitHub Settings > Pages en "Enforce HTTPS" aanvinken.
- [ ] **Rome-check**: staat de Batistuta-mural inderdaad in Rome? (comment in de HTML bij het bijschrift)
- [ ] Maten en exacte seizoenen bij de topstukken aanscherpen (comments in de HTML).
- [x] **Professioneel mailadres**: `info@shirtlegends.nl` staat overal op de site (mailknoppen in Vinted-sectie en footer). Vóór de push even testmailen dat hij echt aankomt.

## Aandachtspunten

- De Van Basten-foto en de Kuip-tifofoto zijn (waarschijnlijk) persfoto's; ze staan erop na uitdrukkelijk akkoord van Adrie en Jan. Risico bij dit soort beelden: fotobureaus sturen soms naheffingen bij commercieel gebruik.
- De foto's met Van Hanegem staan er op verzoek; bij twijfel even aan Willem vragen.
- Pagina werkt zonder JavaScript; hero-wissel, animaties en taalknop vallen dan weg.
- Geen build-stap, geen dependencies: `index.html` bewerken, pushen, klaar.
