---
title: Documentintegratie uitschakelen
user-type: administrator
product-area: system-administration;workfront-integrations
navigation-topic: administrator-integrations
description: Als  [!DNL anAdobe] [!DNL Workfront] beheerder, kunt u de verbinding tussen Workfront en om het even welke derdedocumentleveranciers onbruikbaar maken.
feature: System Setup and Administration, Workfront Integrations and Apps, Digital Content and Documents
role: Admin
author: Courtney, Becky
exl-id: 78281bca-1fa1-4e78-96e5-70be12142bbd
source-git-commit: 53596271a838733b858c0b14a4e22b07a7cd20f6
workflow-type: tm+mt
source-wordcount: '263'
ht-degree: 1%

---

# Documentintegratie uitschakelen

Als [!DNL Adobe] [!DNL Workfront] -beheerder kunt u de verbinding tussen [!DNL Workfront] en alle andere documentproviders uitschakelen.

Wanneer u de verbinding tussen [!DNL Workfront] en een documentprovider uitschakelt, verdwijnen de koppelingen naar de documenten uit [!DNL Workfront] . Gebruikers kunnen de gekoppelde documenten niet meer zien, ze kunnen geen wijzigingen in de documenten aanbrengen via de [!DNL Workfront] -koppelingen en ze kunnen geen documenten meer aan die provider toevoegen.

## Toegangsvereisten

+++Breid uit om de toegangseisen voor de functionaliteit in dit artikel weer te geven.

<table>
  <tr>
   <td>Adobe Workfront-pakket
   </td>
   <td> <p>Prime of Ultimate</p>
    <p>Workflow Ultimate</p>
   </td>
  </tr>
  <tr>
   <td>Adobe Workfront-licenties
   </td>
   <td><p>Standard</p>
   <p>Plan</p>
   </td>
  </tr>
   <tr>
   <td>Configuraties op toegangsniveau
   </td>
   <td>U moet een [!DNL Workfront] beheerder zijn.
   </td>
  </tr>
</table>

Voor informatie, zie [&#x200B; vereisten van de Toegang in de documentatie van Workfront &#x200B;](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Integratie van cloudproviders uitschakelen

Als u documentintegratie wilt uitschakelen voor [!UICONTROL Workfront DAM] , [!DNL Box] , [!DNL Dropbox] , [!DNL Google Drive] , [!DNL Microsoft OneDrive] , [!DNL WebDAM] :

1. Meld u aan bij [!DNL Workfront] als [!DNL Workfront] -beheerder.

{{step-1-to-setup}}

1. Klik op **[!UICONTROL Documents]** > **[!UICONTROL Cloud Providers]** .

1. Schakel een van de cloudproviders uit waarvan u de verbinding wilt verbreken [!DNL Workfront].
1. Klik op **[!UICONTROL Save]**.

   Gebruikers kunnen geen verbinding maken met de specifieke cloud provider die u hebt uitgeschakeld en ze kunnen geen documenten van die cloud provider meer koppelen aan Workfront.

## De integratie met [!DNL SharePoint] uitschakelen

1. Meld u aan bij [!DNL Workfront] als [!DNL Workfront] -beheerder.

{{step-1-to-setup}}

1. Vouw **[!UICONTROL Documents]** uit en klik op **[!UICONTROL [!DNL SharePoint] Integration]** .
1. Selecteer de [!DNL SharePoint] -integratie die u wilt uitschakelen.
1. Klik op **[!UICONTROL Disable]**.\
   Gebruikers kunnen geen verbinding maken met de [!DNL SharePoint] -site die u hebt uitgeschakeld en ze kunnen geen documenten meer koppelen van [!DNL SharePoint] naar [!DNL Workfront] .

## Aangepaste integratie uitschakelen

1. Meld u aan bij [!DNL Workfront] als de beheerder.

{{step-1-to-setup}}

1. Klik op **[!UICONTROL Documents]** > **[!UICONTROL Custom Integration]** .
1. Selecteer de aangepaste integratie die u wilt uitschakelen.
1. Klik op **[!UICONTROL Disable]**.

   Gebruikers kunnen geen verbinding maken met de externe documentprovider die u hebt uitgeschakeld en ze kunnen geen documenten van die cloud provider meer koppelen aan [!DNL Workfront] .
