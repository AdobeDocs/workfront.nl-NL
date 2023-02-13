---
content-type: overview
product-area: workfront-integrations
navigation-topic: workfront-for-salesforce
title: Overzicht Adobe Workfront for Salesforce
description: U kunt [!DNL Adobe Workfront] voor Salesforce om uw Salesforce-gebruikers toe te staan om te verzenden [!DNL Workfront] verzoeken en maken automatisch projecten zonder ooit Salesforce te verlaten.
author: Becky
feature: Workfront Integrations and Apps
exl-id: 65d4cdae-1d34-4a8a-a1c0-706cd41fc75e
source-git-commit: 5b889633a96d634a359181bfd53ec106b0f3705c
workflow-type: tm+mt
source-wordcount: '416'
ht-degree: 0%

---

# [!DNL Adobe Workfront for Salesforce] overzicht

A [!UICONTROL Pro] [!DNL Workfront] U moet een abonnement nemen om deze functie te kunnen gebruiken. Voor meer informatie over de verschillende beschikbare plannen raadpleegt u [[!DNL Workfront] Abonnementen.](https://www.workfront.com/plans)

U kunt [!DNL Adobe Workfront for Salesforce] om uw [!DNL Salesforce] gebruikers om te verzenden [!DNL Workfront] verzoeken en automatisch projecten creëren zonder ooit te verlaten [!DNL Salesforce].

Als [!DNL Workfront] beheerder, kunt u downloaden en vormen [!DNL Workfront for Salesforce]. Vervolgens kunt u deze delen met alle andere gebruikers [!DNL Salesforce] gebruikers.

Meer informatie over installeren [!DNL Workfront for Salesforce], zie [Installeren [!DNL Adobe Workfront for Salesforce]](../../workfront-integrations-and-apps/using-workfront-with-salesforce/install-workfront-for-salesforce.md).\
Voor meer informatie over het configureren van de [!DNL Workfront] sectie in [!DNL Salesforce] voor alle gebruikers, zie [Configureer de [!DNL Adobe Workfront] sectie voor [!DNL Salesforce] gebruikers](../../workfront-integrations-and-apps/using-workfront-with-salesforce/configure-wf-section-for-salesforce-users.md).

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

&#42;Neem contact op met uw [!DNL Workfront] beheerder.

## [!DNL Workfront for Salesforce]

U kunt het volgende doen wanneer het gebruiken [!DNL Workfront for Salesforce]:

* Handmatig nieuw maken [!DNL Workfront] verzoeken van [!DNL Salesforce] binnen een Opportunity of een Account.

   Meer informatie over het maken van [!DNL Workfront] verzoeken van [!DNL Salesforce], zie [Verzenden [!DNL Adobe Workfront] verzoeken van [!DNL Salesforce] objecten](../../workfront-integrations-and-apps/using-workfront-with-salesforce/submit-workfront-requests-from-salesforce-objects.md).

* Automatisch projecten maken in [!DNL Workfront] wanneer aan bepaalde criteria is voldaan in [!DNL Salesforce]. Uw [!DNL Salesforce] systeembeheerder moet trekkers voor het creëren van projecten van vormen [!DNL Salesforce].

   Meer informatie over het maken van [!DNL Workfront] projecten van [!DNL Salesforce], zie [Maken [!DNL Adobe Workfront] projecten van [!DNL Salesforce] objecten](../../workfront-integrations-and-apps/using-workfront-with-salesforce/create-wf-projects-from-salesforce-objects.md).

Houd rekening met het volgende wanneer u werkt met [!DNL Workfront] for [!DNL Salesforce]:

* Wij steunen beide [!DNL Salesforce Classic] en [!DNL Lightning Experience] frameworks.
* Items kunnen alleen worden gemaakt van [!DNL Salesforce] in tot [!DNL Workfront].
* U kunt informatie weergeven over de [!DNL Workfront] objecten in [!DNL Salesforce].

   Deze gegevens kunnen niet worden aangepast.

   Voor een lijst met [!DNL Workfront] velden die u kunt weergeven vanuit [!DNL Salesforce], zie  [Verzenden [!DNL Adobe Workfront] verzoeken van [!DNL Salesforce] objecten](../../workfront-integrations-and-apps/using-workfront-with-salesforce/submit-workfront-requests-from-salesforce-objects.md)  en [Maken [!DNL Adobe Workfront] projecten van [!DNL Salesforce] objecten](../../workfront-integrations-and-apps/using-workfront-with-salesforce/create-wf-projects-from-salesforce-objects.md).

* U hebt rechtstreeks toegang tot items die zijn gekoppeld aan [!DNL Salesforce] door op de knop **[!UICONTROL Go to Salesforce]** verbinding uit Workfront.

   U kunt geen informatie weergeven over de [!DNL Salesforce] objecten in [!DNL Workfront], maar u hebt een koppeling naar de [!UICONTROL Salesforce] item van [!DNL Workfront] om het in [!DNL Salesforce].

   [!UICONTROL The **Ga naar Salesforce**] koppelingen worden weergegeven in de volgende gebieden:

   * De [!UICONTROL Details] deel van een project of een uitgave
   * De kopbal van een project of een kwestie.

      Uw systeem- of groepsbeheerder moet de [!UICONTROL Integrations] veld naar uw lay-outsjabloon om de [!UICONTROL Go to Salesforce] koppeling in het project of in de uitgaveheader.
   * De [!DNL Summary] paneel van een kwestie wanneer het selecteren van de kwestie in een lijst, na het klikken [!UICONTROL Open Summary] ![](assets/summary-panel-icon.png) op de werkbalk van de lijst.

      >[!NOTE]
      >
      >De [!UICONTROL Go to Salesforce] koppeling is voor iedereen zichtbaar [!DNL Workfront] gebruikers die het project of de kwestie kunnen bekijken. U moet beschikken over een [!DNL Salesforce] om naar de [!DNL Salesforce] Opportunity of Account waar het probleem is geregistreerd.

* Als u velden op één item in een toepassing bijwerkt, wordt er geen informatie over gekoppelde items in de andere toepassing bijgewerkt.
