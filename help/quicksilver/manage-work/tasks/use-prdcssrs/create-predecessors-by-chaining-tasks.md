---
product-area: projects
navigation-topic: use-predecessors
title: Maak vorige relaties door taken in een keten te plaatsen
description: In Adobe Workfront kunt u op meerdere manieren voorgangersrelaties maken. Eén methode is het koppelen van taken.
author: Alina
feature: Work Management
exl-id: 38ea13a5-ab95-4617-a47f-9dde5f752fb4
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '335'
ht-degree: 0%

---

# Maak vorige relaties door taken in een keten te plaatsen

In Adobe Workfront kunt u op meerdere manieren voorgangersrelaties maken. Eén methode is het koppelen van taken.

Voor informatie over voorgangerstaken, zie [&#x200B; Overzicht van taakvoorgangers &#x200B;](../../../manage-work/tasks/use-prdcssrs/predecessors-overview.md).

Door taken in een keten op te nemen, kunt u het systeem toestaan om automatisch de voorgangersrelaties te maken voor geselecteerde taken, in plaats van handmatig zelf een relatie te maken voor elke taak. De verschillende types van voorgangersverhouding kunnen nog tussen taken worden gebruikt.

## Toegangsvereisten

U moet de volgende toegang hebben om de stappen in dit artikel uit te voeren:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-abonnement*</td> 
   <td> <p>Alle</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-licentie*</td> 
   <td> <p>Plan </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraties op toegangsniveau*</td> 
   <td> <p>Toegang tot taken en projecten bewerken</p> <p>Opmerking: als u nog steeds geen toegang hebt, vraag dan aan de Workfront-beheerder of deze aanvullende beperkingen op uw toegangsniveau heeft ingesteld. Voor informatie over hoe een beheerder van Workfront uw toegangsniveau kan wijzigen, zie <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref"> tot douanetoegangsniveaus </a> leiden of wijzigen.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objectmachtigingen</td> 
   <td> <p>Rechten voor de taken en het project beheren</p> <p>Voor informatie bij het vragen van om extra toegang, zie <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref"> de toegang van het Verzoek tot voorwerpen </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42; om te weten te komen welk plan, vergunningstype, of toegang u hebt, contacteer uw beheerder van Workfront.

## De taken van de ketting om voorgangersverhoudingen tot stand te brengen

1. Ga naar het project dat de taken bevat die u wilt ketenen.
1. Klik **Taken** in het linkerpaneel.
1. (Voorwaardelijk) Uitgezochte **Autosave** in de hoger-juiste hoek van de taaklijst, dan selecteer de taken die u wilt ketenen.

   ![](assets/nwe-autosave-icon-on-highlighted-350x295.png)

   >[!IMPORTANT]
   >
   >Het is niet mogelijk taken in een takenlijst te voorzien wanneer u handmatig wijzigingen in taken opslaat of de planningsmodus van de tijdlijn gebruikt om taken op te slaan.

1. Klik de geselecteerde taken met de rechtermuisknop aan, dan klik **Keten**.
1. Selecteer een van de volgende afhankelijkheidstypen:

   * **beëindigen-Begin**
   * **beëindigen-Afwerking**
   * **begin-Begin**
   * **begin-Afwerking**

   Voor meer informatie over de types van voorgangsafhankelijkheid, zie [&#x200B; Overzicht van de types van taakgebiedsdeel &#x200B;](../../../manage-work/tasks/use-prdcssrs/task-dependency-types.md).

1. (Facultatief) klik **Unchain** als sommige taken eerder zijn geketend.

   >[!CAUTION]
   >
   >Alleen sequentiële voordecessors worden verwijderd met de optie voor het ongedaan maken van de keten bij taken voor bulkbewerking.

   De geselecteerde taken zijn nu gekoppeld aan eerdere relaties.
