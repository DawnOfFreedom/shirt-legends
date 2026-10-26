# Shirt Legends · shirtlegends.nl

One-pager voor de vintage-voetbalshirtshandel van Adrie. Live op **https://shirtlegends.nl**.

Alles zit in één bestand: `index.html` (ongeveer 3,6 MB). Alle foto's van Adrie zelf zitten als base64 in dat bestand ingebakken: topstukken, de Hanegem-schoenen met signeerfoto, het rek, het familiearchief, De Boer, Van Hanegem, het ingelijste EK '88-shirt met de originele tickets, en de sfeerbeelden uit Rome, Napels, Bilbao, Milaan en De Kuip. De hero draait op de foto's van de topstukken (ze worden uit de top-cards gehaald, dus een nieuw topstuk komt vanzelf in de hero). Alleen de 1974-foto in de strip komt nog van Wikimedia Commons; als die niet laadt verdwijnt de strip automatisch.

Geen build-stap, geen dependencies. Aanpassen is: `index.html` bewerken, committen, pushen.

## Aanpassen en live zetten

```bash
cd ~/GitHub/"Shirt Legends"
git pull
# index.html bewerken
git add index.html
git commit -m "korte omschrijving"
git push
```

Elke push naar `main` staat na ongeveer een minuut live. Bron: Settings › Pages › Deploy from a branch › `main` / root.

Het bestand `CNAME` in de repo bevat `shirtlegends.nl` en is door GitHub zelf aangemaakt. **Niet verwijderen** — zonder dat bestand valt het custom domain weg.

## Taal (NL / EN)

Het vlaggetje rechtsboven schakelt naar Engels. Alle Engelse teksten staan onderin `index.html` onder `VERTALINGEN`. Directe Engelse link: `…/#en`.

Pas je een Nederlandse tekst aan met een `data-t`-attribuut, pas dan ook de bijbehorende sleutel in `VERTALINGEN` aan, anders lopen de twee talen uit elkaar.

## Domein en DNS (TransIP, account van Adrie)

Het domein staat bij TransIP op naam van Adrie. De mail (`info@` en `adriedegraaf@`) loopt via TransIP Mail op hetzelfde domein.

De DNS wordt handmatig beheerd: de schakelaar **TransIP-instellingen staat uit**. Zet die nooit meer aan — dan overschrijft TransIP álle records met zijn standaardset en ligt zowel de site als de mail eruit.

Records die naar GitHub Pages wijzen:

| Naam | Type | Waarde |
|------|------|--------|
| `@` | A | `185.199.108.153` |
| `@` | A | `185.199.109.153` |
| `@` | A | `185.199.110.153` |
| `@` | A | `185.199.111.153` |
| `www` | CNAME | `dawnoffreedom.github.io.` |

Het AAAA-record op `@` is bewust verwijderd: dat wees nog naar TransIP, waardoor IPv6-bezoekers op de verkeerde server terechtkwamen.

Alles wat met mail te maken heeft blijft ongemoeid: de MX naar `mx.transip.email`, de SPF-TXT, `_dmarc`, de drie `transip-x._domainkey`-CNAME's en `autoconfig` / `autodiscover`. Kom je daar per ongeluk aan, dan stopt de mail.

HTTPS staat aan via Settings › Pages › Enforce HTTPS. Het certificaat wordt automatisch vernieuwd.

## Afgerond op 20 augustus 2026

- [x] Repo hernoemd van `house-of-football` naar `shirt-legends`
- [x] San Siro-foto van Adrie in de sfeer-grid, op de plek van het Valencia-museum (bijschrift "Milaan · San Siro", NL en EN)
- [x] De Boer-foto vervangen door de versie zonder het Eemslag-reclamebord
- [x] Witte rand boven de adidas Hanegem-schoen weggesneden
- [x] Hero-foto's minder zwaar behandeld: grijsfilter eraf, helderheid omhoog, verloop opengetrokken
- [x] Domein `shirtlegends.nl` gekoppeld, HTTPS afgedwongen

## Nog te doen

- [ ] **Rome-check**: staat de Batistuta-mural inderdaad in Rome? (staat als comment in de HTML bij het bijschrift)
- [ ] Maten en exacte seizoenen bij de topstukken aanscherpen (comments in de HTML)

## Aandachtspunten

- **Persfoto's.** De Kuip-tifofoto is waarschijnlijk een persfoto. Hij staat erop na uitdrukkelijk akkoord van Adrie en Jan. Fotobureaus sturen bij commercieel gebruik soms naheffingen. De Van Basten-foto (EK '88) is in oktober 2026 weggehaald vanwege portretrecht.
- **Portretrecht.** De foto's met Van Hanegem staan er op verzoek; bij twijfel even aan Willem vragen. De Wikimedia-spelersfoto's in de hero (Pelé, Cruijff, Maradona en anderen) zijn in oktober 2026 weggehaald: de licentie dekt het auteursrecht, niet het portretrecht, en met een gekoppelde shop is het gebruik commercieel.
- **Geen webshop op GitHub Pages.** GitHub staat Pages niet toe als gratis hosting voor sites die primair commerciële transacties faciliteren. Deze one-pager verkoopt zelf niets en verwijst door naar de Shopify-winkel op https://shop.shirtlegends.nl, Instagram en WhatsApp. De winkel en de betalingen draaien bij Shopify, niet op Pages, dus dat is in orde. Winkelfuncties horen daar, niet in dit bestand.
- **Zonder JavaScript** werkt de pagina ook: alle tekst en ingebedde foto's zijn zichtbaar, alleen de hero-fotowissel, de animaties en de taalknop vallen weg.

## Op de plank

Een 360-graden draaiviewer voor één hero-topstuk bestaat als losse proof-of-concept (`spin-demo.html`, laadt een genummerde framereeks met autorotatie en sleepbediening). Pas bruikbaar zodra Adrie een shirt op een draaiplateau fotografeert.
