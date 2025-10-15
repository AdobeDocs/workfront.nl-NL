---
product-area: workfront-integrations;setup
navigation-topic: workfront-for-jira
title: Het activiteitenlog van de bevalling weergeven
description: Als a [!DNL Jira]  beheerder, kunt u de uitzonderingen en de fouten bekijken die tijdens de synchronisatie of de verwezenlijking van de kaartjes tussen  [!DNL Adobe Workfront]  en  [!DNL Jira]  in een Logboek van de Activiteit voorkomen.
author: Becky
feature: Workfront Integrations and Apps
exl-id: 3e66c8e3-94b7-4153-abbb-32b872b9402b
source-git-commit: 064418302767ad20e176080ba9a12db548750f3c
workflow-type: tm+mt
source-wordcount: '376'
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
>Voor informatie over de specifieke mogelijkheden van de modules van de Automatisering en van de Integratie van Workfront voor Jira, zie {de modules van de Software van 0} Jira [.](https://experienceleague.adobe.com/nl/docs/workfront-fusion/using/references/apps-and-their-modules/third-party-app-connectors/jira-software-modules)

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

U moet het volgende hebben:

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><a href="https://business.adobe.com/nl/products/workfront/pricing.html" target="_blank">[!DNL Adobe Workfront] plan </a>*</td> 
   <td> <p>[!UICONTROL Pro] of hoger</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><a href="../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref"> Adobe [!DNL Workfront] vergunningsoverzicht </a>*</td> 
   <td> <p>[!UICONTROL Plan]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Jira] toegang</td> 
   <td> <p>Toegang tot systeembeheerder</p> <p>Belangrijk: we raden u aan aparte systeembeheerdersaccounts te maken in [!DNL Jira] en [!DNL Workfront] om deze integratie te bevorderen in plaats van bestaande accounts te gebruiken die aan gebruikers kunnen worden gekoppeld.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraties op toegangsniveau*</td> 
   <td> <p>U moet een [!DNL Workfront] beheerder zijn. Voor informatie over [!DNL Workfront] beheerders, zie <a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref"> een gebruiker volledige administratieve toegang verlenen </a>.</p> <p>Opmerking: als u nog steeds geen toegang hebt, vraag dan aan de [!DNL Workfront] -beheerder of deze aanvullende beperkingen op uw toegangsniveau heeft ingesteld. Voor informatie over hoe een [!DNL Workfront] beheerder uw toegangsniveau kan wijzigen, zie <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref"> tot douanetoegangsniveaus </a> leiden of wijzigen.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42; om te weten te komen welk plan, vergunningstype, of toegang u hebt, contacteer uw [!DNL Workfront] beheerder.

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
