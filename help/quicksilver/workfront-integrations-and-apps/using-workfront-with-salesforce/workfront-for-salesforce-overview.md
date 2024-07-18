---
content-type: overview
product-area: workfront-integrations
navigation-topic: workfront-for-salesforce
title: Overzicht Adobe Workfront for Salesforce
description: U kunt  [!DNL Adobe Workfront]  voor Salesforce installeren om uw gebruikers toe te staan Salesforce om  [!DNL Workfront]  verzoeken voor te leggen en automatisch projecten tot stand te brengen zonder ooit Salesforce te verlaten.
author: Becky
feature: Workfront Integrations and Apps
exl-id: 65d4cdae-1d34-4a8a-a1c0-706cd41fc75e
source-git-commit: 5b889633a96d634a359181bfd53ec106b0f3705c
workflow-type: tm+mt
source-wordcount: '414'
ht-degree: 0%

---

# [!DNL Adobe Workfront for Salesforce] overzicht

U hebt een [!UICONTROL Pro] [!DNL Workfront] -abonnement nodig om deze functie te kunnen gebruiken. Voor meer informatie over de diverse beschikbare plannen, zie [[!DNL Workfront]  Plannen.](https://www.workfront.com/plans)

U kunt [!DNL Adobe Workfront for Salesforce] installeren zodat [!DNL Salesforce] -gebruikers [!DNL Workfront] -aanvragen kunnen verzenden en automatisch projecten kunnen maken zonder [!DNL Salesforce] te verlaten.

Als [!DNL Workfront] beheerder kunt u [!DNL Workfront for Salesforce] downloaden en configureren. Vervolgens kunt u deze delen voor alle andere [!DNL Salesforce] -gebruikers.

Voor meer informatie over het installeren van [!DNL Workfront for Salesforce], zie [ installeren  [!DNL Adobe Workfront for Salesforce]](../../workfront-integrations-and-apps/using-workfront-with-salesforce/install-workfront-for-salesforce.md).\
Voor meer informatie over het vormen van de [!DNL Workfront] sectie in [!DNL Salesforce] voor alle gebruikers, zie [ de  [!DNL Adobe Workfront]  sectie voor  [!DNL Salesforce]  gebruikers ](../../workfront-integrations-and-apps/using-workfront-with-salesforce/configure-wf-section-for-salesforce-users.md) vormen.

## Toegangsvereisten

U moet de volgende toegang hebben om de in dit artikel beschreven functionaliteit te kunnen gebruiken:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] plan*</td> 
   <td> <p>[!UICONTROL Pro] of hoger</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] licentie*</td> 
   <td> <p>[!UICONTROL Plan]</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42; om te weten te komen welk plan, vergunningstype, of toegang u hebt, contacteer uw [!DNL Workfront] beheerder.

## [!DNL Workfront for Salesforce]

U kunt het volgende doen wanneer u [!DNL Workfront for Salesforce] gebruikt:

* Maak handmatig nieuwe [!DNL Workfront] aanvragen van [!DNL Salesforce] in een Opportunity of een Account.

  Voor meer informatie over het creëren van [!DNL Workfront] verzoeken van [!DNL Salesforce], zie [  [!DNL Adobe Workfront]  verzoeken van  [!DNL Salesforce]  voorwerpen ](../../workfront-integrations-and-apps/using-workfront-with-salesforce/submit-workfront-requests-from-salesforce-objects.md) voorleggen.

* Start automatisch het maken van projecten in [!DNL Workfront] wanneer aan bepaalde criteria wordt voldaan in [!DNL Salesforce] . Uw [!DNL Salesforce] -systeembeheerder moet triggers configureren voor het maken van projecten vanuit [!DNL Salesforce] .

  Voor meer informatie over het creëren van [!DNL Workfront] projecten van [!DNL Salesforce], zie [  [!DNL Adobe Workfront]  tot projecten van  [!DNL Salesforce]  voorwerpen ](../../workfront-integrations-and-apps/using-workfront-with-salesforce/create-wf-projects-from-salesforce-objects.md) leiden.

Houd rekening met het volgende wanneer u werkt met [!DNL Workfront] for [!DNL Salesforce] :

* We ondersteunen zowel de [!DNL Salesforce Classic] - als de [!DNL Lightning Experience] -frameworks.
* Items kunnen alleen van [!DNL Salesforce] in tot [!DNL Workfront] worden gemaakt.
* U kunt bepaalde informatie over de [!DNL Workfront] -items weergeven in [!DNL Salesforce] .

  Deze gegevens kunnen niet worden aangepast.

  Voor een lijst van [!DNL Workfront] gebieden die u van [!DNL Salesforce] kunt bekijken, zie [  [!DNL Adobe Workfront]  verzoeken van  [!DNL Salesforce]  voorwerpen ](../../workfront-integrations-and-apps/using-workfront-with-salesforce/submit-workfront-requests-from-salesforce-objects.md) voorleggen en [ creeer  [!DNL Adobe Workfront]  projecten van  [!DNL Salesforce]  voorwerpen ](../../workfront-integrations-and-apps/using-workfront-with-salesforce/create-wf-projects-from-salesforce-objects.md).

* U hebt rechtstreeks toegang tot items die zijn gekoppeld aan [!DNL Salesforce] door vanuit Workfront op de koppeling **[!UICONTROL Go to Salesforce]** te klikken.

  U kunt geen informatie weergeven over de [!DNL Salesforce] items in [!DNL Workfront] , maar u hebt een koppeling naar het [!UICONTROL Salesforce] -item in [!DNL Workfront] om deze te bekijken in [!DNL Salesforce] .

  [!UICONTROL The **ga naar Salesforce**] verbindingsvertoningen in de volgende gebieden:

   * De [!UICONTROL Details] -sectie van een project of uitgave
   * De kopbal van een project of een kwestie.

     Uw systeem- of groepsbeheerder moet het veld [!UICONTROL Integrations] toevoegen aan uw lay-outsjabloon om de koppeling [!UICONTROL Go to Salesforce] weer te geven in de project- of uitgiftheader.
   * Het deelvenster [!DNL Summary] van een probleem wanneer u een probleem in een lijst selecteert nadat u op [!UICONTROL Open Summary] ![](assets/summary-panel-icon.png) op de werkbalk van de lijst hebt geklikt.

     >[!NOTE]
     >
     >De koppeling [!UICONTROL Go to Salesforce] is zichtbaar voor alle [!DNL Workfront] -gebruikers die het project of het probleem kunnen bekijken. U moet een [!DNL Salesforce] -account hebben om naar de [!DNL Salesforce] Opportunity or Account te kunnen gaan waar de uitgave is geregistreerd.

* Als u velden op één item in een toepassing bijwerkt, wordt er geen informatie over gekoppelde items in de andere toepassing bijgewerkt.
