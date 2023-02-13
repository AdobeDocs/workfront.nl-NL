---
title: Gebruikersvoorkeuren opnieuw instellen
user-type: administrator
product-area: system-administration;user-management
navigation-topic: create-and-manage-users
description: Als Adobe Workfront-beheerder kunt u de voorkeursinstellingen voor gebruikers in het Workfront-systeem opnieuw instellen of verwijderen. Individuele gebruikers kunnen ook hun eigen voorkeursinstellingen voor gebruikers opnieuw instellen.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: abe026d0-3584-49f3-a6db-ef88b3aab186
source-git-commit: e20934501c2117455ca7950834d868f78576dee7
workflow-type: tm+mt
source-wordcount: '358'
ht-degree: 0%

---

# Gebruikersvoorkeuren opnieuw instellen

Als Adobe Workfront-beheerder kunt u de voorkeursinstellingen voor gebruikers in het Workfront-systeem opnieuw instellen of verwijderen.

Individuele gebruikers kunnen ook hun eigen voorkeursinstellingen voor gebruikers opnieuw instellen.

## Toegangsvereisten

U moet de volgende toegang hebben om de stappen in dit artikel uit te voeren:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-plan</td> 
   <td>Alle</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-licentie</td> 
   <td>Plan</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraties op toegangsniveau</td> 
   <td> <p>U moet een Workfront-beheerder zijn.</p> <p><b>OPMERKING</b>: Als u nog steeds geen toegang hebt, vraagt u de Workfront-beheerder of deze aanvullende beperkingen op uw toegangsniveau instelt. Voor informatie over hoe een beheerder van Workfront uw toegangsniveau kan wijzigen, zie <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Aangepaste toegangsniveaus maken of wijzigen</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## De betreffende instellingen

Wanneer u gebruikersvoorkeuren opnieuw instelt, worden sommige voorkeuren teruggezet op de standaardsysteemstandaard en worden andere gewist of verwijderd:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th><strong>Voorkeur</strong> </th> 
   <th><strong>Status na het opnieuw instellen</strong> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>Weergaven</td> 
   <td> <p> Teruggezet naar de systeemstandaard</p> <p>Bestaande weergaven worden niet verwijderd. U kunt deze opnieuw selecteren.</p> </td> 
  </tr> 
  <tr> 
   <td>Filters</td> 
   <td> <p>Teruggezet naar de systeemstandaard</p> <p>Bestaande filters worden niet verwijderd. U kunt deze opnieuw selecteren.</p> </td> 
  </tr> 
  <tr> 
   <td>Groepen</td> 
   <td> <p>Teruggezet naar de systeemstandaard</p> <p>Bestaande groepen worden niet verwijderd. U kunt deze opnieuw selecteren.</p> </td> 
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
   <td> <p>Teruggezet naar de systeemstandaard</p> <p>E-mailmeldingen worden teruggezet naar de standaardwaarden van het systeem</p> </td> 
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

## Gebruikersvoorkeuren opnieuw instellen

1. Klik op de knop **Hoofdmenu** pictogram ![](assets/main-menu-icon.png) in de rechterbovenhoek van Adobe Workfront klikt u op **Instellen** ![](assets/gear-icon-settings.png).

1. Selecteren **Aanmelden als**.
1. Typ de naam van de gebruiker wiens voorkeuren u wilt herstellen en klik vervolgens op de naam wanneer deze wordt weergegeven in de vervolgkeuzelijst.
1. Selecteren  **Aanmelden**.
1. Voeg in het veld URL boven aan uw webbrowser het volgende toe: `/resetUser` na `workfront.com`.

   >[!NOTE]
   >
   >Dit is hoofdlettergevoelig. De U moet een hoofdletter hebben en de overige tekens moeten in kleine letters staan. Bijvoorbeeld:
   >
   >
   ```
   >https://company_domain.my.workfront.com/resetUser
   >```

1. Druk **Enter**.
1. Als u alle gebruikersvoorkeuren opnieuw wilt instellen, selecteert u **Herstellen**.

   of

   Als u alleen aangepaste tabbladen wilt herstellen, selecteert u **Tabs opnieuw instellen**.
