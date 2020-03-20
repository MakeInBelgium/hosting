# Hosting oplossing voor verschillende Corona Denktank initiatieven

De meeste discussies gebeuren op [Slack][1]. Kom kijken in de `#team-tech-hosting` en `#team-tech-uptime` channels als je wil helpen.

## Domeinnamen

Worden geregistreerd door vrijwilligers die een project willen starten. 

## DNS

De DNS zit telkens bij Cloudflare. Er is een account op naam van `tech@coronadenktank.be`.

Volgende personen hebben access, spreek hen aan op Slack als je wil bijdragen:

- Kristof (@iworx)
- Joren Van Severen
- Maarten Huijsmans
- Mattias Geniar (@mattiasgeniar)

## Static site hosting

De meeste websites zijn statische HTML, zonder dynamische inhoud. Daarin spreken we volgende af:

- De repository heeft telkens een commit met de **compiled assets**. De source CSS/JavaScript mag mee in de repo, maar je finale CSS/JS moet mee ge-commit worden. Builden doe je lokaal.
- Hoofdpagina is steeds `index.html`

De statische sites worden met CloudFlare workers online gezet.

**TODO: insert explanation about CF workers here**

## Caching / DoS bescherming / Redirects

Als je geen nood hebt aan onze hosting (omdat je zelf een VPS draait, eigen resources hebt) maar toch achter de beschermende vleugels van CloudFlare wil zitten, neem dan even contact op met hostingteam. 

## WordPress / Drupal hosting

Hiervoor draait een aparte server. De personen die mee de DNS beheren hebben ook hier toegang toe (zie lijst hierboven).

Vraag hen de account aan te maken en je krijgt SSH, FTP, MySQL & alle andere access die je nodig hebt om PHP, Ruby, ... te draaien. Ideaal voor WordPress.

Hou aub rekening met de server load: beperk de plugins & themes, schrijf performante code, ... als jouw site overlast bezorgt zijn andere sites mogelijk ook geïmpacteerd. Voor je live gaat of voor je het in de pers vermeld, neem even contact op met het team om te zien of er caching voor moet komen.

Als je site vermeldt wordt op het VTM journaal of Radio 2 kan je al snel rekenen op 100.000 bezoekers of meer, op héél korte tijdsspanne.

[1]:	https://join.coronadenktank.be/