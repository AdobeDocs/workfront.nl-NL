---
content-type: reference
product-area: reporting;user-management
navigation-topic: custom-view-filter-and-grouping-samples
title: 'Weergeven: documentrapport met koppeling naar bewijs'
description: 'Weergeven: documentrapport met koppeling naar bewijs'
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: a38c5e86-9789-41ca-a832-2ee5eb0a570b
source-git-commit: 661f925b4e485069122ef4278b2914d206387974
workflow-type: tm+mt
source-wordcount: '356'
ht-degree: 0%

---

# Weergeven: documentrapport met koppeling naar proefdruk

In deze documentweergave kunt u een koppeling invoegen naar een proefdruk van de huidige versie van het document.

![](assets/view-document-with-proof-link-350x92.png)

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
   <td> <p>Verzoek om een weergave te wijzigen </p>
   <p>Plan om een rapport te wijzigen</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraties op toegangsniveau*</td> 
   <td> <p>Toegang tot rapporten, dashboards, kalenders bewerken om een rapport te wijzigen</p> <p>Toegang tot filters, weergaven en groepen bewerken om een weergave te wijzigen</p> <p><b>OPMERKING</b>

Als u nog steeds geen toegang hebt, vraagt u de Workfront-beheerder of deze aanvullende beperkingen op uw toegangsniveau instelt. Voor informatie over hoe een beheerder van Workfront uw toegangsniveau kan wijzigen, zie <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref"> tot douanetoegangsniveaus </a> leiden of wijzigen.</p> </td>
</tr>  
  <tr> 
   <td role="rowheader">Objectmachtigingen</td> 
   <td> <p>Machtigingen beheren voor een rapport</p> <p>Voor informatie bij het vragen van om extra toegang, zie <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref"> de toegang van het Verzoek tot voorwerpen </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42; om te weten te komen welk plan, vergunningstype, of toegang u hebt, contacteer uw beheerder van Workfront.

## Een documentrapport weergeven met koppeling naar een proefdruk

Deze weergave toepassen:

1. Ga naar een lijst met documenten.
1. Van het **drop-down menu van de Mening**, uitgezochte **Nieuwe Mening**.

1. Klik **toevoegen Kolom**.
1. Klik **Schakelaar aan de Wijze van de Tekst**.
1. Beweeg over het gebied van de tekstwijze, en klik **Klik om tekst** uit te geven.
1. Verwijder de tekst u in het **vakje van de Wijze van de Tekst** vindt, en vervang het met de volgende code:

   ```
   displayname=Proof Link
   
   shortview=true
   
   textmode=true
   
   valueexpression=CONCAT("https://Your domain.my.workfront.com/document/",{currentVersion}.{ID},"/proof/",{currentVersion}.{proofID},"/view")
   
   valueformat=HTML
   ```

   >[!TIP]
   >
   >Vervang &quot;Uw domein&quot; door uw Workfront-domein. Bijvoorbeeld, als URL van Workfront van uw bedrijf *Company.my.workfront.com* is, is uw domein &quot;Bedrijf.&quot;

1. Klik **sparen**, dan **sparen Mening**.
1. Typ een naam voor de mening, dan klik **sparen Mening**.
1. (Optioneel) Als u alleen documenten met proefdrukken wilt weergeven, voegt u een filter toe door het volgende te doen:

   1. Klik het **drop-down menu van de Filter**, dan klik **Nieuwe Filter**.
   1. Klik **toevoegen een Regel van de Filter** en beginnen Proefeigenaar te typen, dan selecteren **identiteitskaart van de Eigenaar van het Bewijs** wanneer het in de lijst toont.
   1. Selecteer **is niet leeg** voor de filterbepaling.
   1. Klik **sparen Filter**, typ de naam van de filter, dan klik **sparen Filter**.

1. Klik op de koppeling in de kolom Proefkoppeling voor toegang tot de proefdruk van de laatste versie van het document.
