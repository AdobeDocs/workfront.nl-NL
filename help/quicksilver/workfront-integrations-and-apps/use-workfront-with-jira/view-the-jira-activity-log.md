---
product-area: workfront-integrations;setup
navigation-topic: workfront-for-jira
title: Het activiteitenlog van de bevalling weergeven
description: Als [!DNL Jira] beheerder, kunt u de uitzonderingen en de fouten bekijken die tijdens de synchronisatie of de verwezenlijking van de kaartjes tussen voorkomen [!DNL Adobe Workfront] en [!DNL Jira] in een activiteitenlog.
author: Becky
feature: Workfront Integrations and Apps
exl-id: 3e66c8e3-94b7-4153-abbb-32b872b9402b
source-git-commit: 04782dfdb8c1ed24bb9c7399a01511c0cbd2dec3
workflow-type: tm+mt
source-wordcount: '291'
ht-degree: 0%

---

# De weergave van [!UICONTROL [!DNL Jira] Activity Log]

Als [!DNL Jira] beheerder, kunt u de uitzonderingen en de fouten bekijken die tijdens de synchronisatie of de verwezenlijking van de kaartjes tussen voorkomen [!DNL Adobe Workfront] en [!DNL Jira] in een [!UICONTROL Activity Log].

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
   <td role="rowheader"><a href="https://www.workfront.com/plans" target="_blank">[!DNL Adobe Workfront] plan</a>*</td> 
   <td> <p>[!UICONTROL Pro] of hoger</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><a href="../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref">Adobe [!DNL Workfront] overzicht van licenties</a>*</td> 
   <td> <p>[!UICONTROL Plan]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Jira] toegang</td> 
   <td> <p>Toegang tot systeembeheerder</p> <p>Belangrijk: Wij adviseren u afzonderlijke rekeningen van de systeembeheerder in [!DNL Jira] en [!DNL Workfront] om aan deze integratie te wijden, eerder dan het gebruiken van bestaande degenen die aan gebruikers zouden kunnen worden vastgemaakt.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraties op toegangsniveau*</td> 
   <td> <p>U moet een [!DNL Workfront] beheerder. Voor informatie over [!DNL Workfront] beheerders, zie <a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Volledige administratieve toegang verlenen aan een gebruiker</a>.</p> <p>Opmerking: Als u nog steeds geen toegang hebt, vraagt u [!DNL Workfront] beheerder als zij extra beperkingen in uw toegangsniveau plaatsen. Voor informatie over hoe een [!DNL Workfront] de beheerder kan uw toegangsniveau wijzigen, zie <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Aangepaste toegangsniveaus maken of wijzigen</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Neem contact op met uw [!DNL Workfront] beheerder.

## Vereisten

Voordat u items kunt koppelen tussen [!DNL Workfront] en [!DNL Jira]moet u

* Installeren [!DNL Workfront for Jira]

   Voor installatie-instructies [!DNL Workfront for Jira], zie [Installeren [!DNL Adobe Workfront for Jira]](../../workfront-integrations-and-apps/use-workfront-with-jira/install-workfront-for-jira.md).

## Toegang krijgen tot [!UICONTROL [!DNL Jira] Activity Log]:

1. Meld u als systeembeheerder aan bij Jira.
1. Klikken **[!UICONTROL Settings]** in het algemeen [!DNL Jira] -menu.
1. Klikken **[!UICONTROL Add-ons]** vervolgens **[!UICONTROL Manage add-ons]**.

1. Breid uit **[!DNL Workfront]** invoegtoepassing.
1. Klik op **[!UICONTROL Configure]**.
1. Aanmelden bij [!DNL Workfront] als systeembeheerder.
1. Selecteer **[!UICONTROL Activity Log]** tab.

   Informatie weergeven over uitzonderingen en fouten die zijn opgetreden tijdens het maken van items of de synchronisatie van velden tussen de twee toepassingen.

   Het logbestand bevat de volgende velden:

   * Datum van het voorval
   * De naam van de gebruiker in Jira
   * Uitgavennummer van Jira
   * Een korte beschrijving van de fout die is opgetreden.
