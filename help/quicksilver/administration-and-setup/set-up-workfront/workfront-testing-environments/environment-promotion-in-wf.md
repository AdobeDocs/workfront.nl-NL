---
user-type: administrator
content-type: overview;how-to-procedural
product-area: system-administration
navigation-topic: workfront-testing-environments
title: Objecten van de ene omgeving naar de andere verplaatsen binnen Workfront
description: Het vermogen van de Bevordering van het Milieu is bedoeld om de capaciteit te verstrekken om op configuratie betrekking hebbende voorwerpen van één milieu aan een andere te bewegen. Het ondersteunt niet de mogelijkheid om transactieobjecten te verplaatsen (met beperkte uitzonderingen).
author: Becky
feature: System Setup and Administration
role: Admin
hide: true
hidefromtoc: true
recommendations: noDisplay, noCatalog
source-git-commit: b44c83314a06592e21ab3c4316e2574b75e85715
workflow-type: tm+mt
source-wordcount: '910'
ht-degree: 0%

---

# Overzicht van het verplaatsen van objecten tussen Workfront-omgevingen (milieubevordering)

De mogelijkheid om het milieu te bevorderen, moet de mogelijkheid bieden om objecten van de ene Workfront-omgeving naar de andere te verplaatsen. U kunt bijvoorbeeld een sjabloon maken en deze configureren in de sandboxomgeving, in de wetenschap dat het testen geen invloed heeft op de feitelijke gegevens van uw organisatie. Nadat het malplaatje wordt gevormd en getest, kunt u het naar uw productiemilieu bewegen, klaar om te gebruiken.

Dit proces wordt &quot;milieubevordering&quot; genoemd.

U kunt dit proces in Workfront uitvoeren door een pakket met objecten te maken die u wilt verplaatsen en het pakket vervolgens in de nieuwe omgeving te installeren.

* Zie voor specifieke instructies over het uitvoeren van dit proces in Workfront:

   * [Een pakket voor milieubescherming maken of bewerken](/help/quicksilver/administration-and-setup/set-up-workfront/workfront-testing-environments/environment-promotion-create-package.md)
   * [Een pakket voor milieubescherming installeren](/help/quicksilver/administration-and-setup/set-up-workfront/workfront-testing-environments/environment-promotion-install-package.md)

* Voor instructies over het uitvoeren van dit proces via de Workfront API raadpleegt u [Objecten verplaatsen tussen [!DNL Workfront] omgevingen die de [!DNL Workfront] API](/help/quicksilver/administration-and-setup/set-up-workfront/workfront-testing-environments/environment-promotion.md).

## Ondersteunde objecten voor milieubescherming

Het vermogen van de Bevordering van het Milieu is bedoeld om de capaciteit te verstrekken om op configuratie betrekking hebbende voorwerpen van één milieu aan een andere te bewegen. Het ondersteunt niet de mogelijkheid om transactieobjecten te verplaatsen (met beperkte uitzonderingen).

* [Werkobjecten](#work-objects)
* [Objecten rapporteren](#reporting-objects)
* [Aangepaste gegevensobjecten](#custom-data-objects)
* [Organisatie-objecten](#organization-objects)
* [Andere configuratieobjecten](#other-configuration-objects)


### Werkobjecten

| Promoteerbaar object | Opgenomen promoteerbare subobjecten |
| --- | --- |
| Project (PROJ) | Project<br>Taak<br>Toewijzing<br>Voorganger<br>Bedrijf<br>Overschrijvingssnelheid<br>Groep<br>Rol<br>Team<br>Goedkeuringsproces<br>Goedkeuringspad<br>Goedkeuringsstap<br>Stap fiatteur<br>Schema<br>Onwerkdag<br>Wachtrijdefinitie<br>Onderwerpgroep wachtrij<br>Onderwerp van wachtrij<br>Routeringsregel<br>Mijlpad<br>Mijlsteen<br>Uurtype<br>Bronpool<br>Categorie<br>Categorieparameter<br>Parameter<br>Parametergroep<br>Parameteroptie<br>Categorieweergavelogica |
| Sjabloon (TMPL) | Sjabloon<br>Sjabloontaak<br>Toewijzing sjabloontaak<br>Sjabloontaakvoorganger<br>Bedrijf<br>Overschrijvingssnelheid<br>Groep<br>Rol<br>Team<br>Goedkeuringsproces<br>Goedkeuringspad<br>Goedkeuringsstap<br>Stap fiatteur<br>Schema<br>Onwerkdag<br>Wachtrijdefinitie<br>Onderwerpgroep wachtrij<br>Onderwerp van wachtrij<br>Routeringsregel<br>Mijlpad<br>Mijlsteen<br>Uurtype<br>Bronpool<br>Categorie<br>Categorieparameter<br>Parameter<br>Parametergroep<br>Parameteroptie<br>Categorieweergavelogica |

### Objecten rapporteren

| Promoteerbaar object | Opgenomen promoteerbare subobjecten |
| --- | --- |
| Lay-outsjabloon (UITMPL) | Lay-outsjabloon<br>Dashboard<br>Kalender<br>Kalender, sectie<br>Externe pagina<br>Rapport<br>Filter<br>Groepering<br>Weergave<br>Parameter |
| Dashboard (PTLTAB) | Dashboard<br>Kalender<br>Kalender, sectie<br>Externe pagina<br>Rapport<br>Filter<br>Groepering<br>Weergave<br>Parameter |
| Kalender (CALEND) | Kalender<br>Kalender, sectie |
| Externe pagina (EXTSEC) | Externe pagina |
| Rapport (PTLSEC) | Rapport<br>Filter<br>Groepering<br>Weergave<br>Parameter |
| Filter (UIFT) | Filter<br>Parameter |
| Groeperen (UIGB) | Groepering<br>Parameter |
| Weergave (UIVW) | Weergave<br>Parameter |

### Aangepaste gegevensobjecten

| Promoteerbaar object | Opgenomen promoteerbare subobjecten |
| --- | --- |
| Categorie (CTGY) | Categorie<br>Categorieparameter<br>Parameter<br>Parametergroep<br>Parameteroptie<br>Categorieweergavelogica<br>Groep |
| Parameter (PARAM) | Parameter<br>Parameteroptie |
| Parametergroep (PGRP) | Parametergroep |

### Organisatie-objecten

| Promoteerbaar object | Opgenomen promoteerbare subobjecten |
| --- | --- |
| Groep (GROEP) | Groep <br>Subgroepen (maximaal 5 niveaus) *<br>Categorie<br>Categorieparameter<br>Parameter<br>Parametergroep<br>Parameteroptie<br>Categorieweergavelogica |
| Rol (ROLE) | Rol |
| Team (TEAM) | Team<br>Groep |
| Bedrijf (CMPY) | Bedrijf<br>Overschrijvingssnelheid<br>Categorie<br>Categorieparameter<br>Parameter<br>Parametergroep<br>Parameter <br>Categorieweergavelogica<br>Groep |
| Portfolio (HAVEN) | Portfolio<br>Programma<br>Groep<br>Categorie<br>Categorieparameter<br>Parameter<br>Parametergroep<br>Parameteroptie<br>Categorieweergavelogica |
| Programma (PRGM) | Programma<br>Portfolio<br>Groep<br>Categorie<br>Categorieparameter<br>Parameter<br>Parametergroep<br>Parameteroptie<br>Categorieweergavelogica |

### Andere configuratieobjecten

| Promoteerbaar object | Opgenomen promoteerbare subobjecten |
| --- | --- |
| Goedkeuringsproces (ARVPRC) | Goedkeuringsproces<br>Goedkeuringspad<br>Goedkeuringsstap<br>Stap fiatteur<br>Rol<br>Team<br>Groep |
| Schema (SCHED) | Schema<br>Onwerkdag<br>Groep |
| Mijlpad (MPATH) | Mijlpad<br>Mijlsteen |
| Tijdbladprofiel (TSPRO) | Tijdbladprofiel<br>Uurtype |
| Uurtype (URT) | Uurtype |
| Type kosten (EXPTYP) | Type uitgave |
| Type risico (RSKTYP) | Type risico |
| Bronpool (RSPL) | Bronpool |

\* Momenteel niet beschikbaar


## Status van milieubescherming

De bevorderingspakketten van het milieu gaan door verscheidene statussen aangezien zij worden gecreeerd en bereid om zich tussen milieu&#39;s te bewegen. Deze statussen worden weergegeven in uw lijst met pakketten in Workfront of in de API-reacties als u de Workfront API gebruikt.

Deze statussen zijn onder andere:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>VERZAMELING</td> 
   <td><p>Deze status wordt automatisch toegewezen tijdens het samenstellen van objecten. </p><p>Bij samenstellen wordt verwezen naar het geautomatiseerde proces voor het identificeren van objecten en subobjecten die in een pakket moeten worden opgenomen en het toevoegen van die objecten en hun gegevens aan het pakket.</p><p>Deze status kan niet rechtstreeks door een klant worden ingesteld.</p></td> 
  </tr> 
  <tr> 
   <td>CONCEPT</td> 
   <td><p>Deze status wordt toegewezen aan het einde van een assemblageproces of bij het maken van een leeg promotiepakket.</p><p>Het is mogelijk dat een klant het promotiepakket terugbrengt naar deze status.</p><p>In deze status kan het promotiepakket niet in een omgeving worden geïnstalleerd.</p></td> 
  </tr> 
  <tr> 
   <td>TESTS</td> 
   <td><p>Met deze status kan een promotiepakket worden geïnstalleerd in elke voorvertoning of aangepaste vernieuwingssandbox. In deze status kan het pakket niet worden geïnstalleerd in Production.</p></td> 
  </tr> 
  <tr> 
   <td>ACTIEF</td> 
   <td><p>Met deze status kan een promotiepakket worden geïnstalleerd in elke omgeving, inclusief Productie.</p><p>Wanneer de pakketstatus is ingesteld op ACTIEF, wordt de instelling <code>publishedAt</code> De datum wordt automatisch ingesteld op de huidige tijdstempel van de aanvraag.</p></td> 
  </tr> 
  <tr> 
   <td>UITGESCHAKELD</td> 
   <td><p>Deze status wordt gebruikt om eerder gebruikte promotiepakketten te verbergen die in de toekomst niet in een omgeving worden geïnstalleerd.</p><p>Wanneer een pakket zich in deze status bevindt, kan het niet in een omgeving worden geïnstalleerd.</p><p>Wanneer een pakketstatus wordt ingesteld op DISABLED, wordt de <code>retiredAt</code> De datum wordt automatisch ingesteld op de huidige tijdstempel van de aanvraag.</p><p>Het gebruik van deze status wordt aanbevolen tijdens het gebruik van de<code>DELETE /package</code> eindpunt omdat het terugwinnbaar is en de installatiegeschiedenis voor om het even welke plaatsingen wordt behouden die met dit pakket worden gemaakt.</p></td> 
  </tr> 
  <tr> 
   <td>ASSEMBLING_FAILED</td> 
   <td><p>Het promotiepakket wordt automatisch in deze status geplaatst als de ASSEMBLING-fase mislukt.</p><p>Als u het pakket wilt terugplaatsen naar het ASSEMBLING-stadium, moet u het extractieproces opnieuw starten.</p></td> 
  </tr> 
  </tbody> 
</table>


