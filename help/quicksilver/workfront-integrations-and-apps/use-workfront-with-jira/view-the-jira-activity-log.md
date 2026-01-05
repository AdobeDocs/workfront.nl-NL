---
product-area: workfront-integrations;setup
navigation-topic: workfront-for-jira
title: Het activiteitenlog van de bevalling weergeven
description: Als a [!DNL Jira]  beheerder, kunt u de uitzonderingen en de fouten bekijken die tijdens de synchronisatie of de verwezenlijking van de kaartjes tussen  [!DNL Adobe Workfront]  en  [!DNL Jira]  in een Logboek van de Activiteit voorkomen.
author: Becky
feature: Workfront Integrations and Apps
exl-id: 3e66c8e3-94b7-4153-abbb-32b872b9402b
source-git-commit: e06713b8871ba5e7bfae58f67ee246c9c1163a63
workflow-type: tm+mt
source-wordcount: '334'
ht-degree: 1%

---

# De [!UICONTROL [!DNL Jira] Activity Log] weergeven

>[!IMPORTANT]
>
>Om stabielere en scalable integratie te leveren, verschuiven wij naar een moderne, flexibele integratiebenadering gebruikend Workfront Automation and Integration (Fusion). Als deel van dit overgangsproces, zal Workfront voor de integratie van Jira niet beschikbaar na **28 Februari, 2026** zijn.
>
>We raden u aan Workfront Automation and Integration te gebruiken voor de integratiebehoeften van uw organisatie met Jira.
>
>Voor een overzicht van de Automatisering en de Integratie van Workfront, zie [&#x200B; het overzicht van de Fusie van Adobe Workfront &#x200B;](https://experienceleague.adobe.com/nl/docs/workfront-fusion/using/get-started-with-fusion/understand-workfront-fusion/workfront-fusion-overview).
>
>Voor informatie over de specifieke mogelijkheden van de modules van de Automatisering en van de Integratie van Workfront voor Jira, zie {de modules van de Software van 0} Jira [.](https://experienceleague.adobe.com/nl/docs/workfront-fusion/using/references/apps-and-their-modules/third-party-app-connectors/jira-modules-new)

<!--

>[!IMPORTANT]
>
>To deliver more stable and scalable integrations, we're shifting to a modern, flexible integration approach using Workfront Automation and Integration (Fusion). As part of this transition process, the Workfront for Jira integration will not be available after **February 28, 2026**. 
>
>We recommend using Workfront Automation and Integration for your organization's integration needs with Jira. 
>
>Eight ready-to-use Workfront Automation and Integration templates for Jira will be available by August to help replicate common workflows and accelerate implementation. Templates are fully customizable to meet specific business needs and can be extended as requirements evolve. 
> 
>For an overview of Workfront Automation and Integration, see [Adobe Workfront Fusion overview](https://experienceleague.adobe.com/nl/docs/workfront-fusion/using/get-started-with-fusion/understand-workfront-fusion/workfront-fusion-overview). 
>
>For information about the specific capabilities of the Workfront Automation and Integration modules for Jira, see [Jira Software modules](https://experienceleague.adobe.com/nl/docs/workfront-fusion/using/references/apps-and-their-modules/third-party-app-connectors/jira-software-modules). 

-->

Als [!DNL Jira] -beheerder kunt u de uitzonderingen en fouten weergeven die optreden tijdens het synchroniseren of maken van de tickets tussen [!DNL Adobe Workfront] en [!DNL Jira] in een [!UICONTROL Activity Log] .

U kunt tot 500 punten in het Logboek van de Activiteit zien, en zij zijn vermeld beginnend met de meest recente degenen.

## Toegangsvereisten

+++ Breid uit om de toegangseisen voor de functionaliteit in dit artikel weer te geven.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-pakket</td> 
   <td><p>Alle</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-licentie</td> 
   <td><p>Standard </p>
       <p>Plan </p>
   </td>
  </tr> 
  <tr> 
   <td role="rowheader">Toegang tot Jira</td> 
   <td> <p>Toegang tot systeembeheerder</p> <p>Belangrijk: wij adviseren dat u afzonderlijke rekeningen van de systeembeheerder in Jira en Workfront creeert om aan deze integratie te wijden, eerder dan het gebruiken van bestaande die aan gebruikers zouden kunnen worden vastgemaakt.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraties op toegangsniveau</td> 
   <td> <p>U moet een Workfront-beheerder zijn.</p> </td> 
  </tr> 
 </tbody> 
</table>

Voor informatie, zie [&#x200B; vereisten van de Toegang in de documentatie van Workfront &#x200B;](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Vereisten

Voordat u items kunt koppelen tussen [!DNL Workfront] en [!DNL Jira] , moet u

* Installeren [!DNL Workfront for Jira]

  Voor instructies bij het installeren van [!DNL Workfront for Jira], zie [&#x200B; installeren  [!DNL Adobe Workfront for Jira]](../../workfront-integrations-and-apps/use-workfront-with-jira/install-workfront-for-jira.md).

## Ga naar [!UICONTROL [!DNL Jira] Activity Log] :

1. Meld u als systeembeheerder aan bij Jira.
1. Klik op **[!UICONTROL Settings]** in het hoofdmenu [!DNL Jira] .
1. Klik op **[!UICONTROL Add-ons]** en vervolgens op **[!UICONTROL Manage add-ons]** .

1. Vouw de invoegtoepassing **[!DNL Workfront]** uit.
1. Klik op **[!UICONTROL Configure]**.
1. Meld u aan bij [!DNL Workfront] als systeembeheerder.
1. Selecteer het tabblad **[!UICONTROL Activity Log]**. 

   Informatie weergeven over uitzonderingen en fouten die zijn opgetreden tijdens het maken van items of de synchronisatie van velden tussen de twee toepassingen.

   Het logbestand bevat de volgende velden:

   * Datum van het voorval
   * De naam van de gebruiker in Jira
   * Uitgavennummer van Jira
   * Een korte beschrijving van de fout die is opgetreden.
