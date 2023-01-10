# Creatief concept SOA/MSA
*S.P.A.C.E.: Space Planning and Coordination Environment*

Het concept dat ik heb bedacht is een platform dat helpt bij het plannen en coördineren van ruimtemissies genaamd S.P.A.C.E. Door een centrale site aan te bieden voor missieplanning en communicatie, zou het platform de effectiviteit en veiligheid van ruimtevaart moeten vergroten.

## S.P.A.C.E.  
**S**pace **P**lanning **A**nd **C**oordination **E**nvironment is een uitgebreid webplatform voor het organiseren en coördineren van ruimtemissies. 

## Architectuur  

Het platform zal een microservices-architectuur zijn, waardoor flexibiliteit en schaalbaarheid van de verschillende individuele services mogelijk is. Om te kunnen communiceren tussen services maakt de architectuur gebruik van voorziene API-calls in elke service. Alle individuele services worden ook in containers ontwikkeld/geplaatst voor eenvoudige schaalbaarheid, ontwikkeling en overdraagbaarheid.

## Services  

Een opsomming van mijn services die goed in de context van dit concept passen.

- **Wiki-service:**  een gecentraliseerde opslagplaats voor informatie over raketten (en hun fabrikanten) en planeten. Hiermee kunnen gebruikers informatie opzoeken over verschillende raketten en hun specificaties, evenals informatie bekijken over planeten of de ster waar ze rond draaien.
- **Robotcoördinatie:** Deze service is verantwoordelijk voor het verzenden van coördinaten (en opdrachten) vanuit het hoofdkwartier naar verschillende robots op planeten of satelieten.
- **Telefoonboek:** Het opzoeken van telefoonnummers van specifieke mensen die betrokken zijn bij ruimtemissies.
- **Poll-service:** Hiermee kunnen gebruikers (bv. astronauten) polls maken met betrekking tot de ruimtemissie en stemmen op verschillende opties. Dit kan bijvoorbeeld worden gebruikt om feedback te krijgen op verschillende missieplannen.
- **Nutrition calculator:** Deze service helpt bij het berekenen en organiseren van de voeding die een astronaut nodig heeft tijdens de missie voor de best mogelijke prestaties.
- **Binaire conversie**: Het omzetten van tekst in binaire code en vice versa. Dit kan handig zijn met encoderen van communicatie om ze zo via o.a. radiogolven te verzenden naar planeten.

Hier zijn andere services die eventueel nog met deze architectuur zouden samengaan.

- **Notificaties**: Een manier om gebruikers meldingen te sturen over de status van de missie.
- **Weervoorspellingen:** Op basis van de atmosfeer van planeten het weer voorspellen.

## Implementatie (Cloud)

De microservices kunnen georkestreerd worden door infrastructuur zoals Kubernetes of Docker Swarm op een cloudprovider zoals AWS, Azure of Google Cloud Platfrom. Na de implementatie en deployment op een cloudservice kunnen de prestaties van de microservices gemakkelijk gecontroleerd worden door de monitoring van de cloudprovider.