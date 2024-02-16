---
content-type: release-notes
keywords: notities,driemaandelijks,bijwerken
navigation-topic: 2021-4-release-activity
title: 21.4 Overzicht van de release
description: Deze pagina bevat informatie over de functionaliteit voor zowel Adobe Workfront Classic als de nieuwe Adobe Workfront-ervaring die is opgenomen in de release 21.4. om u te helpen productiviteit en samenwerking ontgrendelen.[Eén regel in de handel brengen voor de release]
author: Luke
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: 0897b269-c6f3-4b63-8956-b7f9fbe0a553
source-git-commit: f1e463c90641f9221228e335b583cab72762b3bd
workflow-type: tm+mt
source-wordcount: '4717'
ht-degree: 0%

---

# 21.4 Overzicht van de release

Deze pagina bevat informatie over de functionaliteit voor zowel Adobe Workfront Classic als de nieuwe Adobe Workfront-ervaring die is opgenomen in de release 21.4.

<!--
<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
to help you unlock productivity and collaboration.
</MadCap:conditionalText>
-->

<!--
<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
[Marketing one-liner for the release]
</MadCap:conditionalText>
-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">These enhancements are currently available in the Preview environment. As the 21.4 release nears its planned Production release the week of October 4, 2021
<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
in October 2021
</MadCap:conditionalText>
, this page will be updated with all functionality included with 21.4.</p>
-->

Deze verbeteringen zijn beschikbaar gesteld in de productieomgeving van 4 oktober 2021.

<!--
<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
These enhancements are currently available in the Preview environment and will be made available in the Production environment the week of October 4, 2021
<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
,
</MadCap:conditionalText>
</MadCap:conditionalText>
-->

<!--
<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
unless otherwise specifiedthe week of May 10, 2021.
</MadCap:conditionalText>


For specific release dates and times for each cluster, see the [Adobe Workfront status page](https://status.adobe.com/en/products/5943) on [status.adobe.com](http://status.adobe.com/). You must log in to see specific release times.

-->

## Verbeteringen voor Adobe Workfront

* [Beheerdersverbeteringen](#administrator-enhancements)
* [Verbeteringen voor mobiele apparaten](#agile-enhancements)
* [Projectverbeteringen](#project-enhancements)
* [Verbeteringen voor beheer van bronnen](#resource-management-enhancements)
* [Verbeteringen rapporteren](#reporting-enhancements)
* [Verbeteringen aan verzoeken](#requests-enhancements)
* [Verbeteringen voor proefdrukken](#proofing-enhancements)
* [Verbeteringen voor integratie](#integration-enhancements)
* [Verbeteringen voor mobiele apparaten](#mobile-enhancements)
* [Andere verbeteringen](#other-enhancements)

### Beheerdersverbeteringen {#administrator-enhancements}

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p><strong>Functie</strong> </p> </td> 
   <td> <p><strong>Datums en omgevingen vrijgeven</strong> </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.4-release-activity/21-4-admin-enhancements.md#for" class="MCXref xref" xrefformat="{para}">Voor beheerders: zie welke groepen aan een goedkeuringsproces worden geassocieerd</a> </p> <p>Om u te helpen te weten komen welke groepen met de goedkeuringsprocessen in uw systeem worden geassocieerd, hebben wij een kolom van de Naam van de Groep aan de Standaardmening op de pagina van Goedkeuringen in Opstelling toegevoegd. Nu kunt u deze gegevens weergeven zonder dat u een aangepaste weergave hoeft te maken.</p> </td> 
   <td> <p><b>Beschikbaar op deze data:</b> </p> <p>Voorvertoning release: 9 september 2021<br></p> <p>Productieversie: met de release van 21.4</p> <p><strong>Beschikbaar in deze omgevingen:</strong> </p> <p>De nieuwe Adobe Workfront-ervaring </p> <p>Adobe Workfront Classic </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.4-release-activity/21-4-admin-enhancements.md#new" class="MCXref xref" xrefformat="{para}">Nieuw voor beheerders: de groepen kunnen hun eigen timesheet en uurvoorkeur vormen</a> </p> <p>In een grote organisatie, zouden sommige groepen timesheet en uurvoorkeur onafhankelijk kunnen moeten vormen om hun unieke werkschema's te passen, eerder dan het erven van de voorkeur die door een beheerder op het systeemniveau wordt gevormd. Nu kunnen de beheerders van Workfront een timesheet en een uurvoorkeur voor alle groepen in het systeem ontgrendelen zodat zij het op hun kunnen vormen.</p> <p>Deze mogelijkheid is onlangs ook toegevoegd voor projectvoorkeuren en voor voorkeuren voor taken en uitgaven.</p> </td> 
   <td> <p><b>Beschikbaar op deze data:</b> </p> <p>Voorvertoning release: 9 september 2021<br></p> <p>Productieversie: met de release van 21.4 <span style="color: #ff0000;">(Aanvankelijk alleen beschikbaar in Productie voor klanten op Cluster 4)</span></p> <p><strong>Beschikbaar in deze omgevingen:</strong> </p> <p>De nieuwe Adobe Workfront-ervaring </p> <p>Adobe Workfront Classic </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.4-release-activity/21-4-admin-enhancements.md#new2" class="MCXref xref" xrefformat="{para}">Nieuw voor Workfront-beheerders: lay-outsjablonen configureren voor gebruikers met automatische provisioning in de nieuwe Workfront-ervaring</a> </p> <p>Nu kunt u lay-outmalplaatjes in de nieuwe ervaring van Workfront voor auto-provisioned gebruikers vormen. In het vervolgkeuzemenu Workfront-gebruikerskenmerken waarin u gebruikerskenmerken toewijst (Setup &gt; Systeem &gt; Single Sign-On), is een nieuw menu-item "NWE Layout Template" nu beschikbaar voor het maken van deze configuratie. Eerder, kon u lay-outmalplaatjes voor auto-provisioned gebruikers slechts in Workfront Klassiek vormen.</p> </td> 
   <td> <p><b>Beschikbaar op deze data:</b> </p> <p>Voorvertoning release: 9 september 2021<br></p> <p>Productieversie: met de release van 21.4</p> <p><strong>Beschikbaar in deze omgevingen:</strong> </p> <p>De nieuwe Adobe Workfront-ervaring </p> <p>Adobe Workfront Classic </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.4-release-activity/21-4-admin-enhancements.md#new3" class="MCXref xref" xrefformat="{para}">In het nieuwe veld worden de groepen weergegeven waartoe uw gebruikers behoren</a> </p> <p>Nu is het gemakkelijk om te weten te komen tot welke groepen uw gebruikers behoren. In een rapport of een weergave waarin gebruikers worden vermeld, kunt u een kolom maken met het nieuwe veld Andere groepen. In dit veld worden de groepen weergegeven waarin elke gebruiker lid is.</p> </td> 
   <td> <p><b>Beschikbaar op deze data:</b> </p> <p>Voorvertoning release: 9 september 2021<br></p> <p>Productieversie: met de release van 21.4</p> <p><strong>Beschikbaar in deze omgevingen:</strong> </p> <p>De nieuwe Adobe Workfront-ervaring </p> <p>Adobe Workfront Classic </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.4-release-activity/21-4-admin-enhancements.md#blueprin" class="MCXref xref" xrefformat="{para}">Op de pagina Blauwdrukdetails wordt nu een afbeelding weergegeven</a> </p> <p>De detailspagina voor elke blauwdruk toont nu een beeld van het projectmalplaatje dat met de blauwdruk geïnstalleerd is. De afbeelding bevat een voorvertoning van de blauwdrukinhoud, zodat u weet wat u gaat installeren. U kunt desgewenst een voorvertoning van de volledige afbeelding weergeven in de browser of de afbeelding downloaden.</p> </td> 
   <td><strong>Beschikbaar op deze data:</strong> <p>Voorvertoning release: 9 september 2021<br></p> <p>Productieversie: met de release van 21.4</p> <p><strong>Beschikbaar in deze omgevingen:</strong> </p> <p>De nieuwe Adobe Workfront-ervaring </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.4-release-activity/21-4-admin-enhancements.md#blueprin2" class="MCXref xref" xrefformat="{para}">Voorkeuren voor blauwdrukken voor nieuwe uitgaven</a> </p> <p>Voor sommige blauwdrukken zijn nu nieuwe uitgiftevoorkeuren beschikbaar. Ze worden standaard geïnstalleerd, maar u kunt de installatie van de voorkeuren uitschakelen wanneer u de installatiegegevens configureert.</p> <p>De voorkeur omvat groepen van het rijonderwerp, rijonderwerpen, en het verpletteren van regels om de correcte informatie te verzamelen wanneer een kwestie of een verzoek wordt voorgelegd, en de kwestie of het verzoek naar de correcte baanrol of het team te verzenden. Het gebruik van de voorkeuren draagt bij aan consistentie in de manier waarop nieuwe problemen of verzoeken worden vastgelegd voor uw projecten.</p> <p>Merk op dat het gebruiken van deze voorkeur niet de projecten maakt die van het malplaatje in verzoekrijen worden gecreeerd.</p> </td> 
   <td><strong>Beschikbaar op deze data:</strong> <p>Voorvertoning release: 9 september 2021<br></p> <p>Productieversie: met de release van 21.4</p> <p><strong>Beschikbaar in deze omgevingen:</strong> </p> <p>De nieuwe Adobe Workfront-ervaring </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.4-release-activity/21-4-admin-enhancements.md#new4" class="MCXref xref" xrefformat="{para}">Nieuw voor groepsbeheerders: onlangs verwijderde en herstelde items van een groep weergeven en beheren</a> </p> <p>We maken het nog steeds eenvoudiger om uw groepen en de bijbehorende objecten op één locatie te beheren. Nu kunt u de onlangs verwijderde en herstelde items van een groep weergeven en bewerken in het gebied Groepen. Hierdoor hoeft u niet naar het gebied Onlangs verwijderd of Onlangs hersteld in Setup te gaan om deze items te beheren. En het houdt de lijst van groepspunten u met werkt gescheiden van andere schrapte en herstelde punten in het systeem.</p> </td> 
   <td><strong>Beschikbaar op deze data:</strong> <p>Voorvertoningsrelease: 26 augustus 2021<br></p> <p>Productieversie: met de release van 21.4</p> <p><strong>Beschikbaar in deze omgevingen:</strong> </p> <p>De nieuwe Adobe Workfront-ervaring </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.4-release-activity/21-4-admin-enhancements.md#new5" class="MCXref xref" xrefformat="{para}">Nieuw voor groepsbeheerders: groepsvoorkeuren zijn nu van invloed op groepssjablonen</a> </p> <p>Het is nu gemakkelijker om ervoor te zorgen dat de projectmalplaatjes van uw groep aan de behoeften van uw groep voldoen. Wanneer u een nieuw projectmalplaatje aan een groep op het tijdstip toewijst dat u het creeert, erft het malplaatje diverse montages van het project en de taakvoorkeur van de groep.</p> <p>Wanneer u een nieuwe malplaatjetaak binnen een projectmalplaatje creeert dat met een groep wordt geassocieerd, erft de malplaatjetaak diverse montages van de de taakvoorkeur van de groep.</p> <p>Eerder, werden de projectmalplaatjes en de taken van het projectmalplaatje geërft deze montages van het project en de taakvoorkeur die op het systeemniveau wordt geplaatst.</p> <p>Als u een malplaatje of malplaatjetaak zonder een groep-voor voorbeeld, van de belangrijkste pagina van Malplaatjes creeert-hierboven montages van het project en de taakvoorkeur op systeemniveau worden geërft. Nochtans, als u later een groep aan het malplaatje of malplaatjetaak toewijst, beïnvloeden de voorkeur van de groep niet het.</p> </td> 
   <td> <p>Voorvertoningsrelease: 26 augustus 2021<br></p> <p>Productieversie: met de release van 21.4</p> <p><strong>Beschikbaar in deze omgevingen:</strong> </p> <p>De nieuwe Adobe Workfront-ervaring </p> <p>Adobe Workfront Classic </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.4-release-activity/21-4-admin-enhancements.md#new6" class="MCXref xref" xrefformat="{para}">Nieuw voor beheerders: zoek op welke aangepaste formulieren een aangepast veld gebruiken</a> </p> <p>Het is nu eenvoudiger om een aangepast veld te wijzigen in een aangepast formulier. Met één klik in het aangepaste formulier kunt u meer informatie vinden over andere aangepaste formulieren die ook het veld gebruiken. Het is belangrijk om te beoordelen of die formulieren aanpassingen nodig hebben om correct te blijven werken nadat u de wijziging hebt aangebracht.</p> </td> 
   <td><strong>Beschikbaar op deze data:</strong> <p>Voorvertoningsrelease: 19 augustus 2021<br></p> <p>Productieversie: met de release van 21.4</p> <p><strong>Beschikbaar in deze omgevingen:</strong> </p> <p>De nieuwe Adobe Workfront-ervaring </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.4-release-activity/21-4-admin-enhancements.md#new7" class="MCXref xref" xrefformat="{para}">Nieuw voor groepsbeheerders: Project, taak en uitgiftevoorkeuren voor een groep vergrendelen en ontgrendelen</a> </p> <p>Nu kunt u ervoor zorgen dat iedereen in uw groep en in zijn subgroepen het zelfde plaatsen voor een project, een taak, of een uitgiftevoorkeur gebruikt. Nadat een beheerder van Workfront een voorkeur op het systeemniveau ontgrendelt, kunt u het vormen en dan het voor uw groep sluiten. Hoewel u een gesloten groepsvoorkeur nog kunt aanpassen, kunnen de beheerders van lagere subgroepen dit niet afzonderlijk voor hun groepen doen.</p> </td> 
   <td><strong>Beschikbaar op deze data:</strong> <p>Voorvertoningsrelease: 12 augustus 2021<br></p> <p>Productieversie: met de release van 21.4</p> <p><strong>Beschikbaar in deze omgevingen:</strong> </p> <p>De nieuwe Adobe Workfront-ervaring </p> <p>Adobe Workfront Classic </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.4-release-activity/21-4-admin-enhancements.md#new8" class="MCXref xref" xrefformat="{para}">Nieuw voor groepsbeheerders: sjablonen maken en bewerken in het gebied Groepen</a> </p> <p>We maken het nog steeds eenvoudiger om uw groepen en de bijbehorende objecten op één locatie te beheren. Nu kunt u met de malplaatjes van een groep van het gebied van Groepen in Opstelling bekijken en werken. Hierdoor hoeft u niet naar het gebied Sjablonen te gaan om de sjablonen van een groep te beheren. En het houdt de lijst van groepsmalplaatjes u aan werkt gescheiden van de anderen door het systeem.</p> </td> 
   <td><strong>Beschikbaar op deze data:</strong> <p>Voorvertoningsrelease: 12 augustus 2021<br></p> <p>Productieversie: met de release van 21.4</p> <p><strong>Beschikbaar in deze omgevingen:</strong> </p> <p>De nieuwe Adobe Workfront-ervaring </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.4-release-activity/21-4-admin-enhancements.md#enter" class="MCXref xref" xrefformat="{para}">Gegevens invoeren en opslaan in één aangepast formulier tegelijk</a> </p> <p>Het is nu gemakkelijker om informatie in de sectie Details voor een voorwerp te verstrekken: Type en sparen informatie in één enkel douanegebied of uitbreidbaar gebied (zoals Overzicht en Financiën), zelfs als de vereiste gebieden in andere douaneformulieren op het voorwerp nog niet worden ingevuld.</p> <p>Eerder, toen u informatie in één douaneformulier of uitbreidbaar gebied voor een voorwerp inging, gingen alle douaneformulieren in bijlage aan het voorwerp op bewerkingswijze en al hun vereiste gebieden moesten worden voltooid alvorens u uw veranderingen kon bewaren. Dit was een probleem als u een vereist veld niet kon voltooien omdat het voor een andere gebruiker was bedoeld.</p> </td> 
   <td><strong>Beschikbaar op deze data:</strong> <p>Voorvertoningsrelease: 22 juli 2021<br></p> <p>Productieversie: met de release van 21.4</p> <p><strong>Beschikbaar in deze omgevingen:</strong> </p> <p>De nieuwe Adobe Workfront-ervaring </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.4-release-activity/21-4-admin-enhancements.md#new9" class="MCXref xref" xrefformat="{para}">Nieuw voor groepsbeheerders: statussen voor een groep op elk niveau maken en beheren</a> </p> <p>Om het voor alle niveaus van een organisatie gemakkelijker te maken om hun werkschema's onafhankelijk te beheren en te controleren, hebben wij de capaciteit geïntroduceerd om statussen voor subgroepen tot stand te brengen en te beheren. </p> </td> 
   <td><strong>Beschikbaar op deze data:</strong> <p>Voorvertoningsrelease: 3 juni 2021 (tijdens de releasecyclus van 21.3)<br></p> <p>Productieversie: 22 juli 2021</p> <p><strong>Beschikbaar in deze omgevingen:</strong> </p> <p>De nieuwe Adobe Workfront-ervaring </p> <p>Adobe Workfront Classic </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.4-release-activity/21-4-admin-enhancements.md#new10" class="MCXref xref" xrefformat="{para}">Nieuw voor Workfront-beheerders: Migreer lay-outsjablonen van Workfront Classic naar uw nieuwe Workfront-ervaring</a> </p> <p>Om u te helpen lay-outsjablonen te beheren terwijl uw gebruikers overstappen op het gebruik van de nieuwe Workfront-ervaring, hebben we een knop gemaakt waarmee u lay-outsjablonen kunt migreren van Workfront Classic naar de nieuwe ervaring zonder op de klantenondersteuning van Workfront te vertrouwen.</p> <p>Eerder kon alleen Workfront Customer Support uw lay-outsjablonen migreren van Workfront Classic naar de nieuwe Workfront-ervaring.</p> </td> 
   <td><strong>Beschikbaar op deze data:</strong> <p>Voorvertoningsrelease: 1 juli 2021<br></p> <p>Productieversie: 15 juli 2021</p> <p><strong>Beschikbaar in deze omgevingen:</strong> </p> <p>De nieuwe Adobe Workfront-ervaring </p> <p>Adobe Workfront Classic </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.4-release-activity/21-4-admin-enhancements.md#when" class="MCXref xref" xrefformat="{para}">Wanneer het associëren van een malplaatje met een groep, selecteer een proces van de groepsgoedkeuring in de Details van de Rij en de Onderwerpen van de Rij</a> </p> <p>We hebben een nieuwe optie toegevoegd aan het proces waarbij een sjabloon aan een groep wordt gekoppeld. Nu kunt u groep-specifieke goedkeuringsprocessen voor kwesties in de Details van de Rij van het malplaatje of in één van zijn Onderwerpen van de Rij selecteren.</p> <p>In 21.3, toen wij de capaciteit toevoegden om een groepsmalplaatje met een groep te associëren, kon u een groep-specifiek goedkeuringsproces in het malplaatje selecteren, maar u kon dit niet in de Details van de Rij van het malplaatje of de Onderwerpen van de Rij doen.</p> </td> 
   <td><strong>Beschikbaar op deze data:</strong> <p>Voorvertoningsrelease: 1 juli 2021<br></p> <p>Productieversie: met de release van 21.4</p> <p><strong>Beschikbaar in deze omgevingen:</strong> </p> <p>De nieuwe Adobe Workfront-ervaring </p> <p>Adobe Workfront Classic </p> </td> 
  </tr> 
 </tbody> 
</table>

### Projectverbeteringen {#project-enhancements}

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p><strong>Functie</strong> </p> </td> 
   <td> <p><strong>Datums en omgevingen vrijgeven</strong> </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.4-release-activity/21-4-project-enhancements.md#include" class="MCXref xref" xrefformat="{para}">Afbeeldingen opnemen in updates</a> </p> <p>Op het tabblad Updates van een object kunt u nu afbeeldingen toevoegen door op het pictogram Afbeelding op de werkbalk te klikken. U kunt ook een afbeelding naar het updategebied slepen. De Workfront-beheerder moet het toevoegen van afbeeldingen inschakelen voordat u het afbeeldingspictogram kunt zien.</p> <p>U kunt afbeeldingen zowel in updates als in reacties toevoegen. Een afbeeldingsminiatuur in de update geeft aan dat ontvangers een voorvertoning van de afbeelding in de browser kunnen bekijken of deze kunnen downloaden, en uit e-mail- en in-app-meldingen blijkt dat de afbeeldingen aan de update zijn gekoppeld.</p> <p>Eerder was de enige manier om een afbeelding te delen in Workfront dat u deze aan een object koppelde als een document. Afbeeldingen die zijn toegevoegd op het tabblad Updates, zijn alleen beschikbaar op dat tabblad en niet op het tabblad Documenten.</p> <p>Voordat Workfront-gebruikers afbeeldingen kunnen opnemen in updates, moet deze functie eerst worden ingeschakeld door de Adobe Workfront-beheerder.</p> </td> 
   <td><strong>Beschikbaar op deze data:</strong> <p>Voorvertoning release: 9 september 2021<br></p> <p>Productieversie: met de release van 21.4</p> <p><strong>Beschikbaar in deze omgevingen:</strong> </p> <p>De nieuwe Adobe Workfront-ervaring </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.4-release-activity/21-4-project-enhancements.md#updated" class="MCXref xref" xrefformat="{para}">Bijgewerkt algoritme voor slimme toewijzingen</a> </p> <p>We hebben het algoritme verbeterd dat wordt gebruikt bij het maken van slimme toewijzingen. Met de nieuwe verbetering, bekijkt Workfront de 30 meest recente taken die door het programma geopende gebruiker worden gemaakt om suggesties te doen wanneer zij taken en kwesties toewijzen. De lijst met suggesties kan maximaal 50 gebruikers bevatten. </p> <p>Voorafgaand aan deze verbetering, bezat Workfront de taken op de oudertaken en andere gebruikersattributen met betrekking tot die taken wanneer het adviseren van gebruikers.</p> </td> 
   <td><strong>Beschikbaar op deze data:</strong> <p>Voorvertoning release: 9 september 2021<br></p> <p>Productieversie: met de release van 21.4</p> <p><strong>Beschikbaar in deze omgevingen:</strong> </p> <p>De nieuwe Adobe Workfront-ervaring </p> <p>Adobe Workfront Classic </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.4-release-activity/21-4-project-enhancements.md#new" class="MCXref xref" xrefformat="{para}">Nieuwe ervaring bij het maken van een project op basis van een sjabloon</a> </p> <p>Om uw gebruik van Workfront in overeenstemming te brengen met de nieuwe ervaring van Workfront, hebben wij de interface voor het creëren van een project van malplaatje opnieuw ontworpen. De functionaliteit voor het maken van een project met een sjabloon is niet gewijzigd. Nochtans, omvatten sommige verbeteringen van deze onlangs opnieuw ontworpen interface het volgende:</p> 
    <ul> 
     <li> <p>Sjabloongegevens voorvertonen voordat u deze koppelt</p> </li> 
     <li> <p>Voeg malplaatjes aan een lijst van favorieten tijdens het proces van de projectverwezenlijking toe</p> </li> 
    </ul> <p>Wij hebben de interface voor het creëren van het project bijgewerkt zowel wanneer u het van de Projecten evenals van het gebied van Malplaatjes creeert.</p> </td> 
   <td><strong>Beschikbaar op deze data:</strong> <p>Voorvertoning release: 9 september 2021<br></p> <p>Productieversie: met de release van 21.4</p> <p><strong>Beschikbaar in deze omgevingen:</strong> </p> <p>De nieuwe Adobe Workfront-ervaring </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.4-release-activity/21-4-project-enhancements.md#new2" class="MCXref xref" xrefformat="{para}">Nieuwe ervaring bij het koppelen van sjablonen aan projecten</a> </p> <p>Om uw gebruik van Workfront in overeenstemming te brengen met de nieuwe ervaring van Workfront, hebben wij de interface voor het vastmaken van een malplaatje aan een project opnieuw ontworpen. De functionaliteit voor het koppelen van een sjabloon is niet gewijzigd. Nochtans, zijn er sommige verbeteringen van deze onlangs opnieuw ontworpen interface die het volgende omvatten:</p> 
    <ul> 
     <li> <p>Sjabloongegevens voorvertonen voordat u deze koppelt</p> </li> 
     <li> <p>Sjablonen toevoegen aan een lijst met favorieten tijdens het bijlageproces</p> </li> 
     <li> <p>Alle opties voor het beheer van sjabloon- en projectinstellingen in één doorlopende pagina weergeven</p> </li> 
    </ul> </td> 
   <td><strong>Beschikbaar op deze data:</strong> <p>Voorvertoningsrelease: 26 augustus 2021<br></p> <p>Productieversie: met de release van 21.4</p> <p><strong>Beschikbaar in deze omgevingen:</strong> </p> <p>De nieuwe Adobe Workfront-ervaring </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.4-release-activity/21-4-project-enhancements.md#unified" class="MCXref xref" xrefformat="{para}">Verenigde duur en duureenheidwaarden voor taken</a> </p> <p>Voor een schonere en meer gestroomlijnde gebruikerservaring, hebben wij de waarde van het gebied van de Duur met de duureenheid van tijd samengevoegd. Voorafgaand aan deze verbetering, de eenheid van tijd die op een afzonderlijk drop-down gebied na het gebied van de Duur wordt getoond.</p> <p>Naast de gebieden van de Duur in de de Details van de Taak, geeft Taken en Nieuwe Taakdozen uit, werken wij ook de volgende gebieden bij om deze ervaring aan te passen:</p> 
    <ul> 
     <li> <p>Veld voor duur bij het maken van geavanceerde toewijzingen</p> </li> 
     <li> <p>Het veld Vertraging niveaus bij het maken of bewerken van een taak</p> </li> 
     <li> <p>Frequentieveld bij het maken van een terugkerende taak (binnenkort beschikbaar)</p> </li> 
     <li> <p>Veld labelen bij het toevoegen van een voorganger (binnenkort beschikbaar)</p> </li> 
    </ul> </td> 
   <td><strong>Beschikbaar op deze data:</strong> <p>Voorvertoningsrelease: 19 augustus 2021<br></p> <p>Productieversie: met de release van 21.4</p> <p><strong>Beschikbaar in deze omgevingen:</strong> </p> <p>De nieuwe Adobe Workfront-ervaring </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.4-release-activity/21-4-project-enhancements.md#disable" class="MCXref xref" xrefformat="{para}">Inline toevoegen van problemen in projecten uitschakelen</a> </p> <p>Om ervoor te zorgen dat de gebruikers nauwkeurige informatie verstrekken wanneer het toevoegen van kwesties aan projecten door een uitgifteformulier in te vullen, hebben wij een nieuw plaatsen geïntroduceerd die u toestaat om te beheren of zij kwesties aan een project of zijn taken kunnen inline toevoegen. Deze instelling is standaard ingeschakeld in het gebied Instellingen nieuwe uitgave van het vak Project bewerken. Als u deze optie uitschakelt, wordt de optie Meer problemen toevoegen in de sectie Problemen van een project grijs weergegeven zodat gebruikers geen problemen meer in de lijst kunnen toevoegen. De gebruikers kunnen nog kwesties aan de projecten toevoegen door de Nieuwe optie van de Uitgave in de sectie van Kwesties te gebruiken of een verzoekrij te gebruiken als voor het project wordt gevormd.</p> </td> 
   <td><strong>Beschikbaar op deze data:</strong> <p>Voorvertoningsrelease: 5 augustus 2021<br></p> <p>Productieversie: met de release van 21.4</p> <p><strong>Beschikbaar in deze omgevingen:</strong> </p> <p>De nieuwe Adobe Workfront-ervaring </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.4-release-activity/21-4-project-enhancements.md#custom" class="MCXref xref" xrefformat="{para}">Verbeterde weergave van aangepaste velden voor selectievakjes en keuzerondjes</a> </p> <p>Het weergeven en selecteren van opties voor selectievakjes en keuzerondjes in aangepaste formulieren is nu eenvoudiger geworden. Een aangepast veld met veel opties voor selectievakjes of keuzerondjes wordt nu in meerdere kolommen op de pagina weergegeven. Eerder werden ze in één kolom weergegeven. Hiervoor moesten gebruikers extra schuiven om het formulier in te vullen.</p> <p>Dit hangt af van de positie van de velden in het aangepaste formulier. Als u een ander veld in dezelfde rij plaatst met het selectievakje of keuzerondje, hebben de opties mogelijk slechts voldoende horizontale ruimte om in één kolom weer te geven.</p> </td> 
   <td><strong>Beschikbaar op deze data:</strong> <p>Voorvertoningsrelease: 29 juli 2021<br></p> <p>Productieversie: met de release van 21.4</p> <p><strong>Beschikbaar in deze omgevingen:</strong> </p> <p>De nieuwe Adobe Workfront-ervaring </p> </td> 
  </tr> 
 </tbody> 
</table>

### Verbeteringen voor beheer van bronnen {#resource-management-enhancements}

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p><strong>Functie</strong> </p> </td> 
   <td> <p><strong>Datums en omgevingen vrijgeven</strong> </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.4-release-activity/21-4-resource-management-enhancements.md#make" class="MCXref xref" xrefformat="{para}">Snelle toewijzingen uitvoeren in Workload Balancer</a> </p> <p>U kunt bronnen in de werklastbalans nu op efficiënte wijze in evenwicht brengen met een minimale klik door een item uit het niet-toegewezen gebied te slepen en neer te zetten op de regel van een gebruiker in het toegewezen gebied. Met slepen en neerzetten kunt u de toewijzing van items aan gebruikers ongedaan maken en deze naar het niet-toegewezen gebied verplaatsen en naar andere gebruikers verplaatsen. </p> <p>Vóór deze verbetering, kon u punten slechts toewijzen door het Meer menu van een taak of een kwestie te klikken, dan gebruikend de Assign optie. Nu, de Geplande Uren die aan de gebruiker worden toegewezen bijwerken in real time terwijl het slepen van de taken.</p> </td> 
   <td><strong>Beschikbaar op deze data:</strong> <p>Voorvertoning release: 9 september 2021<br></p> <p>Productieversie: met de release van 21.4</p> <p><strong>Beschikbaar in deze omgevingen:</strong> </p> <p>De nieuwe Adobe Workfront-ervaring </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.4-release-activity/21-4-resource-management-enhancements.md#new" class="MCXref xref" xrefformat="{para}">Nieuwe standaardoptie voor werklastverdeling</a> </p> <p>In het kader van onze inspanningen om planning te vervangen en van het belangrijkste hulpmiddel voor het toewijzen van bronnen in Workload Balancer Workfront te maken, hebben we de Workfront Balancer tot de standaardoptie voor alle nieuwe gebruikers gemaakt. Momenteel, is het plannen de standaardoptie. Deze wijziging is van toepassing op alle gebieden waar u toegang hebt tot de planning, waaronder het gebied Bronnen (in de nieuwe Adobe Workfront-ervaring) of het gebied Mensen (in Adobe Workfront Classic), en op project- en teamniveau.</p> </td> 
   <td><strong>Beschikbaar op deze data:</strong> <p>Voorvertoning release: 9 september 2021<br></p> <p>Productieversie: met de release van 21.4</p> <p><strong>Beschikbaar in deze omgevingen:</strong> </p> <p>De nieuwe Adobe Workfront-ervaring </p> <p>Adobe Workfront Classic </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.4-release-activity/21-4-resource-management-enhancements.md#new2" class="MCXref xref" xrefformat="{para}">Nieuwe filterervaring in werklastverdeling</a> </p> <p>We hebben de filterervaring in Workload Balancer opnieuw ontworpen, zodat deze de volgende extra functionaliteit bevat:</p> 
    <ul> 
     <li> <p>Eenvoudigere, gestroomlijnde gebruikersinterface die aansluit bij de nieuwe Workfront-ervaring</p> </li> 
     <li> <p>Aanvullende velden waarop u kunt filteren</p> </li> 
     <li> <p>De mogelijkheid om een filter te dupliceren</p> </li> 
     <li> <p>Filters delen met andere gebruikers</p> </li> 
    </ul> </td> 
   <td><strong>Beschikbaar op deze data:</strong> <p>Voorvertoningsrelease: 16 september 2021<br></p> <p>Productieversie: met de release van 21.4</p> <p><strong>Beschikbaar in deze omgevingen:</strong> </p> <p>De nieuwe Adobe Workfront-ervaring </p> </td> 
  </tr> 
 </tbody> 
</table>

### Verbeteringen voor mobiele apparaten {#agile-enhancements}

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p><strong>Functie</strong> </p> </td> 
   <td> <p><strong>Datums en omgevingen vrijgeven</strong> </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.4-release-activity/21-4-agile-enhancements.md#user" class="MCXref xref" xrefformat="{para}">Toewijzingen van gebruikers aan Kanban- en Scrum-borden</a> </p> <p>We hebben de artikelkaarten op Kanban- en Scrum-borden bijgewerkt om het gemakkelijker te maken om een gebruiker aan het artikel toe te wijzen. Nu kunt u op een team of gebruikersavatar klikken om een toewijzing toe te voegen wanneer de artikelkaart wordt uitgevouwen. Eerder moest u van een afzonderlijk plusteken de plaats bepalen en klikken.</p> </td> 
   <td> <p>Voorvertoning release: 9 september 2021 <br></p> <p>Productieversie: met de release van 21.4</p> <p><strong>Beschikbaar in deze omgevingen:</strong> </p> <p>De nieuwe Adobe Workfront-ervaring </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.4-release-activity/21-4-agile-enhancements.md#configur" class="MCXref xref" xrefformat="{para}">Configureer hoe datums worden toegepast bij het toevoegen van werkitems aan een scrubherhaling</a> </p> <p>Wanneer u een werkitem aan een herhaling toevoegt, worden de geplande begindatum en de geplande voltooiingsdatum voor het werkitem standaard gewijzigd zodat deze overeenkomen met het begin en de datum van de herhaling. Nu kunt u verkiezen om de originele Geplande Datum van het Begin en Geplande Datum van de Voltooiing op alle het werkpunten voor een team te houden.</p> <p>Deze optie is alleen van toepassing op rumteams en niet op Kanban-teams.</p> </td> 
   <td><strong>Beschikbaar op deze data:</strong> <p>Voorvertoning release: 9 september 2021<br></p> <p>Productieversie: met de release van 21.4</p> <p><strong>Beschikbaar in deze omgevingen:</strong> </p> <p>De nieuwe Adobe Workfront-ervaring </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.4-release-activity/21-4-agile-enhancements.md#changes" class="MCXref xref" xrefformat="{para}">Wijzigingen in de flexibele weergave van projecten</a> </p> <p>In het kader van de release 21.3 hebben we verbeteringen aangebracht in de 'agile card'-koptekst en artikelborden (zie <a href="../../../product-announcements/product-releases/21.3-release-activity/21-3-project-enhancements.md#agile" class="MCXref xref" xrefformat="{para}">Updates van Agicard-kopteksten en artikelborden</a>). Deze updates waren van toepassing op herhalingen en op de flexibele weergave van projecten.</p> <p>Met versie 21.4 herstellen wij deze verbeteringen voor de flexibele weergave van projecten. Er worden geen wijzigingen aangebracht in variabele herhalingen.</p> <p>Hier volgen de wijzigingen die worden teruggedraaid met betrekking tot de flexibele weergave van projecten:</p> 
    <ul> 
     <li> <p>De artikelkaarten en de bordkolommen hebben aanpasbare breedten.</p> </li> 
     <li> <p>Kolommen hebben geen achtergrondarcering.</p> </li> 
     <li> <p>Kaarten hebben geen id-labels (bovenliggend artikel, subtaak, artikel, taak of uitgave).</p> </li> 
     <li> <p>De naam van de kolom Bovenliggend artikel is gewijzigd in Artikelen.</p> </li> 
    </ul> </td> 
   <td><strong>Beschikbaar op deze data:</strong> <p>Voorvertoningsrelease: 16 september 2021<br></p> <p>Productieversie: met de release van 21.4</p> <p><strong>Beschikbaar in deze omgevingen:</strong> </p> <p>De nieuwe Adobe Workfront-ervaring </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.4-release-activity/21-4-agile-enhancements.md#add" class="MCXref xref" xrefformat="{para}">Nieuwe artikelen en problemen toevoegen van het Kanban-bord</a> </p> <p>U kunt nu een nieuw artikel maken of een uitgave rechtstreeks vanaf het Kanban-bord publiceren. Zo kunt u snel een nieuw artikel toevoegen zonder dat u naar een project, rapport of dashboard hoeft te gaan om een taak te maken.</p> </td> 
   <td><strong>Beschikbaar op deze data:</strong> <p>Voorvertoningsrelease: 22 juli 2021<br></p> <p>Productieversie: met de release van 21.4</p> <p><strong>Beschikbaar in deze omgevingen:</strong> </p> <p>De nieuwe Adobe Workfront-ervaring </p> </td> 
  </tr> 
 </tbody> 
</table>

### Verbeteringen rapporteren {#reporting-enhancements}

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p><strong>Functie</strong> </p> </td> 
   <td> <p><strong>Datums en omgevingen vrijgeven</strong> </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.4-release-activity/21-4-reporting-enhancements.md#new" class="MCXref xref" xrefformat="{para}">Nieuwe look en feel voor het veld Toewijzingen in bijgewerkte lijsten en rapporten</a> </p> <p>Om de moderne blik van andere gebieden in de nieuwe ervaring van Workfront aan te passen, is het stileren voor het gebied van Taken in bijgewerkte lijsten en rapporten veranderd. Het nieuwe ontwerp omvat een nieuw de rolpictogram van de Baan een nieuw pictogram van Mensen voor geavanceerde taken, een nieuw Beperkt pictogram van de Toegang, en meer.</p> </td> 
   <td><strong>Beschikbaar op deze data:</strong> <p>Beta Preview-release: 8 april 2021 (met 21.2 release)<br></p> <p>Productieversie: 15 juli 2021<span class="uitext" style="color: #dc143c;">(Oorspronkelijk in productie vrijgegeven op de 21.2-release)</span></p> <p><strong>Beschikbaar in deze omgevingen:</strong> </p> <p>De nieuwe Adobe Workfront-ervaring </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.4-release-activity/21-4-reporting-enhancements.md#new2" class="MCXref xref" xrefformat="{para}">Nieuwe vormgeving voor typekop-kopvelden in bijgewerkte lijsten en rapporten</a> </p> <p>Om de moderne blik van andere gebieden in de nieuwe ervaring van Workfront aan te passen, is het formatteren voor typeahead gebieden in bijgewerkte lijsten en rapporten veranderd. Deze wijzigingen zijn op verschillende manieren verbeterd.</p> </td> 
   <td><strong>Beschikbaar op deze data:</strong> <p>Beta Preview-release: 8 april 2021 (met 21.2 release)<br></p> <p>Productieversie: 15 juli 2021 <span class="uitext" style="color: #dc143c;">(Oorspronkelijk in productie vrijgegeven op de 21.2-release)</span></p> <p><strong>Beschikbaar in deze omgevingen:</strong> </p> <p>De nieuwe Adobe Workfront-ervaring </p> </td> 
  </tr> 
 </tbody> 
</table>

### Verbeteringen aan verzoeken {#requests-enhancements}

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p><strong>Functie</strong> </p> </td> 
   <td> <p><strong>Datums en omgevingen vrijgeven</strong> </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.4-release-activity/21-4-requests-enhancements.md#improved" class="MCXref xref" xrefformat="{para}">Verbeterde zoekopdracht naar aanvragen bevat nu speciale tekens</a> </p> <p>Om het vinden verzoekrijen sneller en gemakkelijker te maken wanneer het voorleggen van verzoeken, hebben wij het onderzoeksalgoritme verbeterd om rijen nu te vinden die om het even welke speciale karakters zouden kunnen bevatten.</p> <p>U kunt bijvoorbeeld een aanvraagwachtrij met de naam "*Workfront" vinden door "*Workfront" of "Workfront" te typen in het veld Request Type.</p> <p>Alle speciale tekens worden ondersteund.</p> </td> 
   <td><strong>Beschikbaar op deze data:</strong> <p>Voorvertoning release: 9 september 2021<br></p> <p>Productieversie: met de release van 21.4</p> <p><strong>Beschikbaar in deze omgevingen:</strong> </p> <p>De nieuwe Adobe Workfront-ervaring </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.4-release-activity/21-4-requests-enhancements.md#new" class="MCXref xref" xrefformat="{para}">Nieuwe look and feel voor ingesloten aanvraagwachtrijen in de nieuwe Workfront-ervaring</a> </p> <p>Om de blik en het gevoel te houden voor het voorleggen van verzoeken het zelfde overal in de nieuwe ervaring van Workfront, hebben wij de interface voor het toevoegen van verzoeken aan een ingebedde verzoekrij opnieuw ontworpen. Voorafgaand aan deze verbetering, paste de interface voor het toevoegen van verzoeken van een dashboard de klassieke milieu van Workfront aan.</p> </td> 
   <td><strong>Beschikbaar op deze data:</strong> <p>Voorvertoningsrelease: 26 augustus 2021<br></p> <p>Productieversie: met de release van 21.4</p> <p><strong>Beschikbaar in deze omgevingen:</strong> </p> <p>De nieuwe Adobe Workfront-ervaring </p> </td> 
  </tr> 
 </tbody> 
</table>

### Verbeteringen voor proefdrukken {#proofing-enhancements}

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p><strong>Functie</strong> </p> </td> 
   <td> <p><strong>Datums en omgevingen vrijgeven</strong> </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.4-release-activity/21-4-proofing-enhancements.md#improved" class="MCXref xref" xrefformat="{para}">Verbeterde mogelijkheden voor proefdrukken voor revisoren en aanvragers</a> </p> <p>Voor een meer geïntegreerde ervaring tussen Workfront en Proof hebben we verschillende verbeteringen aangebracht op het gebied van mogelijkheden voor het testen van bestanden voor revisoren en aanvragers:</p> 
    <ul> 
     <li> <p>U kunt de rollen van de Moderator of van de Auteur aan om het even welke gebruiker in Workfront, ongeacht of zij een Bewijs vergunning hebben, die hen extra rechten geven, zoals het toepassen van acties of het oplossen van commentaren.</p> </li> 
     <li> <p>U kunt revisoren en aanvragers toevoegen aan proefdrukken waarvoor u zich moet aanmelden of waarvoor u een elektronische handtekening moet plaatsen.</p> </li> 
     <li> <p>Alle gebruikers profiteren ook van verbeterde connectiviteit tussen Workfront en Proof. Wanneer u nu een gebruiker deactiveert of een e-mailadres van een gebruiker bijwerkt, worden uw updates correct weergegeven in proefdrukken wanneer ze worden gewijzigd in Workfront.</p> </li> 
    </ul> </td> 
   <td><strong>Beschikbaar op deze data:</strong> <p>Voorvertoningsrelease: 5 augustus 2021 <br></p> <p>Productieversie: met de release van 21.4 <span class="uitext" style="color: #dc143c;">(Verwijderd uit Voorvertoning en Productie op 20 oktober 2021. Oorspronkelijk alleen vrijgegeven aan volledig geïntegreerde EMEA-klanten. Deze functionaliteit zal aan alle klanten in een recentere tijd opnieuw worden geïntroduceerd.)</span></p> <p><strong>Beschikbaar in deze omgevingen:</strong> </p> <p>De nieuwe Adobe Workfront-ervaring </p> <p>Adobe Workfront Classic </p> </td> 
  </tr> 
 </tbody> 
</table>

### Verbeteringen voor integratie {#integration-enhancements}

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p><strong>Functie</strong> </p> </td> 
   <td> <p><strong>Datums en omgevingen vrijgeven</strong> </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.4-release-activity/21-4-integration-enhancements.md#link" class="MCXref xref" xrefformat="{para}">Documenten van Dropbox Business koppelen</a> </p> <p>We hebben Dropbox Business toegevoegd als beschikbare documentintegratie. Nu hebt u rechtstreeks vanuit Workfront toegang tot documenten die u hebt opgeslagen in Dropbox Business.</p> <p>Met Dropbox Business kunt u gedeelde documenten koppelen en documenten uploaden naar gedeelde mappen. Met Dropbox (niet Dropbox Business) kan alleen de eigenaar van de documenten het document in Workfront bekijken.</p> <p>Uw Workfront-beheerder kan deze integratie inschakelen voor uw organisatie.</p> </td> 
   <td> <p><b>Beschikbaar op deze data:</b> </p> <p>Voorvertoning release: n.v.t.<br></p> <p>Productieversie: met de release van 21.4</p> <p><strong>Beschikbaar in deze omgevingen:</strong> </p> <p>De nieuwe Adobe Workfront-ervaring </p> <p>Adobe Workfront Classic </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.4-release-activity/21-4-integration-enhancements.md#updates" class="MCXref xref" xrefformat="{para}">Updates voor Workfront for Slack</a> </p> <p>De volgende updates zijn nu zichtbaar in de Workfront for Slack integration:</p> <p>De Workfront voor de integratie van Slacks heeft nu een nieuw gezicht. Bovendien ontvang je nu je Workfront for Slack-berichten in real-time. </p> <p>Als u bijvoorbeeld aan een taak bent toegewezen, ontvangt u dat bericht zodra u deze hebt toegewezen. </p> <p>Voorheen kon er een vertraging optreden voordat de aanmelding in de Slack verscheen.</p> </td> 
   <td><strong>Beschikbaar op deze data:</strong> <p>Voorvertoningsrelease: 29 juli 2021<br></p> <p>Productieversie: 29 juli 2021</p> <p><strong>Beschikbaar in deze omgevingen:</strong> </p> <p>De nieuwe Adobe Workfront-ervaring </p> <p>Adobe Workfront Classic </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.4-release-activity/21-4-integration-enhancements.md#more" class="MCXref xref" xrefformat="{para}">Meer duidelijkheid over de details van de toegang tot de account bij het verlenen van toestemming voor Adobe Workfront-integratie</a> </p> <p>De instemmingsschermen voor Adobe Workfront-integratie worden nu bijgewerkt. Nu kunt u de specifieke acties en gebieden zien waartoe de integratie toegang heeft, zodat u beter kunt begrijpen waartoe u de integratie of toepassing toegang verleent.</p> <p>Dit nieuwe toestemmingsscherm is op om het even welke integratie van Adobe Workfront van toepassing die OAuth 2.0 gebruikt. </p> </td> 
   <td><strong>Beschikbaar op deze data:</strong> <p>Voorvertoningsrelease: 29 juli 2021<br></p> <p>Productieversie: 29 juli 2021</p> <p><strong>Beschikbaar in deze omgevingen:</strong> </p> <p>De nieuwe Adobe Workfront-ervaring </p> <p>Adobe Workfront Classic </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.4-release-activity/21-4-integration-enhancements.md#api" class="MCXref xref" xrefformat="{para}">API-sleutelverificatie is niet meer nodig voor integratie</a> </p> <p>Workfront-integratie is onlangs begonnen met het gebruik van OAuth2 voor meer veiligheid en bruikbaarheid. Als onderdeel van deze stap vereist Workfront niet langer API-sleutels voor integratieverificatie.</p> </td> 
   <td><strong>Beschikbaar op deze data:</strong> <p>Voorvertoningsrelease: 5 augustus 2021<br></p> <p>Productieversie: 5 augustus 2021</p> <p><strong>Beschikbaar in deze omgevingen:</strong> </p> <p>De nieuwe Adobe Workfront-ervaring </p> <p>Adobe Workfront Classic </p> </td> 
  </tr> 
 </tbody> 
</table>

### Verbeteringen voor mobiele apparaten {#mobile-enhancements}

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p><strong>Functie</strong> </p> </td> 
   <td> <p><strong>Datums en omgevingen vrijgeven</strong> </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.4-release-activity/21-4-mobile-enhancements.md#review" class="MCXref xref" xrefformat="{para}">Proefbestanden in de mobiele app controleren en goedkeuren</a> </p> <p>De mobiele app van Adobe Workfront geeft nu alle proefdrukgoedkeuringen weer die aan u zijn toegewezen, in uw lijst met goedkeuringen in Mijn werk. U kunt een proefdrukdocument rechtstreeks in de app bekijken en er een beslissing over nemen.</p> </td> 
   <td><strong>Beschikbaar op deze data:</strong> <p>Voorvertoning release: n.v.t.<br></p> <p>Productieversie: Week van 11 oktober 2021</p> <p><strong>Beschikbaar in deze omgevingen:</strong> </p> 
    <ul> 
     <li> <p>iOS App Store</p> </li> 
     <li> <p>Android-app-store</p> </li> 
    </ul> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.4-release-activity/21-4-mobile-enhancements.md#create" class="MCXref xref" xrefformat="{para}">Een nieuwe aanvraag maken vanuit het begingebied van de mobiele app</a> </p> <p>U kunt nu een nieuwe aanvraag maken vanuit het thuisgebied van de mobiele Adobe Workfront-app. Als u op de knop Toevoegen op de zwevende navigatiebalk tikt, wordt naast Taak een optie voor Verzoek weergegeven. Eerder, moest u aan de pagina van Verzoeken navigeren om een verzoek tot stand te brengen.</p> </td> 
   <td><strong>Beschikbaar op deze data:</strong> <p>Voorvertoning release: n.v.t.<br></p> <p>Productieversie: 4 augustus 2021</p> <p><strong>Beschikbaar in deze omgevingen:</strong> </p> 
    <ul> 
     <li> <p>iOS App Store</p> </li> 
     <li> <p>Android-app-store</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### Andere verbeteringen {#other-enhancements}

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p><strong>Functie</strong> </p> </td> 
   <td> <p><strong>Datums en omgevingen vrijgeven</strong> </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.4-release-activity/21-4-other-enhancements.md#new" class="MCXref xref" xrefformat="{para}">Nieuwe sneltoetsen voor inspringen en uitspringen in lijsten</a> </p> <p>Om alle systeemgebruikers een toegankelijke ervaring te bieden en te voldoen aan de standaardprincipes voor toetsenbordnavigatie, zijn de opdrachten voor het inspringen/uitspringen van het toetsenbord gewijzigd. </p> <p>Voor Mac drukt u op Option + &gt; om een lijstitem te laten inspringen en op Option + &lt; om uit te springen. </p> <p>Druk in Windows op Alt + &gt; om een lijstitem te laten inspringen en op Alt + &lt; om uit te springen.</p> <p>Eerder was de sneltoets voor inspringen in een lijst Tab en was de uitspringing Shift + Tab. Als u echter de Tab-toets voor inspringen en uitspringen gebruikte, was het niet mogelijk om met de Tab-toets alle actieve velden in de interface te doorlopen.</p> <p>Deze wijziging geldt alleen voor bijgewerkte lijsten en niet voor oudere lijsten. </p> </td> 
   <td><strong>Beschikbaar op deze data:</strong> <p>Voorvertoningsrelease: 12 augustus 2021<br></p> <p>Productieversie: met de release van 21.4</p> <p><strong>Beschikbaar in deze omgevingen:</strong> </p> 
    <ul> 
     <li> <p>De nieuwe Adobe Workfront-ervaring </p> </li> 
     <li> <p>Adobe Workfront Classic </p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

## Workfront Fusion-verbeteringen

Nieuwe functies in Workfront Fusion zijn beschikbaar in Production op een cadence buiten de releaseplanning van 21.4. Voor meer informatie over de nieuwste functies raadpleegt u [Adobe Workfront Fusion-releaseactiviteit](../../../product-announcements/product-releases/fusion-release-activity/fusion-release-activity.md).

## Verbeteringen in Workfront Scenario Planner

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">There are no Scenario Planner updates at this point in the release. This area will be updated when updates are available.</p>
-->

De release van Workfront Scenario Planner met 21.4 bevat nieuwe functies. Voor informatie over deze nieuwe functies die nu beschikbaar zijn in Voorbeeld, raadpleegt u [Release-activiteit Adobe Workfront Scenario Planner](../../../product-announcements/product-releases/scenario-planner-release-activity/sp-release-activity.md).

<!--
<h2 data-mc-conditions="QuicksilverOrClassic.Draft mode">Workfront Proof enhancements</h2>
-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">New features in Workfront Proof are now available. For more information, see <a href="../../../product-announcements/product-releases/workfront-proof-release-activity/wp-release-may-17.md" class="MCXref xref" xrefformat="{para}">Workfront Proof release activity:&nbsp;Week of May 17, 2021</a>.</p>
-->

## Verbeteringen voor Workfront-doelen

Er zijn op dit moment geen updates voor Workfront Goals beschikbaar in de release. Dit gebied wordt bijgewerkt wanneer er updates beschikbaar zijn.

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">Most new features coming to Workfront Goals release with the 21.2 release. For information about these new features now available in Preview, see <a href="../../../product-announcements/product-releases/goals-release-activity/goals-21.2-release/goals-release-21-2.md" class="MCXref xref" xrefformat="{para}" data-mc-conditions="QuicksilverOrClassic.Quicksilver">Adobe Workfront Goals with the 21.2 release</a>.</p>
-->

## API-versie 14

Voor API versie 14 hebben we een aantal bronnen en eindpunten gewijzigd. Sommige wijzigingen ondersteunen nieuwe functionaliteit en andere maken het voor u gemakkelijker om de informatie te gebruiken die beschikbaar is via de API.

Voor informatie over nieuwe en bijgewerkte functies raadpleegt u [Nieuwe functies in API-versie 14](../../../wf-api/api/new-api-version-14.md).

Zie voor informatie over API-versies [API-versieschema en ondersteuningsschema](../../../wf-api/api/api-version-support-schedule.md).

## 21.4 Release-webinar

De Workfront 21.4 Release Webinar werd gepresenteerd op 23 september 2021. U kunt de webinar-opname weergeven via het dialoogvenster [Gebeurtenispagina op Workfront One](https://one.workfront.com/s/event).

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<h2>Functionality being removed from Production</h2>
<h3>Feature rollback: Carry over the existing proof workflow when generating a new version</h3>
<p>Due to customer feedback, <b>Workfront is removing this change from Preview environments on March 30, 2021 and from Production environments on March 31, 2021</b>.</p>
<p>On March 11, 2021, Workfront released a change to existing proof workflows in both Workfront Classic and the new Workfront experience. The change allowed for an existing workflow to carry over to any new proof versions created by a user, regardless of the method used to generate them.</p>
<p>In the new Workfront experience after this change is removed, proofs created with the Simple proof selection will not include any preset proofing settings, and new versions will not carry over existing workflows or proof settings. A user can adjust settings after proof generation.</p>
<p>In Workfront Classic after this change is removed, the option to Generate Proof will not include any preset proofing settings, and new versions will not carry over existing workflows or proof settings. A user can adjust settings after proof generation.</p>
<p>Similar functionality to easily copy existing workflows might be added to Production at a future time.</p>
</div>
-->

## Training-updates

Ontdek de nieuwste updates van leerprogramma&#39;s, leerpaden, video&#39;s en handleidingen voor elke Adobe Workfront-productrelease. Zie de klasse [Pagina met updates van trainingsreleases](https://one.workfront.com/s/training-release-updates).

## Functionaliteit wordt niet meer ondersteund

### Internet Explorer 11

Nu de ondersteuning voor Internet Explorer is afgeschaft, biedt Workfront nu officieel ondersteuning voor Microsoft Edge.

Zie voor meer informatie over ondersteunde browsers [Adobe Workfront-browservereisten](../../../workfront-basics/workfront-browser-requirements.md).
