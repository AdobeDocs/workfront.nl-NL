---
title: Gebruikersvoorkeuren opnieuw instellen
user-type: administrator
product-area: system-administration;user-management
navigation-topic: create-and-manage-users
description: Als Adobe Workfront-beheerder kunt u de voorkeursinstellingen voor gebruikers in het Workfront-systeem opnieuw instellen of verwijderen. Individuele gebruikers kunnen ook hun eigen voorkeursinstellingen voor gebruikers opnieuw instellen.
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: abe026d0-3584-49f3-a6db-ef88b3aab186
source-git-commit: 5706ebd11985b9e67c93686918f8f0327adabdf1
workflow-type: tm+mt
source-wordcount: '397'
ht-degree: 1%

---

# Gebruikersvoorkeuren opnieuw instellen

<!-- Audited: 12/2023 -->

<span class="preview"> de benadrukte informatie op deze pagina verwijst naar functionaliteit nog niet algemeen beschikbaar. Het is beschikbaar slechts in het milieu van de Sandbox van de Voorproef, en wordt vrijgegeven in gefaseerde uitrol aan Productie.</span>

Als Adobe Workfront-beheerder kunt u de voorkeursinstellingen voor gebruikers in het Workfront-systeem opnieuw instellen of verwijderen.

Individuele gebruikers kunnen ook hun eigen voorkeursinstellingen voor gebruikers opnieuw instellen.

## Toegangsvereisten

+++ Breid uit om de toegangseisen voor de functionaliteit in dit artikel weer te geven.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Adobe Workfront-pakket</td> 
   <td><p>Alle</p></td> 
  </tr> 
  <tr> 
   <td>Adobe Workfront-licentie</td> 
   <td><p>Standard</p>
       <p>Plan</p></td>
  </tr> 
  <tr> 
   <td>Configuraties op toegangsniveau</td> 
   <td>Systeembeheerder</td> 
  </tr> 
 </tbody> 
</table>

Voor informatie, zie [&#x200B; vereisten van de Toegang in de documentatie van Workfront &#x200B;](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## De betreffende instellingen

Wanneer u gebruikersvoorkeuren opnieuw instelt, worden sommige voorkeuren teruggezet op de standaardsysteemstandaard en worden andere gewist of verwijderd:

<!--
<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th><strong>Preference</strong> </th> 
   <th><strong>Status after the reset</strong> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>Views</td> 
   <td> <p> Reverted to the system default</p> <p>Existing views are not deleted. You can select them again.</p> </td> 
  </tr> 
  <tr> 
   <td>Filters</td> 
   <td> <p>Reverted to the system default</p> <p>Existing filters are not deleted. You can select them again.</p> </td> 
  </tr> 
  <tr> 
   <td>Groupings</td> 
   <td> <p>Reverted to the system default</p> <p>Existing groupings are not deleted. You can select them again.</p> </td> 
  </tr> 
  <tr> 
   <td>Recent Items list</td> 
   <td>Cleared</td> 
  </tr> 
  <tr> 
   <td>Favorites list</td> 
   <td>Unaffected</td> 
  </tr> 
  <tr> 
   <td>User Preferences</td> 
   <td> <p>Reverted to the system default</p> <p>Email notifications revert to the system defaults. The default notifications are listed in <a href="/help/quicksilver/administration-and-setup/manage-workfront/emails/event-notifications-available-in-wf.md">Event notifications available in Adobe Workfront</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>User-Defined Custom Tabs</td> 
   <td>Removed</td> 
  </tr> 
  <tr> 
   <td>User-Defined Global Navigation Options</td> 
   <td>Set back to layout template definition, or system default if no layout template is assigned.</td> 
  </tr> 
 </tbody> 
</table>
-->

<!--Display this table and hide the HTML table above, when the unshim is released.-->

<div class="preview">

| Voorkeur | Status na het opnieuw instellen |
| --- | --- |
| Weergaven | Teruggedraaid naar systeemstandaard <p>Bestaande weergaven worden niet verwijderd. U kunt deze opnieuw selecteren.</p> |
| Filters | Teruggedraaid naar systeemstandaard <p>Bestaande filters worden niet verwijderd. U kunt deze opnieuw selecteren.</p> |
| Groepen | Teruggedraaid naar systeemstandaard <p>Bestaande groepen worden niet verwijderd. U kunt deze opnieuw selecteren.</p> |
| Lijst met recente objecten | Cleared |
| Lijst Favorieten | Onbeïnvloed |
| Gebruikersvoorkeuren | Teruggedraaid naar systeemstandaard <p>E-mailmeldingen worden teruggezet naar de standaardwaarden van het systeem. De standaardberichten worden vermeld in [&#x200B; berichten van de Gebeurtenis beschikbaar in Adobe Workfront &#x200B;](/help/quicksilver/administration-and-setup/manage-workfront/emails/event-notifications-available-in-wf.md).</p> |

</div>

## Gebruikersvoorkeuren opnieuw instellen

{{step-1-to-setup}}

1. Selecteer **login als**.
1. Typ de naam van de gebruiker wiens voorkeuren u wilt herstellen en klik vervolgens op de naam wanneer deze wordt weergegeven in de vervolgkeuzelijst.
1. Selecteer **Login**.
1. Als uw organisatie niet aan de Adobe Verenigde Ervaring is geregistreerd, volg deze stap:

   * Voeg in het veld URL boven aan uw webbrowser `/resetUser` toe na `workfront.com` .

     >[!NOTE]
     >
     >Dit is hoofdlettergevoelig. De U moet een hoofdletter hebben en de overige tekens moeten in kleine letters staan. Bijvoorbeeld:
     >
     >`https://company_domain.my.workfront.com/resetUser`

1. Als uw organisatie aan de Adobe Verenigde Ervaring is geregistreerd, volg deze stap:

   * Voeg in het veld URL boven aan uw webbrowser `/resetUser` toe na `workfront` .

     >[!NOTE]
     >
     >Dit is hoofdlettergevoelig. De U moet een hoofdletter hebben en de overige tekens moeten in kleine letters staan. Bijvoorbeeld:
     >
     >`https://experience.adobe.com/#/@company/so:(domain)-(environment)/workfront/resetUser`

1. Pers **gaat** binnen.

1. <span class="preview"> om alle gebruikersvoorkeur terug te stellen, klik **Terugstellen**.</span>

   <span class="preview"> Of </span>

   <span class="preview"> om de linkernavigatie van de gebruiker aan de originele configuratie van het lay-outmalplaatje terug te stellen, klik **Linkernavigatie van het Terugstellen**.</span>
