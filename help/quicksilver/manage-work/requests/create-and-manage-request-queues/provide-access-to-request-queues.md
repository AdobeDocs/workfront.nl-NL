---
product-area: requests;user-management
navigation-topic: create-and-manage-request-queues
title: Toegang tot aanvraaglijsten bieden
description: Wanneer u toegang tot een verzoekrij verleent, bepaalt u wie in uw organisatie de verzoekrij in het gebied van Verzoeken van Adobe Workfront kan bekijken.
author: Alina
feature: Work Management
exl-id: eb88c32a-f8b8-42d3-9a3a-72c62fd1dc3a
source-git-commit: abf5f21281b05dedfecbe71c6ffbf54ee69e2460
workflow-type: tm+mt
source-wordcount: '483'
ht-degree: 0%

---

# Toegang tot aanvraagwachtrijen bieden

<!-- Audited: 6/2025 -->

Wanneer u toegang tot een verzoekrij verleent, bepaalt u wie in uw organisatie de verzoekrij in het gebied van Verzoeken van Adobe Workfront kan bekijken.

U kunt verschillende gebruikers toegang tot een Rij van het Verzoek afhankelijk van verstrekken of zij deel van het projectteam, de projectgroep, of het projectbedrijf uitmaken. U kunt de toegang van de verzoekrij tot iedereen in het systeem ook verlenen.

Dit is nuttig in organisaties die externe belanghebbenden uitnodigen in Workfront en de toegang van gebruikers tot specifieke gebieden willen beperken. In dit geval, beperkt een verzoekrij open enkel aan de gebruikers verbonden aan het bedrijf of de groep van het project zicht aan externe belanghebbenden. Als u iedereen toegang geeft, wordt het verzoek zowel aan de interne als aan de externe belanghebbenden weergegeven.

## Toegangsvereisten

+++ Breid uit om de toegangseisen voor de functionaliteit in dit artikel weer te geven.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-plan</td> 
   <td> <p>Alle </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-licentie</td> 
   <td> 
   <p>Nieuw: Standaard </p>
   <p>Huidig: Plan </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraties op toegangsniveau</td> 
   <td> <p>Toegang tot projecten bewerken</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objectmachtigingen</td> 
   <td> <p> Rechten voor het project beheren</p> </td> 
  </tr> 
 </tbody> 
</table>

Voor meer detail over de informatie in deze lijst, zie [&#x200B; vereisten van de Toegang in de documentatie van Workfront &#x200B;](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Vereisten

Voordat de aanvraagwachtrij beschikbaar is voor gebruikers in het gebied Verzoeken, moet u een project met de volgende instellingen maken:

* Wijs het aan als verzoekrij. Voor meer informatie, zie [&#x200B; een Rij van het Verzoek &#x200B;](../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md) creëren.
* Werk de Status van het project aan Huidig bij.

## Toegang tot een aanvraagwachtrij bieden

1. Ga naar het project waar u toegang tot de verzoekrijen wilt verlenen.

   >[!NOTE]
   >
   >Alleen projecten met de status Huidig zijn zichtbaar in het gebied Verzoeken.

1. Klik **Details van de Rij** in het linkerpaneel.
1. Selecteer **publiceren als Rij van het Verzoek van de Hulp** om het project als Rij van het Verzoek aan te wijzen.
1. Maak een keuze uit de volgende opties:

   * **Iedereen**: Om het even welke gebruiker kan verzoeken aan de verzoekrij bekijken en toevoegen.
   * **Mensen met meningstoegang tot dit project**: De gebruikers die de toestemmingen van de Mening aan het project hebben kunnen verzoeken aan de verzoekrij bekijken en toevoegen.
   * **Mensen in het bedrijf van dit project**: De gebruikers verbonden aan het Bedrijf van het project kunnen verzoeken bekijken en toevoegen. Het bedrijf verbonden aan het project is vermeld tussen haakjes naast deze optie.
   * **Mensen in de groep van dit project**: De gebruikers verbonden aan de Groep van het project kunnen verzoeken bekijken en toevoegen. De groep die aan het project is gekoppeld, staat tussen haakjes naast deze optie.

     De rijen van de groep zijn nuttig wanneer verscheidene afdelingen een rekening van Workfront delen om unieke organisatorische doelstellingen te bereiken. Elke afdeling kan zijn eigen rijen hebben die de leden van andere groepen niet zouden moeten kunnen zien.

     Voor informatie over wie toestemmingen op een project heeft zie [&#x200B; een project in Adobe Workfront &#x200B;](../../../workfront-basics/grant-and-request-access-to-objects/share-a-project.md) delen.

     Groepen en bedrijven kunnen met het project worden geassocieerd wanneer het uitgeven van het project. Voor meer informatie, zie [&#x200B; projecten &#x200B;](../../../manage-work/projects/manage-projects/edit-projects.md) uitgeven.

1. Klik **sparen**.
