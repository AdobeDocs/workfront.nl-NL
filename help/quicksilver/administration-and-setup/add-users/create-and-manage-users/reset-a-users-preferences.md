---
title: Gebruikersvoorkeuren opnieuw instellen
user-type: administrator
product-area: system-administration;user-management
navigation-topic: create-and-manage-users
description: Als Adobe Workfront-beheerder kunt u de voorkeursinstellingen voor gebruikers in het Workfront-systeem opnieuw instellen of verwijderen. Individuele gebruikers kunnen ook hun eigen voorkeursinstellingen voor gebruikers opnieuw instellen.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: abe026d0-3584-49f3-a6db-ef88b3aab186
source-git-commit: b0b9b80b4eb718e3e131ee0cd022f54cb906f187
workflow-type: tm+mt
source-wordcount: '380'
ht-degree: 1%

---

# Gebruikersvoorkeuren opnieuw instellen

<!-- Audited: 12/2023 -->

<!--<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview Sandbox environment, and is being released in a phased rollout to Production.</span>-->

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

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th><strong> Voorkeur </strong> </th> 
   <th><strong> Status na het terugstellen </strong> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>Weergaven</td> 
   <td> <p> Teruggedraaid naar systeemstandaard</p> <p>Bestaande weergaven worden niet verwijderd. U kunt deze opnieuw selecteren.</p> </td> 
  </tr> 
  <tr> 
   <td>Filters</td> 
   <td> <p>Teruggedraaid naar systeemstandaard</p> <p>Bestaande filters worden niet verwijderd. U kunt deze opnieuw selecteren.</p> </td> 
  </tr> 
  <tr> 
   <td>Groepen</td> 
   <td> <p>Teruggedraaid naar systeemstandaard</p> <p>Bestaande groepen worden niet verwijderd. U kunt deze opnieuw selecteren.</p> </td> 
  </tr> 
  <tr> 
   <td>Lijst met recente items</td> 
   <td>Cleared</td> 
  </tr> 
  <tr> 
   <td>Lijst Favorieten</td> 
   <td>Onbeïnvloed</td> 
  </tr> 
  <tr> 
   <td>Gebruikersvoorkeuren</td> 
   <td> <p>Teruggedraaid naar systeemstandaard</p> <p>E-mailmeldingen worden teruggezet naar de standaardwaarden van het systeem. De standaardberichten worden vermeld in <a href="/help/quicksilver/administration-and-setup/manage-workfront/emails/event-notifications-available-in-wf.md"> berichten van de Gebeurtenis beschikbaar in Adobe Workfront </a>.</p> </td> 
  </tr> 
  <tr> 
   <td>Door gebruiker gedefinieerde aangepaste tabbladen</td> 
   <td>Verwijderd</td> 
  </tr> 
  <tr> 
   <td>Door gebruiker gedefinieerde globale navigatieopties</td> 
   <td>Terugzetten op definitie van lay-outsjabloon of systeemstandaard als er geen lay-outsjabloon is toegewezen.</td> 
  </tr> 
 </tbody> 
</table>

<!-- Display this table and hide the HTML table above, when the unshim is released.
| Preference | Status after the reset |
| --- | --- |
| Views | Reverted to the system default <p>Existing views are not deleted. You can select them again.</p> |
| Filters | Reverted to the system default <p>Existing filters are not deleted. You can select them again.</p> |
| Groupings | Reverted to the system default <p>Existing groupings are not deleted. You can select them again.</p> |
| Recent items list | Cleared |
| Favorites list | Unaffected |
| User Preferences | Reverted to the system default <p>Email notifications revert to the system defaults. The default notifications are listed in [Event notifications available in Adobe Workfront](/help/quicksilver/administration-and-setup/manage-workfront/emails/event-notifications-available-in-wf.md).</p> |
-->

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
1. Om alle gebruikersvoorkeur terug te stellen, selecteer **Terugstellen**.

   <!--When this is unshimmed, adjust the comment tags to hide these last two lines, because the Reset Tabs button is going away.-->
of

   Om slechts douanetabs terug te stellen, uitgezochte **Lusjes van het Terugstellen**.
