# Boekenwinkel Broese

Broese boekenwinkel, opgericht in 1845 boekhandel in Utrecht en behoort tot de grootste van Nederland. Het assortiment omvat boeken in diverse genres, tijdschriften, spellen, puzzels, muziek (cd's en vinyl) en schrijfwaren

Linkje naar de website: www.broese.nl

<img width="1470" alt="image" src="https://github.com/user-attachments/assets/8221fd21-3fec-4a40-b842-bbc9e2b9f61d" />

## Performance Audit test
Voor deze performance-audit heb ik de website van Broese getest met drie verschillende tools: Lighthouse, Google PageSpeed Insights en WebPageTest. Elk van deze tools geeft op zijn eigen manier inzicht in hoe snel en efficiënt de website laadt, zowel op mobiel als op desktop. Hieronder bespreek ik kort de resultaten per test en trek ik aan het einde een algemene conclusie.

### Lighthouse test

Linkje naar mijn bevindingen van de [Lighthouse test](https://github.com/ambersr/performance-audit/wiki/Bevindingen-Lighthousetest) in de Wiki.

**Mobile**

Belangrijke bevindingen:
- Te grote afbeeldingen
- Veel externe javacript bestanden die worden ingeladen
- DOM zit te vol met elementen
<br>
<img width="1470" alt="image" src="https://github.com/user-attachments/assets/595c706f-518a-4099-83d7-7468ebf2d6d2" />

**Desktop**

Belangrijke bevindingen:
- Website presteert beter op desktop
- Largest Contentful Paint (LCP) laat sneller op desktop
<br>
<img width="1469" alt="image" src="https://github.com/user-attachments/assets/c862cf04-ac2d-463f-ba91-890bcff092ee" />

### PageSpeed test

Linkje naar mijn bevindingen van de [PageSpeed test](https://github.com/ambersr/performance-audit/wiki/Bevindingen-PageSpeed-Insights) in de Wiki.

**Mobile**

Belangrijke bevindingen:
- Onnodige, ongebruikte Javascript en CSS
- Zware afbeeldingen
<br>
<img width="1467" alt="image" src="https://github.com/user-attachments/assets/791a0b5d-63b0-4a67-ad9c-abe4041ff433" />

**Desktop**

Belangrijke bevindingen:
- Te grote afbeeldingbestanden
- Teveel externe scripts die ingeladen worden (Google Analytics en Google Tag Manager)
<br>
<img width="1469" alt="image" src="https://github.com/user-attachments/assets/6f3769cd-8296-408e-acd0-8363be7a35b1" />

### WebPageTest

Linkje naar mijn bevindingen van de [WebPageTest](https://github.com/ambersr/performance-audit/wiki/Bevindingen-WebPageTest) in de Wiki.

**Waterfall chart**

Belangrijke bevindingen:
- Externe scripts zorgen voor een lange laattijd
- Afbeeldingen (banner slider) hebben een lange laattijd
<br>
<img width="1144" alt="image" src="https://github.com/user-attachments/assets/b781930e-1d0d-4829-b6fc-b03db48b3b66" />

### Conclusie bevindingen
Uit de verschillende tests blijkt dat de grootste knelpunten op de Broese-website liggen bij het laden van de grote bannerafbeeldingen in de slider. Deze afbeeldingen zijn qua bestandsgrootte veel te zwaar, wat zorgt voor een merkbaar lange laadtijd – vooral op mobiele apparaten. Bezoekers moeten hierdoor langer wachten voordat de pagina volledig zichtbaar en bruikbaar is.

Daarnaast spelen externe scripts ook een behoorlijke rol. Deze scripts zoals Google Analytics en Google Tag Manager veroorzaken extra netwerkverkeer en vertragen het laadproces van de pagina. Vooral bij trage netwerken of mobiele verbindingen wordt dit probleem versterkt.

**Hoe verbeteren?**
- Afbeeldingen comprimeren en moderne formaten gebruiken (zoals WebP).
- Onnodige scripts verminderen.
- Slimme caching en lazy loading toepassen.

## Licentie

This project is licensed under the terms of the [MIT license](./LICENSE).
