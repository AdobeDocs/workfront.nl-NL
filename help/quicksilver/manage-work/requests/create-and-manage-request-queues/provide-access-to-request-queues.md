---
product-area: requests;user-management
navigation-topic: create-and-manage-request-queues
title: Toegang tot aanvraagwachtrijen bieden
description: Wanneer u toegang tot een verzoekrij verleent, bepaalt u wie in uw organisatie de verzoekrij in het gebied van Verzoeken van Adobe Workfront kan bekijken.
author: Alina
feature: Work Management
exl-id: eb88c32a-f8b8-42d3-9a3a-72c62fd1dc3a
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '544'
ht-degree: 0%

---

# Toegang tot aanvraagwachtrijen bieden

Wanneer u toegang tot een verzoekrij verleent, bepaalt u wie in uw organisatie de verzoekrij in het gebied van Verzoeken van Adobe Workfront kan bekijken.

U kunt verschillende gebruikers toegang tot een Rij van het Verzoek verlenen, afhankelijk van of zij deel van het projectteam, de projectgroep, of het projectbedrijf uitmaken. U kunt toegang tot iedereen in het systeem aan een verzoekrij ook verlenen. 

Dit is nuttig in organisaties die externe belanghebbenden uitnodigen in Workfront en de toegang van gebruikers tot specifieke gebieden willen beperken — in dit geval beperkt een aanvraagwachtrij die alleen open staat voor de gebruikers die bij het bedrijf of de groep van het project horen, de zichtbaarheid tot externe belanghebbenden. Als u iedereen toegang geeft, wordt het verzoek zowel aan de interne als aan de externe belanghebbenden weergegeven.

## Toegangsvereisten

U moet het volgende hebben:

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
   <td> <p>Plan </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraties op toegangsniveau*</td> 
   <td> <p>Toegang tot projecten bewerken</p> <p>Opmerking: als u nog steeds geen toegang hebt, vraag dan aan de Workfront-beheerder of deze aanvullende beperkingen op uw toegangsniveau heeft ingesteld. Voor informatie over hoe een beheerder van Workfront uw toegangsniveau kan wijzigen, zie <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref"> tot douanetoegangsniveaus </a> leiden of wijzigen.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objectmachtigingen</td> 
   <td> <p> Rechten voor het project beheren</p> <p>Voor informatie bij het vragen van om extra toegang, zie <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref"> de toegang van het Verzoek tot voorwerpen </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42; om te weten te komen welk plan, vergunningstype, of toegang u hebt, contacteer uw beheerder van Workfront

## Vereisten

Voordat de aanvraagwachtrij beschikbaar is voor gebruikers in het gebied Verzoeken, moet u een project met de volgende instellingen maken:

* Wijs het aan als verzoekrij. Voor meer informatie over het creëren van een Rij van het Verzoek, zie [ een Rij van het Verzoek ](../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md) creëren.
* Werk de Status van het project aan Huidig bij.

## Toegang tot een aanvraagwachtrij bieden

1. Ga naar het project waar u toegang tot de verzoekrijen wilt verlenen.

   >[!NOTE]
   >
   >Alleen projecten met de status Huidig zijn zichtbaar in het gebied Verzoeken.

1. Klik **Details van de Rij** in het linkerpaneel. U zou kunnen moeten klikken **Meer** tonen, dan **de Details van de Rij**.
1. Selecteer **Publish als Rij van het Verzoek van de Hulp** om het project als Rij van het Verzoek aan te wijzen.
1. Selecteer een van de volgende opties:

   * **Iedereen**: Om het even welke gebruiker kan verzoeken aan de verzoekrij bekijken en toevoegen.
   * **Mensen met meningstoegang tot dit project**: De gebruikers die de toestemmingen van de Mening aan het project hebben kunnen verzoeken aan de verzoekrij bekijken en toevoegen. 
   * **Mensen in het bedrijf van dit project**: De gebruikers verbonden aan het Bedrijf van het project kunnen verzoeken bekijken en toevoegen. Het bedrijf verbonden aan het project is vermeld tussen haakjes naast deze optie. 
   * **Mensen in de groep van dit project**:De gebruikers verbonden aan de Groep van het project kunnen verzoeken bekijken en toevoegen. De groep die aan het project is gekoppeld, staat tussen haakjes naast deze optie.

     De rijen van de groep zijn nuttig wanneer verscheidene afdelingen een rekening van Workfront delen om unieke organisatorische doelstellingen te bereiken. Elke afdeling kan zijn eigen rijen hebben die de leden van andere groepen niet zouden moeten kunnen zien.

     Voor informatie over wie toestemmingen op een project heeft zie [ een project in Adobe Workfront ](../../../workfront-basics/grant-and-request-access-to-objects/share-a-project.md) delen.\
     Groepen en bedrijven kunnen met het project worden geassocieerd wanneer het uitgeven van het project. Voor meer informatie over het uitgeven van projecten, zie [ projecten ](../../../manage-work/projects/manage-projects/edit-projects.md) uitgeven.

1. Klik **sparen**.
