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
exl-id: 8b4c04f5-f519-44e9-8429-0ce80c2d7c5b
source-git-commit: 53596271a838733b858c0b14a4e22b07a7cd20f6
workflow-type: tm+mt
source-wordcount: '1046'
ht-degree: 0%

---

# Overzicht van het verplaatsen van objecten tussen Workfront-omgevingen (milieubevordering)

Met de functie voor milieubescherming kunt u objecten van de ene Workfront-omgeving naar de andere verplaatsen. U kunt bijvoorbeeld een sjabloon maken en deze configureren in de sandboxomgeving, in de wetenschap dat het testen geen invloed heeft op de feitelijke gegevens van uw organisatie. Nadat het malplaatje wordt gevormd en getest, kunt u het naar uw productiemilieu bewegen, klaar om te gebruiken.

Dit proces wordt &quot;milieubevordering&quot; genoemd.

U kunt dit proces in Workfront uitvoeren door een pakket met objecten te maken die u wilt verplaatsen en het pakket vervolgens in de nieuwe omgeving te installeren.

* Zie voor specifieke instructies over het uitvoeren van dit proces in Workfront:

   * [Een pakket voor milieubescherming maken of bewerken](/help/quicksilver/administration-and-setup/set-up-workfront/workfront-testing-environments/environment-promotion-create-package.md)
   * [Een pakket voor milieubescherming installeren](/help/quicksilver/administration-and-setup/set-up-workfront/workfront-testing-environments/environment-promotion-install-package.md)

* Voor instructies bij het uitvoeren van dit proces door Workfront API, zie [&#x200B; voorwerpen van de Beweging tussen  [!DNL Workfront]  milieu&#39;s gebruikend  [!DNL Workfront]  API &#x200B;](/help/quicksilver/administration-and-setup/set-up-workfront/workfront-testing-environments/environment-promotion.md).

[&#x200B; Bekijk een videodemonstratie van deze eigenschap &#x200B;](https://video.tv.adobe.com/v/3429735/){target=_blank}

## Ondersteunde objecten voor milieubescherming

Het milieu bevorderend vermogen is bedoeld om de capaciteit te verstrekken om op configuratie betrekking hebbende voorwerp van één milieu aan een andere te bewegen. Dit zijn objecten die kunnen worden geconfigureerd, zoals projecten, teams of aangepaste formulieren.

Omdat de bevordering van het milieu objecten configuratie behandelt, zijn de transactionele voorwerpen (voorwerpen die vaak veranderen of die sterk van gebruiksgeval afhankelijk zijn) niet inbegrepen. Voorbeelden van transactieobjecten zijn documenten, problemen, verzoeken, updates en proefdrukbeslissingen.

* [Werkobjecten](#work-objects)
* [Objecten rapporteren](#reporting-objects)
* [Aangepaste gegevensobjecten](#custom-data-objects)
* [Organisatie-objecten](#organization-objects)
* [Andere configuratieobjecten](#other-configuration-objects)


### Werkobjecten

| Promoteerbaar object | Opgenomen promoteerbare gekoppelde objecten |
| --- | --- |
| Project (PROJ) | De Taak van het project <br> 1&rbrace; Taak <br> Predecessor <br> Onderneming <br> het Tarief van de Overschrijving van de Groep <br> <br> Rol van het Team <br> het Proces van de Goedkeuring <br> Stap van de Goedkeuring 11&rbrace; Stap <br> Plan van de Stap 13&rbrace; Dag van de Werkvoorraad <br> Werkgroep 16&rbrace; Het Onderwerp van de rij <br> Verpletterend Regel <br> Mijlpad van de Mijlsteen <br> Mijlsteen <br> het Pool van het Type van uur <br> Categorie <br> CategorieParameter <br> de Groep van de Parameter 25&rbrace; <br> Optie van de Parameter <br> Logica van de Categorie<br><br><br><br><br><br><br><br><br> |
| Sjabloon (TMPL) | De Taak van het Malplaatje <br> Taak van het Malplaatje <br> Predecessor van de Taak van het Malplaatje <br> Bedrijf <br> het Tarief van de Overschrijving van de Groep <br> Rol van de Groep <br> 8&rbrace; van de Goedkeuring <br> Stap van de Goedkeuring 11&rbrace; Stap van de Stap van de Stap <br> Dag van de Werkvoorraad <br> Werkgroep 15&rbrace; <br> het Onderwerp van de Rij <br> Verpletterend 18&rbrace; Mijlpad van de Regel <br> Mijlsteen <br> het Type van het Huur <br> Pool van het Middel <br> CategorieParameter <br> de 25&rbrace; 26&rbrace; Optie van de Parameter van de Parameter <br> Logica van de Categorie<br><br><br><br><br><br><br><br><br><br><br> |

### Objecten rapporteren

| Promoteerbaar object | Opgenomen promoteerbare gekoppelde objecten |
| --- | --- |
| Lay-outsjabloon (UITMPL) | Het Malplaatje van de lay-out &lbrace;<br> Kalender <br> Sectie van de Kalender <br> Externe Pagina <br> het Rapport <br> van de Filter <br> Groepering <br> van de Mening <br> van de Parameter <br> Groep<br> |
| Dashboard (PTLTAB) | De Sectie van de Kalender van het dashboard <br> &lbrace;<br> Externe Pagina <br> van het Rapport <br> <br> Groepering <br> van de Mening <br> Parameter<br> |
| Kalender (CALEND) | Kalender <br> Sectie van de Kalender |
| Externe pagina (EXTSEC) | Externe pagina |
| Rapport (PTLSEC) | Het verslag <br> Groepering van de 1&rbrace; Filter <br> Mening <br> Parameter<br> |
| Filter (UIFT) | Filter <br> Parameter |
| Groeperen (UIGB) | <br> Parameter groeperen |
| Weergave (UIVW) | Weergave <br> Parameter |

### Aangepaste gegevensobjecten

| Promoteerbaar object | Opgenomen promoteerbare gekoppelde objecten |
| --- | --- |
| Categorie (CTGY) | De Categorie <br> Parameter van de 1&rbrace; <br> Parameter van de Groep <br> Optie van de Parameter van de Partij <br> Categorie van de Logische Logica van de Vertoning van de Categorie <br> Groep van de Groep van de Categorie &lbrace;<br> |
| Parameter (PARAM) | De Optie van de Parameter <br> |
| Parametergroep (PGRP) | Parametergroep |

### Organisatie-objecten

| Promoteerbaar object | Opgenomen promoteerbare gekoppelde objecten |
| --- | --- |
| Groep (GROEP) | De Groep <br> Subgroepen (tot 5 niveaus) * <br> Categorie <br> CategorieParameter <br> de Groep van de Parameter <br> Optie van de Parameter <br> Logische van de Vertoning van de Categorie<br> |
| Rol (ROLE) | Rol |
| Team (TEAM) | Team <br> Groep |
| Bedrijf (CMPY) | Het bedrijf <br> het Tarief van de Overschrijving <br> Categorie <br> <br> Parameter <br> de Groep van de Parameter <br> Parameter <br> van de Categorie van de Logica van de Vertoning <br> Groep |
| Portfolio (PORT) | Portfolio <br> van de Groep van het 1&rbrace; &lbrace;<br> Categorie <br> <br> Parameter <br> van de Parameter {<br> Optie van de Parameter van de 6} <br> Logische van de Vertoning van de Categorie<br> |
| Programma (PRGM) | Het programma <br> van de Groep van Portfolio <br> <br> Categorie <br> Parameter <br> Van de Groep van de Parameter &lbrace;<br> Logische van de Vertoning van de Categorie van de Categorie van de Optie van de Partij van de Parameter &lbrace;<br><br> |

### Andere configuratieobjecten

| Promoteerbaar object | Opgenomen promoteerbare gekoppelde objecten |
| --- | --- |
| Goedkeuringsproces (ARVPRC) | De Stap van de Stap van de Goedkeuring van het Proces van de Goedkeuring <br> <br> Stap <br> Rol <br> van het Team <br> Groep<br> |
| Schema (SCHED) | De Groep van de Dag van het Werk van het Programma <br><br> |
| Mijlpad (MPATH) | Mijlpad <br> Mijlsteen |
| Tijdbladprofiel (TSPRO) | Het Type van het Profiel van het Tijdopmaakprofiel <br> |
| Uurtype (URT) | Uurtype |
| Type kosten (EXPTYP) | Type uitgave |
| Type risico (RSKTYP) | Type risico |
| Bronpool (RSPL) | Bronpool |
| Toegangsniveau (ACSLVL) | Toegangsniveau |
| Rate Card (RTCRD) | Creditcard |
| Locatie/classificator (CLSF) | Locatie/classificator |
| Bedrijfsvoorschriften (BSNRUL) | Zakelijke regels |

\* Momenteel niet beschikbaar

<!--

>[!NOTE]
>
>Actions (ignore, select existing, and create new) are available on the following objects:
>
>* Role
>* Team
>* Company
>* Group

-->

## Status van milieubescherming

De bevorderingspakketten van het milieu gaan door verscheidene statussen aangezien zij worden gecreeerd en bereid om zich tussen milieu&#39;s te bewegen. Deze statussen worden weergegeven in uw lijst met pakketten in Workfront of in de API-reacties als u de Workfront API gebruikt.

Deze statussen zijn onder andere:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>UNASSEMBED</td> 
   <td><p>Deze status wordt automatisch toegewezen en vertegenwoordigt een pakket dat is opgeslagen maar nog niet is samengesteld. </p><p>Deze status kan niet rechtstreeks door een gebruiker worden ingesteld.</p></td> 
  </tr> 
  <tr> 
   <td>VERZAMELING</td> 
   <td><p>Deze status wordt automatisch toegewezen tijdens het samenstellen van objecten. </p><p>Bij samenstellen wordt verwezen naar het geautomatiseerde proces voor het identificeren van objecten en subobjecten die in een pakket moeten worden opgenomen en het toevoegen van die objecten en hun gegevens aan het pakket.</p><p>Deze status kan niet rechtstreeks door een gebruiker worden ingesteld.</p></td> 
  </tr> 
  <tr> 
   <td>CONCEPT</td> 
   <td><p>Deze status wordt toegewezen aan het einde van een assemblageproces of bij het maken van een leeg promotiepakket.</p><p>Het is mogelijk dat een gebruiker het promotiepakket terugzet naar deze status.</p><p>In deze status kan het promotiepakket niet in een omgeving worden geïnstalleerd.</p></td> 
  </tr> 
  <tr> 
   <td>TESTS</td> 
   <td><p>Met deze status kan een promotiepakket worden geïnstalleerd in elke voorvertoning of aangepaste vernieuwingssandbox. In deze status kan het pakket niet worden geïnstalleerd in Production.</p></td> 
  </tr> 
  <tr> 
   <td>ACTIEF</td> 
   <td><p>Met deze status kan een promotiepakket worden geïnstalleerd in elke omgeving, inclusief Productie.</p><p>Wanneer de pakketstatus is ingesteld op ACTIEF, wordt de datum <code>publishedAt</code> automatisch ingesteld op de huidige tijdstempel van de aanvraag.</p></td> 
  </tr> 
  <tr> 
   <td>UITGESCHAKELD</td> 
   <td><p>Deze status wordt gebruikt om eerder gebruikte promotiepakketten te verbergen die in de toekomst niet in een omgeving worden geïnstalleerd.</p><p>Wanneer een pakket zich in deze status bevindt, kan het niet in een omgeving worden geïnstalleerd.</p><p>Wanneer de pakketstatus is ingesteld op DISABLED, wordt de datum <code>retiredAt</code> automatisch ingesteld op de huidige tijdstempel van de aanvraag.</p><p>Het gebruik van deze status wordt aangeraden bij het gebruik van het <code>DELETE /package</code> -eindpunt omdat het kan worden opgehaald en de installatiegeschiedenis bewaard blijft voor alle implementaties die met dit pakket zijn gemaakt.</p></td> 
  </tr> 
  <tr> 
   <td>ASSEMBLING_FAILED</td> 
   <td><p>Het promotiepakket wordt automatisch in deze status geplaatst als de ASSEMBLING-fase mislukt.</p><p>Als u het pakket wilt terugbrengen naar het ASSEMBLING-werkgebied, moet u het assemblageproces opnieuw activeren.</p><p>Voor details bij het assembleren van een pakket, zie de sectie <a href="https://experienceleague.adobe.com/en/docs/workfront/using/administration-and-setup/set-up-wf/testing-environments/environment-promotion-create-package#edit-or-assemble-an-existing-package"> uitgeven of een bestaand pakket </a> in artikel assembleren creeer of geef een pakket van de milieubevordering uit.</td> 
  </tr> 
  </tbody> 
</table>

## Bronnen

* Voor FAQs betreffende milieubevordering, zie [&#x200B; Veelgestelde vragen van de Bevordering van het Milieu &#x200B;](/help/quicksilver/administration-and-setup/set-up-workfront/workfront-testing-environments/environment-promotion-faq.md)
* Voor het oplossen van problemenaanbevelingen, zie [&#x200B; het bevorderingsoplossen van problemen van het Milieu &#x200B;](/help/quicksilver/administration-and-setup/set-up-workfront/workfront-testing-environments/environment-promotion-troubleshooting.md)


