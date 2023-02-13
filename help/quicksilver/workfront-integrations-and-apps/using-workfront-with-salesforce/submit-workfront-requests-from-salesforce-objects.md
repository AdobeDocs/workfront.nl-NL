---
product-area: workfront-integrations
navigation-topic: workfront-for-salesforce
title: Verzenden [!DNL Adobe Workfront] verzoeken van [!DNL Salesforce] objecten
description: Na installatie [!DNL Adobe Workfront] for [!DNL Salesforce], you can submit [!DNL Workfront] verzoeken van [!DNL Salesforce] Kansen en accounts. Deze functionaliteit is beschikbaar in zowel de raamwerken voor klassieke en bliksemervaring.
author: Becky
feature: Workfront Integrations and Apps
exl-id: 84f8cb15-4840-4fe1-bf60-93bc4283b564
source-git-commit: 5b889633a96d634a359181bfd53ec106b0f3705c
workflow-type: tm+mt
source-wordcount: '518'
ht-degree: 0%

---

# Verzenden [!DNL Adobe Workfront] verzoeken van [!DNL Salesforce] objecten

Na installatie [!DNL Adobe Workfront for Salesforce], kunt u verzenden [!DNL Workfront] verzoeken van [!DNL Salesforce] Kansen en accounts. Deze functionaliteit bestaat in beide [!DNL Classic] en [!DNL Lightning Experience] frameworks.

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

&#42;Neem contact op met uw [!DNL Workfront] beheerder.

## Vereisten

Een [!DNL Workfront] verzoek van een [!DNL Salesforce] De kans of de Rekening zorgen ervoor dat u het volgende in uw milieu hebt:

* Uw [!DNL Workfront] beheerder heeft geïnstalleerd [!DNL Workfront for Salesforce].\
   Meer informatie over installeren [!DNL Workfront for Salesforce], zie [Installeren [!DNL Adobe Workfront for Salesforce]](../../workfront-integrations-and-apps/using-workfront-with-salesforce/install-workfront-for-salesforce.md)

* Uw [!DNL Workfront] beheerder heeft de [!DNL Workfront] in uw [!UICONTROL Opportunity] en [!UICONTROL Account] paginalay-outs.\
   Voor meer informatie over het toevoegen van de [!DNL Workfront] sectie naar een pagina-indeling, zie [Configureer de [!DNL Adobe Workfront] sectie voor [!DNL Salesforce] gebruikers](../../workfront-integrations-and-apps/using-workfront-with-salesforce/configure-wf-section-for-salesforce-users.md).

* U hebt een [!DNL Workfront] en u kunt zich hier aanmelden via het dialoogvenster [!DNL Workfront] in uw Opportunity of Account.\
   Wanneer u zich aanmeldt, kunt u de [!UICONTROL New Requests] tabblad waar u aanvragen kunt invoeren.

## Verzenden [!DNL Workfront] verzoeken van [!DNL Salesforce]

1. Ga naar een opportunity of account in Salesforce.
1. Ga naar de [!DNL Workfront] sectie.
1. In de **[!UICONTROL New Requests]** selecteert u een aanvraagtype in het dialoogvenster **[!UICONTROL Select a Request Type]** vervolgkeuzemenu.

   Je kunt dezelfde aanvraagrijen zien die je in Workfront kunt zien.

1. Vul de beschikbare velden voor uw aanvraag in.

   Een verzoek indienen van [!DNL Salesforce] is identiek aan het indienen van een verzoek in het [!DNL Workfront] webtoepassing.

   >[!NOTE]
   >
   >Een document uploaden met de [!DNL Workfront] insteekmodule [!DNL Salesforce] is tijdelijk niet beschikbaar.

   Ga door met het volgen van de stappen beschreven in [Maken en verzenden [!DNL Adobe Workfront] verzoeken](../../manage-work/requests/create-requests/create-submit-requests.md).

1. Klik op **[!UICONTROL Submit]**.

## Weergave [!DNL Workfront] verzoeken

1. Naar een opportunity of account gaan in [!DNL Salesforce].
1. Ga naar de **[!DNL Workfront]** sectie.

   >[!NOTE]
   >
   >Afhankelijk van hoe uw [!DNL Workfront] beheerder vormde deze sectie, zou het een verschillende naam kunnen hebben.

1. Selecteer **[!UICONTROL Submitted Requests]** tab.

   U kunt alle verzoeken die u of anderen van deze Opportunity of Account hebben verzonden op dit tabblad bekijken. Verzoeken die naar deze aanvraagwachtrij worden verzonden in de webtoepassing, worden niet weergegeven in deze lijst in [!DNL Salesforce].

   >[!NOTE]
   >
   >Verzoeken die naar deze aanvraagwachtrij in de webtoepassing worden verzonden, worden niet weergegeven in deze lijst in Salesforce.

   ![salesforce_submitted_Requests.png](assets/salesforce-submitted-requests-350x58.png)

   U kunt de volgende informatie over de verzonden verzoeken bekijken:

   * Naam van verzoeken (in de [!UICONTROL Subject] kolom)
   * Referentienummer
   * Type aanvraag
   * Status
   * Verzonden op datum
   * Aangevraagd op naam
   * Toegewezen aan naam\

      Wanneer deze informatie wordt bijgewerkt in [!DNL Workfront], wordt het ook in deze lijst bijgewerkt.

1. (Optioneel) Klik op de naam van de aanvraag om deze te openen in [!DNL Workfront].

1. (Optioneel) Klik op **[!UICONTROL Go to [!DNL Salesforce]]** om toegang te krijgen tot de Opportunity or Account waar het probleem is ontstaan uit de volgende gebieden van Workfront:

   * In de [!UICONTROL Details] deel van de kwestie
   * Klik in het deelvenster Samenvatting als u een probleem in een lijst selecteert nadat u op [!UICONTROL Open Summary] ![](assets/summary-panel-icon.png) op de werkbalk van de lijst.
   * In de uitgiftekopbal, wanneer [!UICONTROL Integrations] is beschikbaar. Uw systeem- of groepsbeheerder moet de [!UICONTROL Integrations] in naar uw lay-outsjabloon om de koppeling Ga naar Salesforce in de uitgiftheader weer te geven. Zie voor meer informatie [Objectkoppen aanpassen met een lay-outsjabloon](../../administration-and-setup/customize-workfront/use-layout-templates/customize-object-headers.md).

   >[!NOTE]
   >
   >De [!UICONTROL Go to Salesforce] koppeling is voor iedereen zichtbaar [!DNL Workfront] gebruikers die de uitgave kunnen bekijken. U moet beschikken over een [!DNL Salesforce] om naar de [!DNL Salesforce] Opportunity of Account waar het probleem is geregistreerd.
