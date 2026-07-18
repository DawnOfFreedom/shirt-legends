# Shirts-site (werktitel)

One-pager voor de vintage-voetbalshirtshandel. Concept in reviewfase, merknaam volgt nog.

Alles zit in een enkel bestand: `index.html`. Foto's van de shirts, de De Boer-foto en het inlijst-voorbeeld zijn in het bestand zelf opgenomen. Alleen de grote hero-foto's (Pele, Maradona, Cruijff, Zlatan, Beckham, Pirlo) en de 1974-foto komen van Wikimedia Commons en vragen dus internet.

## Live zetten

Elke push naar `main` is na ongeveer een minuut live op GitHub Pages. Instelling staat op Settings > Pages > Deploy from a branch > `main` / root.

## Nog invullen voor livegang

- [x] Vinted- en Instagram-links: ingevuld en actief (staan hardgecodeerd in de HTML)
- [x] WhatsApp-nummer en e-mailadres in de contactregel: ingevuld
- [ ] Foto bij "Inlijsten" vervangen: het huidige beeld is een tijdelijke plaatshouder van een andere aanbieder en mag niet mee live (staat als comment in de code gemarkeerd)
- [ ] Topstukken vervangen door de echte topstukken van Adrie zodra de foto's er zijn (elke kaart is een `top-card`-blok in de HTML; kopieren, aanpassen of verwijderen)
- [ ] Merknaam en logo: "House of Football" is een werktitel en botst met een bestaande shop; rebrand loopt
- [ ] Domein pas registreren zodra de naam vaststaat, op naam en rekening van Adrie

## Aandachtspunten

- Spelersfoto's in de hero: Commons-licenties dekken het auteursrecht (credits staan in beeld), maar bij commercieel gebruik blijft portretrecht een aandachtspunt.
- De pagina werkt ook zonder JavaScript (documentviewers, WhatsApp-voorbeeld): alle tekst en ingebedde foto's zijn dan zichtbaar, alleen de hero-fotowissel en animaties vallen weg.
- Geen build-stap, geen dependencies. Aanpassen is: `index.html` bewerken, pushen, klaar.
