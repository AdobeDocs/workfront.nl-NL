---
product-area: workfront-integrations
navigation-topic: workfront-for-salesforce
title: Verzend  [!DNL Adobe Workfront]  verzoeken van  [!DNL Salesforce]  voorwerpen
description: Na het installeren van  [!DNL Adobe Workfront]  voor  [!DNL Salesforce], you can submit [!DNL Workfront]  verzoeken van  [!DNL Salesforce]  Kansen en Rekeningen. Deze functionaliteit is beschikbaar in zowel de raamwerken voor klassieke en bliksemervaring.
author: Becky
feature: Workfront Integrations and Apps
exl-id: 84f8cb15-4840-4fe1-bf60-93bc4283b564
source-git-commit: 494c7bf8aaf3570d4a01b5e88b85410ee3f52f18
workflow-type: tm+mt
source-wordcount: '519'
ht-degree: 0%

---

# [!DNL Adobe Workfront] aanvragen verzenden vanuit [!DNL Salesforce] -objecten

Nadat u [!DNL Adobe Workfront for Salesforce] hebt geïnstalleerd, kunt u [!DNL Workfront] -aanvragen van [!DNL Salesforce] Opportunity and Accounts verzenden. Deze functionaliteit bestaat zowel in de [!DNL Classic] - als in [!DNL Lightning Experience] -frameworks.

## Toegangsvereisten

U moet de volgende toegang hebben om de in dit artikel beschreven functionaliteit te kunnen gebruiken:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><p>[!DNL Adobe Workfront] plan*</p></td> 
   <td> <p>[!UICONTROL Pro] of hoger</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>[!DNL Adobe Workfront] licentie*</p></td> 
   <td> <p>[!UICONTROL Plan]</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42; om te weten te komen welk plan, vergunningstype, of toegang u hebt, contacteer uw [!DNL Workfront] beheerder.

## Vereisten

Als u een [!DNL Workfront] -aanvraag van een [!DNL Salesforce] Opportunity of Account wilt verzenden, moet u het volgende doen in uw omgeving:

* Uw [!DNL Workfront] -beheerder heeft [!DNL Workfront for Salesforce] geïnstalleerd.\
   Voor meer informatie over het installeren van [!DNL Workfront for Salesforce], zie [ installeren  [!DNL Adobe Workfront for Salesforce]](../../workfront-integrations-and-apps/using-workfront-with-salesforce/install-workfront-for-salesforce.md)

* De beheerder van [!DNL Workfront] heeft de sectie [!DNL Workfront] toegevoegd aan uw pagina-indelingen [!UICONTROL Opportunity] en [!UICONTROL Account] .\
   Voor meer informatie over het toevoegen van de [!DNL Workfront] sectie aan een paginalay-out, zie [ de  [!DNL Adobe Workfront]  sectie voor  [!DNL Salesforce]  gebruikers ](../../workfront-integrations-and-apps/using-workfront-with-salesforce/configure-wf-section-for-salesforce-users.md) vormen.

* U hebt een [!DNL Workfront] -account en u kunt zich er vanuit de [!DNL Workfront] -sectie in uw Opportunity of Account aan aanmelden.\
   Nadat u zich hebt aangemeld, kunt u het tabblad [!UICONTROL New Requests] zien waarop u aanvragen kunt invoeren.

## [!DNL Workfront] aanvragen verzenden vanuit [!DNL Salesforce]

1. Ga naar een opportunity of account in Salesforce.
1. Ga naar de sectie [!DNL Workfront] .
1. Selecteer op het tabblad **[!UICONTROL New Requests]** een aanvraagtype in de vervolgkeuzelijst **[!UICONTROL Select a Request Type]** .

   Je kunt dezelfde aanvraagrijen zien die je in Workfront kunt zien.

1. Vul de beschikbare velden voor uw aanvraag in.

   Het verzenden van een aanvraag van [!DNL Salesforce] is hetzelfde als het verzenden van een aanvraag in de [!DNL Workfront] -webtoepassing.

   >[!NOTE]
   >
   >Het uploaden van een document met de [!DNL Workfront] plug-in [!DNL Salesforce] is tijdelijk niet beschikbaar.

   Ga verder om de stappen te volgen die in [ worden beschreven creeer en voorleg  [!DNL Adobe Workfront]  verzoeken ](../../manage-work/requests/create-requests/create-submit-requests.md).

1. Klik op **[!UICONTROL Submit]**.

## [!DNL Workfront] aanvragen weergeven

1. Ga naar een opportunity of account in [!DNL Salesforce] .
1. Ga naar de sectie **[!DNL Workfront]** .

   >[!NOTE]
   >
   >Afhankelijk van de configuratie van deze sectie door de [!DNL Workfront] -beheerder, heeft deze mogelijk een andere naam.

1. Selecteer de tab **[!UICONTROL Submitted Requests]** .

   U kunt alle verzoeken die u of anderen van deze Opportunity of Account hebben verzonden op dit tabblad bekijken. Verzoeken die naar deze aanvraagwachtrij worden verzonden in de webtoepassing, worden niet weergegeven in deze lijst in [!DNL Salesforce] .

   >[!NOTE]
   >
   >Aanvragen die in de webtoepassing naar deze wachtrij met aanvragen worden verzonden, worden niet in deze lijst in Salesforce weergegeven.

   ![ salesforce_submitted_Requests.png ](assets/salesforce-submitted-requests-350x58.png)

   U kunt de volgende informatie over de verzonden verzoeken bekijken:

   * Naam aanvragen (in de kolom [!UICONTROL Subject] )
   * Referentienummer
   * Type aanvraag
   * Status
   * Verzonden op datum
   * Aangevraagd op naam
   * Toegewezen aan naam\

     Wanneer deze informatie wordt bijgewerkt in [!DNL Workfront] , wordt deze ook bijgewerkt in deze lijst.

1. (Optioneel) Klik op de naam van de aanvraag om deze te openen in [!DNL Workfront] .

1. (Optioneel) Klik op **[!UICONTROL Go to [!DNL Salesforce]]** om toegang te krijgen tot de Opportunity or Account waar het probleem is ontstaan in de volgende Workfront-regio&#39;s:

   * In de sectie [!UICONTROL Details] van het probleem
   * In het Summiere paneel wanneer het selecteren van de kwestie in een lijst, na het klikken [!UICONTROL Open Summary] ![ Summiere het paneelpictogram van de Samenvatting ](assets/summary-panel-icon.png) in de toolbar van de lijst.
   * Wanneer het veld [!UICONTROL Integrations] beschikbaar is in de uitgiftekop. Uw systeem- of groepsbeheerder moet het veld [!UICONTROL Integrations] toevoegen aan uw lay-outsjabloon om de koppeling Ga naar Salesforce in de uitgiftheader weer te geven. Voor meer informatie, zie [ objecten kopballen aanpassen gebruikend een lay-outmalplaatje ](../../administration-and-setup/customize-workfront/use-layout-templates/customize-object-headers.md).

   >[!NOTE]
   >
   >De koppeling [!UICONTROL Go to Salesforce] is zichtbaar voor alle [!DNL Workfront] -gebruikers die de uitgave kunnen bekijken. U moet een [!DNL Salesforce] -account hebben om naar de [!DNL Salesforce] Opportunity or Account te kunnen gaan waar de uitgave is geregistreerd.
