# Corona Denktank : Team Hosting

De meeste discussies gebeuren op [Slack][1]. Kom kijken in de `#team-tech-hosting` en `#team-tech-uptime` channels als je wil helpen.

## Domeinnamen

Worden geregistreerd door vrijwilligers die een project willen starten. 
Probeer hier pragmatisch in te zijn en registreer niet zomaar iets. 
Check even met `#corona-communicatie` voor een passende naam.

## DNS

De DNS zit telkens bij Cloudflare. Er is een account op naam van `tech@coronadenktank.be`.

DNS Servers die nu meestal toegewezen worden door Cloudflare zijn : 
```
gordon.ns.cloudflare.com
julissa.ns.cloudflare.com
``` 

Volgende personen hebben access, spreek hen aan op Slack als je wil bijdragen:

- Kristof Rutten (@iworx)
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

Als je geen nood hebt aan onze hosting (omdat je zelf een VPS draait, eigen resources hebt) maar toch achter de beschermende vleugels van CloudFlare wil zitten, neem dan even contact op met hosting team. 

Wat kunnen we bieden : 
- Full offloading: enkel voor volledig statische websites. (Always on/Cache everything)
- WWW to non-WWW rewriting
- Forwarding (301/302) 

## WordPress / Drupal hosting

Hiervoor draait een aparte server. De personen die mee de DNS beheren hebben ook hier toegang toe (zie lijst hierboven).

Vraag hen de account aan te maken en je krijgt SSH, FTP, MySQL & alle andere access die je nodig hebt om PHP, Ruby, ... te draaien. Ideaal voor WordPress.

Hou aub rekening met de server load: beperk de plugins & themes, schrijf performante code, ... als jouw site overlast bezorgt zijn andere sites mogelijk ook geïmpacteerd. Voor je live gaat of voor je het in de pers vermeld, neem even contact op met het team om te zien of er caching voor moet komen.

Als je site vermeldt wordt op het VTM journaal of Radio 2 kan je al snel rekenen op 100.000 bezoekers of meer, op héél korte tijdsspanne.

[1]:	https://join.coronadenktank.be/

## Sysadmin hulp
Kom je er zelf niet aan uit op jouw hosting? Stel gerust je vraag. 
Er zitten altijd wel een paar specialisten om je verder te helpen.