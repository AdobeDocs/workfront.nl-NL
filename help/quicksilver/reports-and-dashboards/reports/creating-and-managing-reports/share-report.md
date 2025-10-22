---
product-area: reporting
navigation-topic: create-and-manage-reports
title: Een rapport delen in Adobe Workfront
description: Uw Adobe Workfront-beheerder verleent gebruikers toegang tot rapporten om deze weer te geven of te bewerken wanneer zij toegangsniveaus toewijzen. Zie Toegang verlenen tot rapporten, dashboards en kalenders voor meer informatie over het verlenen van toegang tot problemen.
author: Nolan
feature: Reports and Dashboards
exl-id: 225e815a-0354-493d-bbcf-59304ef77570
source-git-commit: c8a25bcc8c9b56a649ca7764918c86f9cdd5b3e2
workflow-type: tm+mt
source-wordcount: '826'
ht-degree: 0%

---

# Een rapport delen in Adobe Workfront

<!-- Audited: 11/2024 -->

Uw Adobe Workfront-beheerder verleent gebruikers toegang tot rapporten om deze weer te geven of te bewerken wanneer zij toegangsniveaus toewijzen. Voor meer informatie over het verlenen van toegang tot kwesties, zie [&#x200B; Toegang verlenen tot rapporten, dashboards, en kalenders &#x200B;](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-reports-dashboards-calendars.md).

Samen met het toegangsniveau dat de gebruikers worden verleend, kunt u hen toestemmingen aan Mening ook verlenen of specifieke rapporten beheren die u toegang hebt om te delen. Voor meer informatie over toegangsniveaus en toestemmingen, zie [&#x200B; hoe de toegangsniveaus en de toestemmingen samen &#x200B;](../../../administration-and-setup/add-users/access-levels-and-object-permissions/how-access-levels-permissions-work-together.md) werken.

Machtigingen gelden specifiek voor één item in Workfront en definiëren welke handelingen u op dat item kunt uitvoeren.

>[!NOTE]
>
>Een Workfront-beheerder kan machtigingen toevoegen of verwijderen voor alle items in het systeem, zonder de eigenaar van die items te zijn.

## Toegangsvereisten

+++ Breid uit om de toegangseisen voor de functionaliteit in dit artikel weer te geven. 

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-pakket</td> 
   <td> <p>Alle</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-licentie</td> 
   <td> 
      <p>Licht</p>
      <p>Controleren</p>
   </td>
  </tr> 
  <tr> 
   <td role="rowheader">Configuraties op toegangsniveau</td> 
   <td> <p>Toegang tot rapporten, dashboards, kalenders of hoger weergeven</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objectmachtigingen</td> 
   <td> <p>Toestemmingen van de mening of hoger aan het rapport</p></td> 
  </tr> 
 </tbody> 
</table>

Voor meer detail over de informatie in deze lijst, zie [&#x200B; vereisten van de Toegang in de documentatie van Workfront &#x200B;](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Overwegingen bij het delen van rapporten

Naast de overwegingen hieronder, zie ook [&#x200B; rapporten van het Aandeel, dashboards, en kalenders &#x200B;](../../../workfront-basics/grant-and-request-access-to-objects/permissions-reports-dashboards-calendars.md).

* U kunt rapporten delen die u met andere individuen, teams, groepen, baanrollen, of bedrijven creeert. U kunt ook rapporten delen die anderen hebben gemaakt en met u zijn gedeeld.
* U kunt rapporten delen met uw volledige organisatie of hen openbaar maken. Wanneer u een rapport openbaar maakt, wordt een URL gegenereerd die met anderen kan worden gedeeld.
* U kunt een afzonderlijk rapport delen, of u kunt meerdere rapporten delen vanuit een lijst met rapporten.

## Manieren om rapporten te delen

U kunt rapporten op de volgende manier delen in Workfront:

* Handmatig, zoals die in [&#x200B; wordt beschreven deel een rapport &#x200B;](#share-a-report) hieronder sectie.
* Automatisch door de toestemmingen van de Mening van een dashboard over te nemen dat het rapport bevat dat is gedeeld. Voor informatie over het bekijken van geërfte toestemmingen op voorwerpen, zie [&#x200B; Mening geërfte toestemmingen op voorwerpen &#x200B;](../../../workfront-basics/grant-and-request-access-to-objects/view-inherited-permissions-on-objects.md).

## Een rapport delen {#share-a-report}

Het delen van een rapport of meerdere rapporten uit een lijst is identiek.

1. Ga naar een lijst van rapporten en selecteer één of veelvoudige rapporten, dan klik het **pictogram van het Aandeel** pictogram van het Aandeel ![.](assets/share-icon.png)

   of

   Klik de naam van één rapport, dan klik **Acties van het Rapport** > **het Delen**. De **2&rbrace; doos van het 1&rbrace; RAPPORTNAAM van het Aandeel &lbrace;opent.[]**

   ![&#x200B; het Delen optie &#x200B;](assets/unshimmed-report-actions-sharing.png)

1. In het **het rapporttoegang van de Verlening tot** gebied, begin de naam van de gebruiker, het team, de baanrol, de groep, of het bedrijf te typen wie u het rapport met wilt delen, dan het selecteren wanneer het toont.

1. Als u het toegangsniveau wilt aanpassen voor een naam die u hebt toegevoegd, klikt u op het vervolgkeuzemenu rechts van de naam en kiest u een van de onderstaande opties.

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Weergave</td> 
      <td> <p>Staat uw ontvankelijke toegang toe om het rapport in het <strong> gebied van Rapporten </strong> te zien en het in werking te stellen.</p> <p>U kunt het <strong> Geavanceerde pictogram van Montages </strong> op het recht klikken om te specificeren of u de gebruiker of de gebruikers <strong> </strong> het met iedereen in het systeem wilt kunnen delen.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Beheren</td> 
      <td> <p>Staat uw ontvanger volledig toe geef toegang tot het rapport uit.</p> <p>U kunt het <strong> Geavanceerde pictogram van Montages </strong> op het recht klikken om te specificeren of u de gebruiker of de gebruikers <strong> </strong> het rapport van het systeem <strong> wilt kunnen schrappen en </strong> het met iedereen in het systeem delen.</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. (Optioneel) Herhaal de vorige twee stappen om andere namen aan de lijst toe te voegen en de opties te configureren.
1. (Facultatief) klik **slechts uitgenodigde mensen kunnen tot** dropdown menu in het het delen vakje toegang hebben, dan tussen de volgende opties kiezen:

   * **slechts kunnen de uitgenodigde mensen tot** toegang hebben: Selecteer deze optie zodat slechts de gebruikers die toegang tot het rapport zijn verleend het kunnen bekijken.

   * **iedereen in het systeem kan** bekijken: Selecteer deze optie zodat iedereen in Workfront met toegang tot rapporten het rapport kan bekijken.

1. (Facultatief) klik het **pictogram van het Gear** pictogram ![&#x200B; pictogrammontages van het Gear in de hoger-juiste hoek van de het delen doos, dan naar keuze de volgende optie selecteren:](assets/gear-icon-settings-with-dn-arrow.jpg)

   * **maak dit openbaar aan externe gebruikers**: Selecteer deze optie om een URL te produceren die met anderen kan worden gedeeld. Iedereen met de URL heeft toegang tot het rapport, zonder een Adobe Workfront-licentie.

     >[!CAUTION]
     >
     >We raden u aan voorzichtig te zijn wanneer u een object met vertrouwelijke informatie deelt met externe gebruikers. Op deze manier kunnen ze informatie weergeven zonder dat ze een Workfront-gebruiker of onderdeel van uw organisatie zijn.

     >[!NOTE]
     >
     >Als het rapport een herinnering heeft en u het openbaar deelt, zullen de gebruikers die het rapport door de openbare aandeelverbinding in werking stellen het rapport niet kunnen in werking stellen gebruikend de herinnering. Zij zullen het rapport zien zonder de herinnering op het wordt toegepast tenzij zij login aan Workfront en toegang tot het rapport zonder de openbare aandeelverbinding te gebruiken. Voor meer informatie over de beperkingen om rapporten met herinneringen te delen, zie de sectie [&#x200B; Beperkingen van het delen veroorzaakt rapporten &#x200B;](../../../reports-and-dashboards/reports/creating-and-managing-reports/add-prompt-report.md#limitations-of-running-public-prompted-reports) in het artikel [&#x200B; een herinnering aan een rapport &#x200B;](../../../reports-and-dashboards/reports/creating-and-managing-reports/add-prompt-report.md) toevoegen.

1. Klik **sparen**.
