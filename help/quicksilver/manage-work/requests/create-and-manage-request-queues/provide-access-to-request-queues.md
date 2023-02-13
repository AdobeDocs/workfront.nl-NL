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
   <td> <p>Toegang tot projecten bewerken</p> <p>Opmerking: Als u nog steeds geen toegang hebt, vraagt u de Workfront-beheerder of deze aanvullende beperkingen op uw toegangsniveau instelt. Voor informatie over hoe een beheerder van Workfront uw toegangsniveau kan wijzigen, zie <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Aangepaste toegangsniveaus maken of wijzigen</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objectmachtigingen</td> 
   <td> <p> Rechten voor het project beheren</p> <p>Voor informatie over het aanvragen van aanvullende toegang raadpleegt u <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Toegang tot objecten aanvragen </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Neem contact op met uw Workfront-beheerder als u wilt weten welk plan, licentietype of toegang u hebt

## Vereisten

Voordat de aanvraagwachtrij beschikbaar is voor gebruikers in het gebied Verzoeken, moet u een project met de volgende instellingen maken:

* Wijs het aan als verzoekrij. Voor meer informatie over het creëren van een Rij van het Verzoek, zie [Een aanvraagwachtrij maken](../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md).
* Werk de Status van het project aan Huidig bij.

## Toegang tot een aanvraagwachtrij bieden

1. Ga naar het project waar u toegang tot de verzoekrijen wilt verlenen.

   >[!NOTE]
   >
   >Alleen projecten met de status Huidig zijn zichtbaar in het gebied Verzoeken.

1. Klikken **Wachtrij** in het linkerdeelvenster. Mogelijk moet u op **Meer weergeven** vervolgens **Wachtrij**.
1. Selecteren **Publiceren als wachtrij voor Help-aanvragen** om het project als Rij van het Verzoek aan te wijzen.
1. Selecteer een van de volgende opties:

   * **Iedereen**: Elke gebruiker kan aanvragen weergeven en toevoegen aan de wachtrij met aanvragen.
   * **Personen met toegang tot dit project**: De gebruikers die de toestemmingen van de Mening aan het project hebben kunnen verzoeken aan de verzoekrij bekijken en toevoegen. 
   * **Personen in het bedrijf van dit project**: De gebruikers verbonden aan het Bedrijf van het project kunnen verzoeken bekijken en toevoegen. Het bedrijf verbonden aan het project is vermeld tussen haakjes naast deze optie. 
   * **Personen in de projectgroep**:De gebruikers verbonden aan de Groep van het project kunnen verzoeken bekijken en toevoegen. De groep die aan het project is gekoppeld, staat tussen haakjes naast deze optie.

      De rijen van de groep zijn nuttig wanneer verscheidene afdelingen een rekening van Workfront delen om unieke organisatorische doelstellingen te bereiken. Elke afdeling kan zijn eigen rijen hebben die de leden van andere groepen niet zouden moeten kunnen zien.

      Voor informatie over wie toestemmingen op een project heeft zie [Een project delen in Adobe Workfront](../../../workfront-basics/grant-and-request-access-to-objects/share-a-project.md).\
      Groepen en bedrijven kunnen met het project worden geassocieerd wanneer het uitgeven van het project. Voor meer informatie over het bewerken van projecten raadpleegt u [Projecten bewerken](../../../manage-work/projects/manage-projects/edit-projects.md).

1. Klikken **Opslaan**.
