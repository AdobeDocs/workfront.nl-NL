---
content-type: tips-tricks-troubleshooting
product-area: documents
navigation-topic: tips-tricks-and-troubleshooting-proofing-within-workfront
title: Gebruikers met een proefdruklicentie weergeven in Adobe Workfront
description: U kunt op een van de volgende manieren bekijken welke gebruikers in Adobe Workfront momenteel de optie "Gebruiker kan proefdrukken genereren" hebben ingeschakeld.
author: Courtney
feature: Digital Content and Documents
exl-id: 4d45ecd9-4348-43a4-9fa7-090b996b4695
source-git-commit: 49950895440fec8cebdf12ec81191c6e890383cf
workflow-type: tm+mt
source-wordcount: '369'
ht-degree: 0%

---

# Gebruikers met een proefdruklicentie weergeven in Adobe Workfront

U kunt op een van de volgende manieren bekijken welke gebruikers in Adobe Workfront momenteel de optie &quot;Gebruiker kan proefdrukken genereren&quot; hebben ingeschakeld.

## Toegangsvereisten

U moet de volgende toegang hebben om de stappen in dit artikel uit te voeren:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-abonnement*</td> 
   <td> <p>Verouderd abonnement: Selecteren of Premium</p> <p>Voor meer informatie over het proefdrukken van toegang met de verschillende plannen, zie <a href="/help/quicksilver/administration-and-setup/manage-workfront/configure-proofing/access-to-proofing-functionality.md" class="MCXref xref"> Toegang tot het proefdrukken van functionaliteit in Workfront </a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-licentie*</td> 
   <td> <p>Plan</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objectmachtigingen</td> 
   <td> <p>Toegang bewerken tot:</p> 
    <ul> 
     <li> <p>Rapporten, dashboards en kalenders maken</p> </li> 
     <li> <p>Filters, weergaven en groepen maken</p> </li> 
    </ul> <p>Opmerking: als u nog steeds geen toegang hebt, vraag dan aan de Workfront-beheerder of deze aanvullende beperkingen op uw toegangsniveau heeft ingesteld. Voor informatie over hoe een beheerder van Workfront uw toegangsniveau kan veranderen, zie <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref"> tot douanetoegangsniveaus </a> leiden of wijzigen.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42; om te weten te komen welk plan, rol, of Profiel van de Toestemming van het Bewijs u hebt, contacteer uw beheerder van Workfront of van Workfront Proof.

## Een gebruikersrapport maken

U kunt een gebruikersrapport maken om te bekijken welke gebruikers proefdrukken kunnen genereren:

1. Navigeer aan **Meldend** gebied.
1. Klik het **Nieuwe drop-down menu van het Rapport**, dan klik **Rapport van de Gebruiker**.

1. Op het **lusje van Filters**, klik **voeg een Regel van de Filter** toe.

1. Op het beschikbare gebied, breid **Gebruiker** uit, dan klik **heeft Vergunning van Bewijs**.

1. Selecteer **Gelijk** > **Waar**.

   ![ report_prooflicenses.png ](assets/report-prooflicenses-350x135.png)

1. Klik **sparen+Sluiten**.

   In het rapport worden alle gebruikers in Workfront weergegeven waaraan een testlicentie is toegewezen.

## De weergave Personen bijwerken

U kunt een nieuwe kolom in de weergave Personen toevoegen om te bekijken welke gebruikers proefdrukken kunnen genereren:

1. Ga naar het **gebied van Mensen**.
1. Klik de **Mensen** tabel.
1. In het **drop-down menu van de Mening**, doe één van beiden van het volgende:

   * Om deze informatie aan een bestaande mening toe te voegen, selecteer de mening u wilt aanpassen, dan **klik aanpassen Mening**.
   * Om deze informatie aan een nieuwe mening toe te voegen, klik **Nieuwe Mening**.

1. Klik **toevoegen Kolom**.
1. Op het beschikbare gebied, breid **Gebruiker** uit, dan klik **heeft Vergunning van Bewijs**.

1. Klik **Gedaan**, dan klik **sparen Mening** of **sparen als Nieuwe Mening**.

   De meningsvertoningen **Waar** of **Vals** afhankelijk van of de gebruiker een het proeven vergunning heeft die aan hen wordt toegewezen.
