---
product-area: workfront-integrations;setup
navigation-topic: workfront-for-jira
title: Het activiteitenlog van de bevalling weergeven
description: Als a [!DNL Jira]  beheerder, kunt u de uitzonderingen en de fouten bekijken die tijdens de synchronisatie of de verwezenlijking van de kaartjes tussen  [!DNL Adobe Workfront]  en  [!DNL Jira]  in een Logboek van de Activiteit voorkomen.
author: Becky
feature: Workfront Integrations and Apps
exl-id: 3e66c8e3-94b7-4153-abbb-32b872b9402b
source-git-commit: b18a7835c6de131c125b77c6688057638c62fa4a
workflow-type: tm+mt
source-wordcount: '290'
ht-degree: 0%

---

# De [!UICONTROL [!DNL Jira] Activity Log] weergeven

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
   <td role="rowheader"><a href="https://business.adobe.com/products/workfront/pricing.html" target="_blank">[!DNL Adobe Workfront] plan </a>*</td> 
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

  Voor instructies bij het installeren van [!DNL Workfront for Jira], zie [ installeren  [!DNL Adobe Workfront for Jira]](../../workfront-integrations-and-apps/use-workfront-with-jira/install-workfront-for-jira.md).

## Ga naar [!UICONTROL [!DNL Jira] Activity Log] :

1. Meld u als systeembeheerder aan bij Jira.
1. Klik op **[!UICONTROL Settings]** in het hoofdmenu [!DNL Jira] .
1. Klik op **[!UICONTROL Add-ons]** en vervolgens op **[!UICONTROL Manage add-ons]** .

1. Vouw de invoegtoepassing **[!DNL Workfront]** uit.
1. Klik op **[!UICONTROL Configure]**.
1. Meld u aan bij [!DNL Workfront] als systeembeheerder.
1. Selecteer de tab **[!UICONTROL Activity Log]** .

   Informatie weergeven over uitzonderingen en fouten die zijn opgetreden tijdens het maken van items of de synchronisatie van velden tussen de twee toepassingen.

   Het logbestand bevat de volgende velden:

   * Datum van het voorval
   * De naam van de gebruiker in Jira
   * Uitgavennummer van Jira
   * Een korte beschrijving van de fout die is opgetreden.
