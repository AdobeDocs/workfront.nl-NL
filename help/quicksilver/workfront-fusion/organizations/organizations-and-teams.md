---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations;user-management
navigation-topic: organizations
title: Adobe Workfront Fusion-organisaties en -teams
description: Met de functies van Adobe Workfront Fusion Organisation en Teams kunnen ondernemingen de toegang tot scenario's en andere functies in Fusion controleren.
author: Becky
feature: Workfront Fusion
exl-id: 601e937f-0286-4557-9a87-59aa9c0c22f1
source-git-commit: e58ff769015b8c4e34b34eea653f55a296eea371
workflow-type: tm+mt
source-wordcount: '867'
ht-degree: 0%

---

# [!DNL Adobe Workfront Fusion] organisaties en teams

[!DNL Adobe Workfront Fusion]Met de functies Organisatie en Teams kunnen ondernemingen de toegang tot scenario&#39;s en andere kenmerken binnen Fusion controleren.

## Toegangsvereisten

U moet de volgende toegang hebben om de functionaliteit in dit artikel te kunnen gebruiken:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
    <td role="rowheader">[!DNL Adobe Workfront] plan*</td> 
   <td> <p>[!DNL Pro] of hoger</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Adobe Workfront Fusion] licentie**</td> 
   <td> <p>Workfront Fusion for Work Automation and Integration,</p>  </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Product</td> 
   <td>Uw organisatie moet [!DNL Adobe Workfront Fusion] alsmede [!DNL Adobe Workfront] om de in dit artikel beschreven functionaliteit te gebruiken.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">Configuraties op toegangsniveau*</td> 
   <td> 
     <p>U moet een [!DNL Workfront Fusion] beheerder van uw organisatie.</p>
     <p>U moet een [!DNL Workfront Fusion] beheerder voor uw team.</p>
   </td> 
  </tr> 
 </tbody> 
</table>

Neem contact op met uw [!DNL Workfront] beheerder.

<p>**Voor informatie over [!DNL Adobe Workfront Fusion] licenties, zie <a href="../../workfront-fusion/get-started/license-automation-vs-integration.md" class="MCXref xref">[!DNL Adobe Workfront Fusion] licenties</a></p>


## Organisaties

[!DNL Workfront Fusion] gebruikers behoren tot een organisatie. Uw [!DNL Fusion] De vergunning bepaalt hoeveel actieve scenario&#39;s en schakelaars in uw organisatie beschikbaar zijn.

[!DNL Fusion] het verlenen van vergunningen bepaalt het aantal actieve scenario&#39;s en actieve apps die aan een organisatie beschikbaar zijn. [!DNL Fusion] geeft het huidige aantal actieve scenario&#39;s en actieve apps weer op het dashboard van de organisatie.

* [Organisatiefuncties](#organization-roles)
* [Gebruikers uitnodigen voor een organisatie](#inviting-users-to-an-organization)

### Organisatiefuncties

Een gebruiker heeft een van de volgende rollen in een organisatie:

* **[!UICONTROL Owner]**: De eigenaar heeft alle rechten die beschikbaar zijn in de organisatie.
* **[!UICONTROL Admin]**: Met de beheerdersrol kan een gebruiker teams en gebruikers voor de organisatie maken en beheren.
* **[!UICONTROL Member]**: Leden kunnen [!DNL Workfront Fusion] maar kan geen organisatorische wijzigingen aanbrengen.
* **[!UICONTROL Accountant]**: Met een accountantrol kunnen gebruikers alleen licentiegegevens weergeven op het dashboard van de organisatie.
* **[!UICONTROL App Developer]**: De functionaliteit voor deze rol is momenteel niet beschikbaar en zal in de nabije toekomst beschikbaar worden gesteld. We raden u momenteel niet aan gebruikers aan deze rol toe te wijzen.

### Gebruikers uitnodigen voor een organisatie

Door gebrek, kan een organisatieeigenaar (of erkende gebruiker) een andere persoon uitnodigen om zich bij hun organisatie aan te sluiten.

Een gebruiker uitnodigen om deel te nemen aan een organisatie:

1. Klikken **[!UICONTROL Change details]** in de rechterbovenhoek van het scherm.
1. Selecteren **[!UICONTROL Invite a new user]**.

   ![](assets/fusion-organization-invite-user-350x199.png)

1. Vul het e-mailadres en de naam van de gebruiker in.
1. Selecteer een rol voor de gebruiker. Voor meer informatie over rollen, zie [Organisatiefuncties](#organization-roles) in dit document.
1. (Optioneel) Voeg een notitie toe. Deze opmerking wordt weergegeven in de e-mail met de uitnodiging die de gebruiker ontvangt.
1. Klik op **[!UICONTROL Save]**.

[!DNL Fusion] stuurt een e-mail met een uitnodiging naar de specifieke organisatie en een [!UICONTROL Accept The Role] knop.

![](assets/accept-the-role.png)

Wanneer de ontvanger op de knop klikt, wordt hij of zij omgeleid naar de uitnodigingspagina waar hij of zij de uitnodiging kan accepteren.

De uitnodiging verloopt over een dag.

>[!NOTE]
>
>Als de gebruiker nieuw is voor [!DNL Fusion], [!DNL Fusion] maakt automatisch een account voor deze gebruikers en stuurt een e-mail met een tijdelijk wachtwoord, zodat de nieuwe gebruiker zich kan aanmelden en zijn wachtwoord kan wijzigen.

## Teams

Teams zijn groepen gebruikers die toegang tot specifieke bronnen delen. Deze middelen kunnen omvatten:

* Scenarios
* Verbindingen
* Webhaken
* Toetsen
* Gegevensopslag
* Gegevensstructuren
* Instellingen voor e-mailmeldingen

>[!NOTE]
>
>Aangezien de teams toegang tot middelen controleren, is het soms nuttig voor een team om slechts ????n lid te hebben. Gebruikers in opleiding kunnen bijvoorbeeld verbindingen maken met hun individuele [!DNL Google] rekeningen. Om het even welke teamleden zouden ook met het individu kunnen verbinden [!DNL Google] account, dus in dit geval is het beter dat de gebruiker het enige lid van een trainingsteam is.

Organisaties kunnen zo veel teams hebben als ze nodig hebben en gebruikers kunnen tot een of meer teams behoren.

Gebruikers kunnen hun team selecteren in de vervolgkeuzelijst in het navigatievenster aan de linkerkant. Gebruikers zien alleen teams waarvan zij lid zijn. Als u een team selecteert, heeft de gebruiker toegang tot de bronnen van dat team.

* [Teamrollen](#team-roles)
* [Teambeheer](#team-management)

### Teamrollen

Een gebruiker heeft ????n van de volgende rollen in elk van zijn teams:

* **[!UICONTROL Team Admin]**: Naast de mogelijkheden van de andere teamrollen, staat de rol Admin de gebruiker toe om, de rol van een teamlid toe te voegen te verwijderen of te veranderen.
* **[!UICONTROL Team Member]**: De rol van het teamlid staat gebruikers toe om scenario&#39;s tot stand te brengen en uit te voeren.
* **[!UICONTROL Team Monitoring]**: De [!UICONTROL monitoring] de rol staat gebruikers toe om tot uitvoerinformatie voor scenario&#39;s toegang te hebben, maar zij kunnen scenario&#39;s ontwerpen of hun &quot;Actieve&quot;status veranderen niet.
* **[!UICONTROL Team Operator]**: De [!UICONTROL operator] de rol staat gebruikers toe om uitvoeringsgegevens te zien en de &quot;Actieve&quot;status van scenario&#39;s te veranderen.
* **[!UICONTROL Team Restricted Member]**: De functionaliteit voor deze rol is momenteel niet beschikbaar en zal in de nabije toekomst beschikbaar worden gesteld. We raden u momenteel niet aan gebruikers aan deze rol toe te wijzen.

### Teambeheer

* [Een team maken](#create-a-team)
* [Meldingsopties voor team instellen](#set-team-notification-options)

#### Een team maken

Eigenaars en beheerders van organisaties kunnen teams maken.

Een team maken:

1. Klik in het navigatievenster aan de linkerkant op **[!UICONTROL Organization]**
1. Selecteer **[!UICONTROL Team]** tab.
1. Klikken **[!UICONTROL Add a new team]** onder de lijst van teams.
1. Voer een naam in voor het nieuwe team en klik op **Toevoegen**.

#### Meldingsopties voor team instellen

De opties voor e-mailmeldingen worden ingesteld op teamniveau.

1. Klik in het navigatievenster aan de linkerkant op **[!UICONTROL Team]**
1. Selecteer **[!UICONTROL Notification Options]** tab.
1. Schakel de meldingen in die het team moet ontvangen.

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">'[!UICONTROL Warning in scenario run]'</td> 
      <td> <p>Ontvang een e-mail wanneer er een waarschuwing in een scenario looppas is</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Errors in scenario run]</td> 
      <td>Ontvang een e-mail wanneer er een fout in een scenario looppas is.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>[!UICONTROL Scenario deactivation]</p> </td> 
      <td><p>Ontvang een e-mail wanneer een scenario deactiveert.</p><p><b>Opmerking:</b> U wordt op de hoogte gesteld van deactivering van scenario's alleen wanneer het scenario automatisch is gedeactiveerd vanwege fouten. U ontvangt geen meldingen over scenario's die handmatig worden gedeactiveerd.</p><p>In sommige gevallen kan een scenario door de [!DNL Workfront Fusion] engineeringsteam omdat het scenario prestaties of andere kwesties veroorzaakt. In deze gevallen ontvangt u geen meldingen in [!DNL Workfront Fusion]. </p></td>

</tr>
</tbody>
</table>

Wijzigingen in meldingsopties worden automatisch opgeslagen

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode"> <img src="assets/organization-add-team-350x181.png" style="width: 350;height: 181;"> </p>
-->