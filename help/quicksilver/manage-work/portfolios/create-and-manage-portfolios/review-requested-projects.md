---
product-area: portfolios;projects
navigation-topic: create-and-manage-portfolios
title: Gevraagde projecten controleren
description: Projectverzoeken worden weergegeven als projecten met de status [!UICONTROL Requested] in Adobe Workfront. Dit artikel beschrijft hoe te om projectverzoeken te herzien.
author: Alina
feature: Work Management, Strategic Planning
exl-id: 1acfb885-0da3-495d-ba66-e80e339e90de
source-git-commit: cf3466759a7263c446525b97dd2748ad17d0f7a6
workflow-type: tm+mt
source-wordcount: '435'
ht-degree: 0%

---

# Gevraagde projecten controleren

Wanneer meerdere projectaanvragen ter beoordeling worden ingediend, kan het projectbeheersbureau of het portefeuillecomité bijeenkomen om ingediende aanvragen te beoordelen en goedkeuringen voor projectaanvragen te bepalen. Projectverzoeken worden weergegeven als projecten met de status [!UICONTROL Requested] in [!DNL Adobe Workfront] .

U kunt een projectverzoek om overzicht voorleggen door één van het volgende te doen:

* Wijzig de projectstatus in **[!UICONTROL Requested]** .
* Voltooi [!UICONTROL Business Case] van het project en verzend het ter goedkeuring.\
   Voor meer informatie over de voltooiing van een BedrijfsGeval voor een project, zie [ een BedrijfsGeval voor een project ](../../../manage-work/projects/define-a-business-case/create-business-case.md) creëren.

U kunt opgevraagde projecten op de volgende gebieden van [!DNL Adobe Workfront] controleren:

* In een projectrapport
* Binnen een portfolio

## Toegangsvereisten

U moet de volgende toegang hebben om de stappen in dit artikel uit te voeren:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] plan*</td> 
   <td> <p>[!UICONTROL Business] of hoger</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] licentie*</td> 
   <td> <p>[!UICONTROL Plan] </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraties op toegangsniveau*</td> 
   <td> <p>[!UICONTROL View] toegang tot Portfolio's of hoger</p> <p>[!UICONTROL Edit] toegang tot projecten</p> <p>Opmerking: als u nog steeds geen toegang hebt, vraag dan aan de [!DNL Workfront] -beheerder of deze aanvullende beperkingen op uw toegangsniveau heeft ingesteld. Voor informatie over hoe een [!DNL Workfront] beheerder uw toegangsniveau kan veranderen, zie <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref"> tot douanetoegangsniveaus </a> leiden of wijzigen.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objectmachtigingen</td> 
   <td> <p>[!UICONTROL View] machtigingen of hoger voor het portfolio</p> <p>[!UICONTROL Manage] machtigingen voor de projecten om hun status bij te werken</p> <p>Voor informatie bij het vragen van om extra toegang, zie <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref"> de toegang van het Verzoek tot voorwerpen </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42; om te weten te komen welk plan, vergunningstype, of toegang u hebt, contacteer uw [!DNL Workfront] beheerder.

## Gevraagde projecten in een projectrapport evalueren

U kunt een rapport maken voor projecten om te zien welke projecten de status [!UICONTROL Requested] hebben.

Voor meer informatie over het goedkeuren van projectverzoeken door een projectrapport te bouwen, zie de [[!UICONTROL Approving the Business Case by Building a Project Report]](../../../manage-work/projects/define-a-business-case/approve-business-case.md#build-a-report) sectie in [ een BedrijfsGeval ](../../../manage-work/projects/define-a-business-case/approve-business-case.md) goedkeuren. 

## Gevraagde projecten in een portfolio bekijken

1. Ga naar het portfolio waarvan u de gewenste projecten wilt bekijken.
1. Klik &#x200B; **[!UICONTROL Projects]** in het linkerpaneel
1. Selecteer **[!UICONTROL Requested]** in de vervolgkeuzelijst **[!UICONTROL Filter]** .

   Alleen projecten met de status **[!UICONTROL Requested]** display in de lijst.

   >[!TIP]
   >
   > Naast het hebben van een Status van **[!UICONTROL Requested]**, moeten de projecten met het geselecteerde Portfolio worden geassocieerd om in deze lijst te tonen.

1. Klik op de naam van een project in de lijst om het te openen.
1. Klik op **[!UICONTROL Project Details]** in het linkerdeelvenster.
1. Voer een van de volgende handelingen uit:

   * Klik op **[!UICONTROL Business Case]** en klik vervolgens op **[!UICONTROL Approve]** of **[!UICONTROL Reject]** in het gebied [!UICONTROL Business Case Summary] om de Business Case goed te keuren of af te wijzen.

     ![ accept_or_weiger_business_case.png ](assets/approve-or-reject-business-case-350x563.png)

     De status van het project wordt gewijzigd in **[!UICONTROL Approved]** als de Business Case is goedgekeurd.

     De projectstatus wordt gewijzigd in **[!UICONTROL Rejected]** als de Business-case wordt afgewezen.

     >[!NOTE]
     >
     >Er zijn geen meldingen die de gebruiker die de goedkeuring van de bedrijfscase heeft ingediend, waarschuwen of zijn projectaanvraag is goedgekeurd of afgewezen. 

     of

   * Wijzig de status van het project in een andere status in de vervolgkeuzelijst **[!UICONTROL Status]** .

     ![](assets/project-status-change-from-drop-down-in-header-nwe-350x294.png)
 

 
