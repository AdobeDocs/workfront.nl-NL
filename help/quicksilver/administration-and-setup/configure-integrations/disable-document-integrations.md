---
title: Documentintegratie uitschakelen
user-type: administrator
product-area: system-administration;workfront-integrations
navigation-topic: administrator-integrations
description: Als  [!DNL anAdobe] [!DNL Workfront] beheerder, kunt u de verbinding tussen Workfront en om het even welke derdedocumentleveranciers onbruikbaar maken.
feature: System Setup and Administration, Workfront Integrations and Apps, Digital Content and Documents
role: Admin
exl-id: 78281bca-1fa1-4e78-96e5-70be12142bbd
source-git-commit: ceda437684f565b91dbb8b02f6b03cbe8d27a70a
workflow-type: tm+mt
source-wordcount: '301'
ht-degree: 0%

---

# Documentintegratie uitschakelen

Als [!DNL Adobe] [!DNL Workfront] -beheerder kunt u de verbinding tussen [!DNL Workfront] en een van de externe documentproviders uitschakelen.

Wanneer u de verbinding tussen [!DNL Workfront] en een documentprovider uitschakelt, verdwijnen de koppelingen naar de documenten uit [!DNL Workfront] . Gebruikers kunnen de gekoppelde documenten niet meer zien, ze kunnen geen wijzigingen in de documenten aanbrengen via de [!DNL Workfront] -koppelingen en ze kunnen geen documenten meer aan die provider toevoegen.

## Toegangsvereisten

U moet het volgende hebben om de stappen in dit artikel uit te voeren:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] plan</td> 
   <td>Alle</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] licentie</td> 
   <td>[!UICONTROL Plan]</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraties op toegangsniveau*</td> 
   <td> <p>U moet een [!DNL Workfront] beheerder zijn. Voor informatie over [!DNL Workfront] beheerders, zie <a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref"> een gebruiker volledige administratieve toegang verlenen </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42; Neem contact op met uw [!DNL Workfront] -beheerder als u wilt weten welk abonnement, licentietype of toegang u hebt.

## Integraties van cloudproviders uitschakelen

Als u documentintegraties wilt uitschakelen voor [!UICONTROL Workfront DAM] , [!DNL Box] , [!DNL Dropbox] , [!DNL Google Drive] , [!DNL Microsoft OneDrive] , [!DNL WebDAM] :

1. Meld u aan bij [!DNL Workfront] als [!DNL Workfront] -beheerder.
1. Klik op het **[!UICONTROL Main Menu]** pictogram ![](assets/main-menu-icon.png) rechtsboven in [!DNL Adobe Workfront] en klik vervolgens op **[!UICONTROL Setup]** ![](assets/gear-icon-settings.png) .

1. Klik op **[!UICONTROL Documents]** > **[!UICONTROL Cloud Providers]** .

1. Schakel een van de cloudproviders uit waarvan u de verbinding wilt verbreken [!DNL Workfront].
1. Klik op **[!UICONTROL Save]**.

   Gebruikers kunnen geen verbinding maken met de specifieke cloud provider die u hebt uitgeschakeld en ze kunnen geen documenten van die cloud provider meer koppelen aan Workfront.

## De integratie met [!DNL SharePoint] uitschakelen

1. Meld u aan bij [!DNL Workfront] als [!DNL Workfront] -beheerder.
1. Klik op het **[!UICONTROL Main Menu]** pictogram ![](assets/main-menu-icon.png) rechtsboven in [!DNL Adobe Workfront] en klik vervolgens op **[!UICONTROL Setup]** ![](assets/gear-icon-settings.png) .

1. Vouw **[!UICONTROL Documents]** uit en klik op **[!UICONTROL [!DNL SharePoint] Integration]** .
1. Selecteer de [!DNL SharePoint] -integratie die u wilt uitschakelen.
1. Klik op **[!UICONTROL Disable]**.\
   Gebruikers kunnen geen verbinding maken met de [!DNL SharePoint] -site die u hebt uitgeschakeld en ze kunnen geen documenten meer koppelen van [!DNL SharePoint] naar [!DNL Workfront] .

## Aangepaste integratie uitschakelen

1. Meld u aan bij [!DNL Workfront] als de beheerder.
1. Klik op het **[!UICONTROL Main Menu]** pictogram ![](assets/main-menu-icon.png) rechtsboven in [!DNL Adobe Workfront] en klik vervolgens op **[!UICONTROL Setup]** ![](assets/gear-icon-settings.png) .

1. Klik op **[!UICONTROL Documents]** > **[!UICONTROL Custom Integration]** .
1. Selecteer de aangepaste integratie die u wilt uitschakelen.
1. Klik op **[!UICONTROL Disable]**.

   Gebruikers kunnen geen verbinding maken met de externe documentprovider die u hebt uitgeschakeld en ze kunnen geen documenten van die cloudprovider meer koppelen aan [!DNL Workfront] .
