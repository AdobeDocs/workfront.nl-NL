---
product-area: calendars
navigation-topic: calendars-navigation-topic
title: Een kalenderrapport delen
description: U kunt een kalender met andere gebruikers delen en u kunt het openbaar ter beschikking stellen, toestaand iemand zonder een  [!DNL Adobe Workfront]  vergunning om het te bekijken.
author: Lisa
feature: Reports and Dashboards
exl-id: 77eed0fe-2d47-40c4-a03d-590f7fa17dbe
source-git-commit: 14b78ee4dc441ca84b891b2f021d959fcf357fdd
workflow-type: tm+mt
source-wordcount: '619'
ht-degree: 0%

---

# Een kalenderrapport delen

<span class="preview"> de benadrukte informatie op deze pagina verwijst naar functionaliteit nog niet algemeen beschikbaar. Het is beschikbaar slechts in het milieu van de Sandbox van de Voorproef.</span>

U kunt een kalender delen met andere gebruikers en deze openbaar maken, zodat iemand zonder [!DNL Adobe Workfront] -licentie de kalender kan bekijken.

## Toegangsvereisten

+++ Breid uit om de toegangseisen voor de functionaliteit in dit artikel weer te geven.

U moet de volgende toegang hebben om de stappen in dit artikel uit te voeren:

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront plan]</td> 
   <td> <p>Alle</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] licentie</td> 
   <td><p>Nieuw: Licht</p>
       <p>of</p>
       <p>Huidige: revisie</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraties op toegangsniveau</td> 
   <td> <p>[!UICONTROL View] of betere toegang tot [!UICONTROL Reports] , [!UICONTROL Dashboards] , en [!UICONTROL Calendars]</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objectmachtigingen</td> 
   <td>[!UICONTROL View] of hogere machtigingen voor het kalenderrapport, met toegang tot delen</td> 
  </tr> 
 </tbody> 
</table>

Voor meer detail over de informatie in deze lijst, zie [ vereisten van de Toegang in de documentatie van Workfront ](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Een kalender delen met [!DNL Workfront] -gebruikers {#share-a-calendar-with-workfront-users}

Het delen van een kalender is vergelijkbaar met het delen van andere objecten. Voor meer informatie over het delen van voorwerpen in [!DNL Adobe Workfront], zie [ Overzicht van het delen van toestemmingen op voorwerpen ](../../../workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md).

Kalenders die met u zijn gedeeld tonen met een asterisk (&#42;) naast de kalendernaam.

Een kalender delen in [!DNL Workfront] :

1. Ga naar de kalender die u wilt delen.
1. <span class="preview"> in Voorproef, klik het **Meer** menu naast de kalendernaam, dan klik **het Delen**.
   ![ kalender meer menu ](assets/more-menu-calendar.png)</span>
1. Klik op **[!UICONTROL Calendar Actions]** en vervolgens op **[!UICONTROL Sharing]** .

1. Typ in het veld **[!UICONTROL Give Calendar access to]** de naam van de gebruiker, het team, de rol, de groep of het bedrijf die u de kalender wilt delen, en klik vervolgens op de naam wanneer deze wordt weergegeven in de vervolgkeuzelijst.\
   Om over het plaatsen van toestemmingen te leren, zie [ Overzicht van het delen van toestemmingen op voorwerpen ](../../../workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md).

1. (Optioneel) Herhaal stap 3 voor elke gebruiker, elk team, elke rol of elke groep die u toegang tot de kalender wilt verlenen.
1. Specificeer de toestemmingen voor elke gebruiker, het team, de rol, de groep, of het bedrijf die u in Stap 3 door het drop-down menu toevoegde te klikken toevoegde, dan het toestemmingsniveau dat u wilt verlenen:

   * **[!UICONTROL View]:** Gebruikers kunnen de kalender controleren en delen.

     ![ kalender van het Aandeel met de toegang van de Mening ](assets/calendar-share-view-permissions-350x249.png)

     <!--
      ![Share calendar with view access](assets/view-calendar.png)
      -->

   * **[!UICONTROL Manage]:** De gebruikers hebben volledige toegang tot de kalender, minus administratieve rechten, die op het toegangsniveau, plus alle toestemmingen van de Mening worden verleend.

     ![ kalender van het Aandeel met Manage toegang ](assets/calendar-share-manage-permissions-350x241.png)

     <!--![Share calendar with manage access](assets/manage-calendar.png)-->

     >[!NOTE]
     >
     >De [!DNL Workfront] -beheerder en de maker van de kalender kunnen machtigingen uit deze entiteiten verwijderen.

1. (Optioneel) Afhankelijk van de rol van een gebruiker kunt u mogelijk op **[!UICONTROL Advanced Options]** klikken en vervolgens op **[!UICONTROL Share]** &#x200B; klikken om de gebruiker de kalender te laten delen met andere gebruikers.

   Voor meer informatie over de toestemmingsniveaus, zie [ Overzicht van het delen van toestemmingen op voorwerpen ](../../../workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md).

1. (Optioneel) Als u de kalender beschikbaar wilt maken voor alle [!DNL Workfront] -gebruikers, klikt u op het tandwielpictogram en klikt u vervolgens in de vervolgkeuzelijst **[!UICONTROL Make this visible system-wide]** om het object beschikbaar te maken voor alle [!DNL Workfront] -gebruikers.\
   Alle gebruikers kunnen het object zien op basis van de machtigingen die u instelt.

1. Klik op **[!UICONTROL Save]**.

## Een kalender delen met een openbare koppeling

U kunt een kalender openbaar maken en een koppeling delen met personen die geen [!DNL Workfront] -licentie hebben.

1. Ga naar de kalender die u wilt delen.
1. Klik op **[!UICONTROL Calendar Actions]** en vervolgens op **[!UICONTROL Sharing]** .
1. <span class="preview"> in Voorproef, klik het **Meer** menu naast de kalendernaam.
   ![ kalender meer menu ](assets/more-menu-calendar.png)</span>

1. Klik op het tandwielpictogram en klik vervolgens op **[!UICONTROL Make this public to external users]** .
1. Klik op **[!UICONTROL Copy link]**.
1. <span class="preview"> in Voorproef, klik **Openbare verbinding van het Exemplaar**.</span>
1. Klik op **[!UICONTROL Save]**.

## Een kalender delen met een persoonlijke koppeling

U kunt een persoonlijke kalenderkoppeling delen met [!DNL Workfront] -gebruikers. Gebruikers moeten zich aanmelden om de kalender te bekijken wanneer ze de koppeling gebruiken.

1. Ga naar de kalender die u wilt delen.
1. <span class="preview"> in Voorproef, klik het **Meer** menu naast de kalendernaam, dan klik **[!UICONTROL Get Sharable Link]**.
   ![ kalender meer menu ](assets/more-menu-calendar.png)</span>
1. Klik op **[!UICONTROL Calendar Actions]** en vervolgens op **[!UICONTROL Get Sharable Link]** .
1. Klik op **[!UICONTROL Copy Link]**.

   >[!NOTE]
   >
   >[!DNL Workfront] -gebruikers moeten toegang hebben tot de kalender om deze te kunnen openen met de koppeling. Om toegang te verlenen, zie [ een kalender met  [!DNL Workfront]  gebruikers ](#share-a-calendar-with-workfront-users) delen.\
   >Als gebruikers geen toegang hebben, kunnen ze deze aanvragen nadat ze de koppeling in hun browser hebben geplakt.
