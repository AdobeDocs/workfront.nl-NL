---
product-area: reporting
navigation-topic: create-and-manage-reports
title: Een rapport delen in Adobe Workfront
description: Uw Adobe Workfront-beheerder verleent gebruikers toegang tot rapporten om deze weer te geven of te bewerken wanneer zij toegangsniveaus toewijzen. Zie Toegang verlenen tot rapporten, dashboards en kalenders voor meer informatie over het verlenen van toegang tot problemen.
author: Nolan
feature: Reports and Dashboards
exl-id: 225e815a-0354-493d-bbcf-59304ef77570
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '807'
ht-degree: 0%

---

# Een rapport delen in Adobe Workfront

Uw Adobe Workfront-beheerder verleent gebruikers toegang tot rapporten om deze weer te geven of te bewerken wanneer zij toegangsniveaus toewijzen. Voor meer informatie over het verlenen van toegang tot kwesties, zie [Toegang verlenen tot rapporten, dashboards en kalenders](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-reports-dashboards-calendars.md).

Samen met het toegangsniveau dat de gebruikers worden verleend, kunt u hen toestemmingen aan Mening ook verlenen of specifieke rapporten beheren die u toegang hebt om te delen. Voor meer informatie over toegangsniveaus en toestemmingen, zie [Hoe de toegangsniveaus en de toestemmingen samenwerken](../../../administration-and-setup/add-users/access-levels-and-object-permissions/how-access-levels-permissions-work-together.md).

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
   <td> <p>Toegang tot rapporten, dashboards, kalenders of hoger weergeven</p> <p>Opmerking: Als u nog steeds geen toegang hebt, vraagt u de Workfront-beheerder of deze aanvullende beperkingen op uw toegangsniveau instelt. Voor informatie over hoe een beheerder van Workfront uw toegangsniveau kan wijzigen, zie <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Aangepaste toegangsniveaus maken of wijzigen</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objectmachtigingen</td> 
   <td> <p>De toestemmingen van de mening of hoger het rapport</p> <p>Voor informatie over het aanvragen van aanvullende toegang raadpleegt u <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Toegang tot objecten aanvragen </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Neem contact op met uw Workfront-beheerder om te weten te komen welk plan, licentietype of toegang u hebt.

## Overwegingen bij het delen van rapporten

Naast de onderstaande overwegingen, zie ook [Rapporten, dashboards en kalenders delen](../../../workfront-basics/grant-and-request-access-to-objects/permissions-reports-dashboards-calendars.md).

* U kunt rapporten delen die u met andere individuen, teams, groepen, baanrollen, of bedrijven creeert. U kunt ook rapporten delen die anderen hebben gemaakt en die met u zijn gedeeld.
* U kunt ze ook delen met uw volledige organisatie of ze openbaar maken. Wanneer u een rapport openbaar maakt, wordt een URL gegenereerd die met anderen kan worden gedeeld.
* U kunt een afzonderlijk rapport delen, of u kunt meerdere rapporten delen vanuit een lijst met rapporten.

## Manieren om rapporten te delen

U kunt rapporten op de volgende manier delen in Workfront:

* Handmatig, zoals wordt beschreven in de [Een rapport delen](#share-a-report) hieronder.
* Automatisch, door de toestemmingen van de Mening van een dashboard over te nemen dat het rapport bevat dat is gedeeld. Voor informatie over het weergeven van overgeërfde machtigingen voor objecten raadpleegt u [Overerfde machtigingen voor objecten weergeven](../../../workfront-basics/grant-and-request-access-to-objects/view-inherited-permissions-on-objects.md).

## Een rapport delen {#share-a-report}

Het delen van een rapport of meerdere rapporten uit een lijst is identiek.

1. Ga naar een lijst met rapporten en selecteer een of meerdere rapporten. Klik vervolgens op **Delen**.

   of

   Klik op de naam van één rapport en klik vervolgens op **Handelingen rapporteren >****Delen**.

   ![](assets/qs-report-actions-sharing.png)

1. In het vak dat wordt weergegeven, in het dialoogvenster **Personen, teams, rollen, groepen of bedrijven toevoegen...** het gebied begint de naam van de gebruiker te typen, het team, de baanrol, de groep, of het bedrijf met wie u het rapport wilt delen, dan te drukken **Enter** wanneer de naam wordt weergegeven.

1. Als u het toegangsniveau wilt aanpassen voor een naam die u hebt toegevoegd, klikt u op het vervolgkeuzemenu rechts van de naam en kiest u een van de onderstaande opties.

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Weergeven</td> 
      <td> <p>Staat uw ontvankelijke toegang toe om het rapport in te zien <strong>Rapporten</strong> <img src="assets/reports-in-main-menu.png"> en uitvoeren.</p> <p>U kunt op <strong>Geavanceerde instellingen</strong> om te bepalen of u de gebruiker of de gebruikers wilt kunnen <strong>Delen</strong> het met iedereen in het systeem.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Beheren</td> 
      <td> <p>Staat uw ontvanger volledig toe geef toegang tot het rapport uit.</p> <p>U kunt op <strong>Geavanceerde instellingen</strong> om te bepalen of u de gebruiker of de gebruikers wilt kunnen <strong>Verwijderen</strong> het verslag van het systeem en <strong>Delen</strong> het met iedereen in het systeem.</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. (Optioneel) Herhaal de vorige twee stappen om andere namen aan de lijst toe te voegen en de opties te configureren.
1. (Optioneel) Klik op de knop **Tandwiel** pictogram ![](assets/gear-icon-settings-with-dn-arrow.jpg) in de rechterbovenhoek van het dialoogvenster voor delen selecteert u een van de volgende opties:

   * **Maak dit openbaar voor externe gebruikers:** Selecteer deze optie om een URL te genereren die met anderen kan worden gedeeld. Iedereen met de URL heeft toegang tot het rapport, zonder een Adobe Workfront-licentie.

      >[!CAUTION]
      >
      >We raden u aan voorzichtig te zijn wanneer u een object met vertrouwelijke informatie deelt met externe gebruikers. Op deze manier kunnen ze informatie weergeven zonder dat ze een Workfront-gebruiker of onderdeel van uw organisatie zijn.

      >[!NOTE]
      >
      >Als het rapport een herinnering heeft en u het openbaar deelt, moeten de gebruikers die het rapport in werking stellen aan Workfront worden geregistreerd om het rapport te kunnen in werking stellen gebruikend de herinnering. Als ze zich niet kunnen aanmelden bij Workfront, wordt het rapport weergegeven zonder dat er een melding verschijnt. Zie de sectie voor meer informatie over de beperkingen van het delen van rapporten met aanwijzingen [Beperkingen voor het delen van rapporten die worden gevraagd om rapporten](../../../reports-and-dashboards/reports/creating-and-managing-reports/add-prompt-report.md#limitations-of-running-public-prompted-reports) in het artikel [Een vraag toevoegen aan een rapport](../../../reports-and-dashboards/reports/creating-and-managing-reports/add-prompt-report.md).

   * **Dit voor het hele systeem zichtbaar maken:** Selecteer deze optie zodat iedereen in Workfront die toegang heeft tot rapporten het rapport kan zien.

1. Klikken **Opslaan**.
