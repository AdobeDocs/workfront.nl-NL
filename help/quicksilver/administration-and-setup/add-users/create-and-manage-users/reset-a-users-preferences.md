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
source-git-commit: 20cb940de1d42057ed11e4e7d59f1875cdba38bb
workflow-type: tm+mt
source-wordcount: '346'
ht-degree: 0%

---

# Gebruikersvoorkeuren opnieuw instellen

<!-- Audited: 12/2023 -->

Als Adobe Workfront-beheerder kunt u de voorkeursinstellingen voor gebruikers in het Workfront-systeem opnieuw instellen of verwijderen.

Individuele gebruikers kunnen ook hun eigen voorkeursinstellingen voor gebruikers opnieuw instellen.

## Toegangsvereisten

+++ Breid uit om de toegangseisen voor de functionaliteit in dit artikel weer te geven.

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
   <td><p>Nieuw: Standaard</p>
       <p>of</p>
       <p>Huidig: Plan</p></td>
  </tr> 
  <tr> 
   <td role="rowheader">Configuraties op toegangsniveau</td> 
   <td> <p>U moet een Workfront-beheerder zijn.</p> </td> 
  </tr> 
 </tbody> 
</table>

Voor meer detail over de informatie in deze lijst, zie [ vereisten van de Toegang in de documentatie van Workfront ](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

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

## Gebruikersvoorkeuren opnieuw instellen

{{step-1-to-setup}}

1. Selecteer **login als**.
1. Typ de naam van de gebruiker wiens voorkeuren u wilt herstellen en klik vervolgens op de naam wanneer deze wordt weergegeven in de vervolgkeuzelijst.
1. Selecteer **Login**.
1. Voeg in het veld URL boven aan uw webbrowser `/resetUser` toe na `workfront.com` .

   >[!NOTE]
   >
   >Dit is hoofdlettergevoelig. De U moet een hoofdletter hebben en de overige tekens moeten in kleine letters staan. Bijvoorbeeld:
   >
   >`https://company_domain.my.workfront.com/resetUser`

1. Pers **gaat** binnen.
1. Om alle gebruikersvoorkeur terug te stellen, selecteer **Terugstellen**.

   of

   Om slechts douanetabs terug te stellen, uitgezochte **Lusjes van het Terugstellen**.
