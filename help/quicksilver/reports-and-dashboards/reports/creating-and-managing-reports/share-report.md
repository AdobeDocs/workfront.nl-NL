---
product-area: reporting
navigation-topic: create-and-manage-reports
title: Een rapport delen in Adobe Workfront
description: Uw Adobe Workfront-beheerder verleent gebruikers toegang tot rapporten om deze weer te geven of te bewerken wanneer zij toegangsniveaus toewijzen. Zie Toegang verlenen tot rapporten, dashboards en kalenders voor meer informatie over het verlenen van toegang tot problemen.
author: Nolan
feature: Reports and Dashboards
exl-id: 225e815a-0354-493d-bbcf-59304ef77570
source-git-commit: 28dd016d5edf51807c35cb392706107a08fb95f2
workflow-type: tm+mt
source-wordcount: '817'
ht-degree: 0%

---

# Een rapport delen in Adobe Workfront

Uw Adobe Workfront-beheerder verleent gebruikers toegang tot rapporten om deze weer te geven of te bewerken wanneer zij toegangsniveaus toewijzen. Voor meer informatie over het verlenen van toegang tot kwesties, zie [ Toegang verlenen tot rapporten, dashboards, en kalenders ](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-reports-dashboards-calendars.md).

Samen met het toegangsniveau dat de gebruikers worden verleend, kunt u hen toestemmingen aan Mening ook verlenen of specifieke rapporten beheren die u toegang hebt om te delen. Voor meer informatie over toegangsniveaus en toestemmingen, zie [ hoe de toegangsniveaus en de toestemmingen samen ](../../../administration-and-setup/add-users/access-levels-and-object-permissions/how-access-levels-permissions-work-together.md) werken.

Machtigingen gelden specifiek voor één item in Workfront en definiëren welke handelingen u op dat item kunt uitvoeren.

>[!NOTE]
>
>Een Workfront-beheerder kan machtigingen toevoegen of verwijderen voor alle items in het systeem, zonder de eigenaar van die items te zijn.

## Toegangsvereisten

U moet het volgende hebben om objecten te delen:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-abonnement*</td> 
   <td> <p>Alle </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-licentie*</td> 
   <td> <p>Controleren of hoger</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraties op toegangsniveau*</td> 
   <td> <p>Toegang tot rapporten, dashboards, kalenders of hoger weergeven</p> <p>Opmerking: als u nog steeds geen toegang hebt, vraag dan aan de Workfront-beheerder of deze aanvullende beperkingen op uw toegangsniveau heeft ingesteld. Voor informatie over hoe een beheerder van Workfront uw toegangsniveau kan wijzigen, zie <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref"> tot douanetoegangsniveaus </a> leiden of wijzigen.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objectmachtigingen</td> 
   <td> <p>De toestemmingen van de mening of hoger het rapport</p> <p>Voor informatie bij het vragen van om extra toegang, zie <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref"> de toegang van het Verzoek tot voorwerpen </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42; om te weten te komen welk plan, vergunningstype, of toegang u hebt, contacteer uw beheerder van Workfront.

## Overwegingen bij het delen van rapporten

Naast de overwegingen hieronder, zie ook [ rapporten van het Aandeel, dashboards, en kalenders ](../../../workfront-basics/grant-and-request-access-to-objects/permissions-reports-dashboards-calendars.md).

* U kunt rapporten delen die u met andere individuen, teams, groepen, baanrollen, of bedrijven creeert. U kunt ook rapporten delen die anderen hebben gemaakt en die met u zijn gedeeld.
* U kunt ze ook delen met uw volledige organisatie of ze openbaar maken. Wanneer u een rapport openbaar maakt, wordt een URL gegenereerd die met anderen kan worden gedeeld.
* U kunt een afzonderlijk rapport delen, of u kunt meerdere rapporten delen vanuit een lijst met rapporten.

## Manieren om rapporten te delen

U kunt rapporten op de volgende manier delen in Workfront:

* Handmatig, zoals die in [ wordt beschreven deel een rapport ](#share-a-report) hieronder sectie.
* Automatisch, door de toestemmingen van de Mening van een dashboard over te nemen dat het rapport bevat dat is gedeeld. Voor informatie over het bekijken van geërfte toestemmingen op voorwerpen, zie [ Mening geërfte toestemmingen op voorwerpen ](../../../workfront-basics/grant-and-request-access-to-objects/view-inherited-permissions-on-objects.md).

## Een rapport delen {#share-a-report}

Het delen van een rapport of meerdere rapporten uit een lijst is identiek.

1. Ga naar een lijst van rapporten en selecteer één of veelvoudige rapporten, dan klik **Aandeel**.

   of

   Klik de naam van één rapport, dan klik **de Acties van het Rapport >* **het Delen**.

   ![](assets/qs-report-actions-sharing.png)

1. In de doos die toont, in **voegt mensen, teams, rollen, groepen, of bedrijven toe..** het gebiedsbegin typend de naam van de gebruiker, het team, de baanrol, de groep, of het bedrijf u het rapport met wilt delen, dan drukt **** binnen wanneer de naamvertoningen.

1. Als u het toegangsniveau wilt aanpassen voor een naam die u hebt toegevoegd, klikt u op het vervolgkeuzemenu rechts van de naam en kiest u een van de onderstaande opties.

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Weergeven</td> 
      <td> <p>Staat uw ontvankelijke toegang toe om het rapport in het <strong> gebied van Rapporten </strong> te zien <img src="assets/reports-in-main-menu.png"> en het in werking te stellen.</p> <p>U kunt <strong> Geavanceerde Montages </strong> klikken om te specificeren of u de gebruiker of de gebruikers <strong> </strong> het met iedereen in het systeem wilt kunnen delen.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Beheren</td> 
      <td> <p>Staat uw ontvanger volledig toe geef toegang tot het rapport uit.</p> <p>U kunt <strong> Geavanceerde Montages </strong> klikken om te specificeren of u de gebruiker of de gebruikers <strong> </strong> het rapport van het systeem <strong> wilt kunnen schrappen en </strong> het met iedereen in het systeem delen.</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. (Optioneel) Herhaal de vorige twee stappen om andere namen aan de lijst toe te voegen en de opties te configureren.
1. (Optioneel) Klik op het **pictogram ![](assets/gear-icon-settings-with-dn-arrow.jpg) Gear** in de rechterbovenhoek van het vak Delen en selecteer vervolgens een van de volgende opties:

   * **maak dit openbaar aan externe gebruikers:** selecteer deze optie om een URL te produceren die met anderen kan worden gedeeld. Iedereen met de URL heeft toegang tot het rapport, zonder een Adobe Workfront-licentie.

     >[!CAUTION]
     >
     >We raden u aan voorzichtig te zijn wanneer u een object met vertrouwelijke informatie deelt met externe gebruikers. Op deze manier kunnen ze informatie weergeven zonder dat ze een Workfront-gebruiker of onderdeel van uw organisatie zijn.

     >[!NOTE]
     >
     >Als het rapport een herinnering heeft en u het openbaar deelt, zullen de gebruikers die het rapport door de openbare aandeelverbinding in werking stellen het rapport niet kunnen in werking stellen gebruikend de herinnering. Zij zullen het rapport zien zonder de herinnering op het wordt toegepast tenzij zij login aan Workfront en toegang tot het rapport zonder de openbare aandeelverbinding te gebruiken. Voor meer informatie over de beperkingen om rapporten met herinneringen te delen, zie de sectie [ Beperkingen van het delen veroorzaakt rapporten ](../../../reports-and-dashboards/reports/creating-and-managing-reports/add-prompt-report.md#limitations-of-running-public-prompted-reports) in het artikel [ een herinnering aan een rapport ](../../../reports-and-dashboards/reports/creating-and-managing-reports/add-prompt-report.md) toevoegen.

   * **maak dit zichtbaar systeem-breed:** selecteer deze optie zodat iedereen in Workfront met toegang tot rapporten het rapport kan zien.

1. Klik **sparen**.
