---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations;user-management
navigation-topic: organizations
title: Adobe Workfront Fusion organisaties en teams
description: De Adobe Workfront Fusion-documentatie is verplaatst naar een nieuwe locatie. Dit artikel is vervangen, maar bevat een koppeling naar het nieuwe artikel dat deze functionaliteit behandelt.
author: Becky
feature: Workfront Fusion
exl-id: 601e937f-0286-4557-9a87-59aa9c0c22f1
source-git-commit: 2d6af8b4988bd9aab7381daa79dec79e41408c45
workflow-type: tm+mt
source-wordcount: '1237'
ht-degree: 0%

---

# [!DNL Adobe Workfront Fusion] organisaties en teams

>[!IMPORTANT]
>
>De Adobe Workfront Fusion-documentatie is verplaatst naar een nieuwe locatie.
>
>De informatie in dit artikel is nu te vinden in de artikelen:
>
>* [ overzicht van de organisaties en de teams van de Fusie van Adobe Workfront ](https://experienceleague.adobe.com/docs/workfront-fusion/using/set-up-and-manage-fusion/set-up-and-manage-orgs-and-teams/set-up-orgs-teams-and-users/org-and-team-overview.html)
>* [ plaats de Opties van het Bericht van het Team ](https://experienceleague.adobe.com/docs/workfront-fusion/using/set-up-and-manage-fusion/set-up-and-manage-orgs-and-teams/set-up-orgs-teams-and-users/set-team-notification-options.html)
>
>Werk eventuele bladwijzers bij.
>
>Dit artikel wordt niet meer bijgewerkt en wordt in de nabije toekomst verwijderd.

Met de functies Organisatie en Teams van [!DNL Adobe Workfront Fusion] kunnen bedrijven de toegang tot scenario&#39;s en andere functies in Fusion beheren.

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
   <td>
   <p>Huidige licentievereiste: geen [!DNL Workfront Fusion] licentievereiste.</p>
   <p>of</p>
   <p>Vereiste voor verouderde licentie: [!UICONTROL [!DNL Workfront Fusion] voor werkautomatisering en -integratie], [!UICONTROL [!DNL Workfront Fusion] voor werkautomatisering]</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Product</td> 
   <td>
   <p>Huidige productvereiste: als u het [!UICONTROL Select] - of [!UICONTROL Prime] [!DNL Adobe Workfront] -abonnement hebt, moet uw organisatie [!DNL Adobe Workfront Fusion] en [!DNL Adobe Workfront] aanschaffen om de in dit artikel beschreven functionaliteit te kunnen gebruiken. [!DNL Workfront Fusion] wordt opgenomen in het [!UICONTROL Ultimate] [!DNL Workfront] -abonnement.</p>
   <p>of</p>
   <p>Vereiste verouderd product: uw organisatie moet [!DNL Adobe Workfront Fusion] en [!DNL Adobe Workfront] aanschaffen om de in dit artikel beschreven functionaliteit te kunnen gebruiken.</p>
   </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">Configuraties op toegangsniveau*</td> 
   <td> 
     <p>U moet een [!DNL Workfront Fusion] beheerder voor uw organisatie zijn.</p>
     <p>U moet een [!DNL Workfront Fusion] beheerder voor uw team zijn.</p>
   </td> 
  </tr> 
 </tbody> 
</table>

Neem contact op met de [!DNL Workfront] -beheerder als u wilt weten welk abonnement, licentietype of toegang u hebt.

<p>**Zie <a href="../../workfront-fusion/get-started/license-automation-vs-integration.md" class="MCXref xref">[!DNL Adobe Workfront Fusion] licenties </a> voor informatie over [!DNL Adobe Workfront Fusion] -licenties.</p>


## Organisaties

[!DNL Workfront Fusion] -gebruikers behoren tot een organisatie.

* [Organisatiefuncties](#organization-roles)
* [Gebruikers uitnodigen voor een organisatie](#inviting-users-to-an-organization)
* [Overschakelen tussen organisaties](#switch-between-organizations)

### Organisatiefuncties

Een gebruiker heeft een van de volgende rollen in een organisatie:

* **[!UICONTROL Owner]**: De eigenaar heeft alle machtigingen die beschikbaar zijn in de organisatie.
* **[!UICONTROL Admin]**: Met de beheerrol kan een gebruiker teams en gebruikers voor de organisatie maken en beheren.
* **[!UICONTROL Member]**: leden kunnen [!DNL Workfront Fusion] gebruiken, maar kunnen geen organisatorische wijzigingen aanbrengen.
* **[!UICONTROL Accountant]**: gebruikers kunnen met een accountantsrol alleen licentiegegevens op het dashboard van de organisatie zien.
* **[!UICONTROL App Developer]**: De functionaliteit voor deze rol is momenteel niet beschikbaar en wordt in de nabije toekomst beschikbaar gesteld. We raden u momenteel niet aan gebruikers aan deze rol toe te wijzen.

Voor informatie over specifieke acties beschikbaar aan gebruikers in elke organisatierol, zie [ Organisatie en teamrollen ](/help/quicksilver/workfront-fusion/organizations/organization-roles.md).

### Gebruikers uitnodigen voor een organisatie

Door gebrek, kan een organisatieeigenaar (of erkende gebruiker) een andere persoon uitnodigen om zich bij hun organisatie aan te sluiten.

Een gebruiker uitnodigen om deel te nemen aan een organisatie:

1. Klik op **[!UICONTROL Change details]** in de rechterbovenhoek van het scherm.
1. Selecteer **[!UICONTROL Invite a new user]** .

   ![](assets/fusion-organization-invite-user-350x199.png)

1. Vul het e-mailadres en de naam van de gebruiker in.
1. Selecteer een rol voor de gebruiker. Voor meer informatie over rollen, zie {de rollen van 0} Organisatie ](#organization-roles) in dit document.[
1. (Optioneel) Voeg een notitie toe. Deze opmerking wordt weergegeven in de e-mail met de uitnodiging die de gebruiker ontvangt.
1. Klik op **[!UICONTROL Save]**.

[!DNL Fusion] verzendt een e-mail met een uitnodiging naar de specifieke organisatie en een knop [!UICONTROL Accept The Role] .

Wanneer de ontvanger op de knop klikt, wordt hij of zij omgeleid naar de uitnodigingspagina waar hij of zij de uitnodiging kan accepteren.

De uitnodiging verloopt over een dag.

>[!NOTE]
>
>Als de gebruiker [!DNL Fusion] nog niet eerder heeft gebruikt, maakt [!DNL Fusion] automatisch een account voor de gebruiker en verzendt deze een e-mail met een tijdelijk wachtwoord, waarmee de nieuwe gebruiker zich kan aanmelden en zijn wachtwoord kan wijzigen.

### Overschakelen tussen organisaties

U kunt deel uitmaken van meer dan één organisatie in Fusion. De middelen worden niet gedeeld tussen organisaties.

U kunt organisaties binnen de Adobe Verenigde Ervaring schakelen door de organisatienaam in de hoger-juiste hoek te klikken en de nieuwe organisatie van dropdown te selecteren. Alleen organisaties met een Fusion-account worden in het vervolgkeuzemenu weergegeven, zelfs als u lid bent van andere organisaties in de Adobe.

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
>Aangezien de teams toegang tot middelen controleren, is het soms nuttig voor een team om slechts één lid te hebben. Gebruikers in opleiding kunnen bijvoorbeeld verbindingen maken met hun individuele [!DNL Google] -accounts. Om het even welke teamleden zouden ook met de individuele [!DNL Google] rekening kunnen verbinden, zodat in dit geval is het best dat de gebruiker het enige lid van een trainingsteam is.

Organisaties kunnen zo veel teams hebben als ze nodig hebben en gebruikers kunnen tot een of meer teams behoren.

Gebruikers kunnen hun team selecteren in de vervolgkeuzelijst in het navigatievenster aan de linkerkant. Gebruikers zien alleen teams waarvan zij lid zijn. Als u een team selecteert, heeft de gebruiker toegang tot de bronnen van dat team.

* [Teamrollen](#team-roles)
* [Teambeheer](#team-management)

### Teamrollen

Een gebruiker heeft één van de volgende rollen in elk van zijn teams:

* **[!UICONTROL Team Admin]**: Naast de mogelijkheden van de andere teamrollen, staat de rol Admin de gebruiker toe om, de rol van een teamlid toe te voegen te verwijderen of te veranderen.
* **[!UICONTROL Team Member]**: De rol van het teamlid staat gebruikers toe om scenario&#39;s tot stand te brengen en uit te voeren.
* **[!UICONTROL Team Monitoring]**: Met de rol [!UICONTROL monitoring] hebben gebruikers toegang tot uitvoeringsinformatie voor scenario&#39;s, maar ze kunnen geen scenario&#39;s ontwerpen of hun status Actief wijzigen.
* **[!UICONTROL Team Operator]**: met de rol [!UICONTROL operator] kunnen gebruikers uitvoeringsgegevens zien en de status Actief van scenario&#39;s wijzigen.
* **[!UICONTROL Team Restricted Member]**: De functionaliteit voor deze rol is momenteel niet beschikbaar en wordt in de nabije toekomst beschikbaar gesteld. We raden u momenteel niet aan gebruikers aan deze rol toe te wijzen.

Voor informatie over specifieke acties beschikbaar aan gebruikers in elke teamrol, zie [ Organisatie en teamrollen ](/help/quicksilver/workfront-fusion/organizations/organization-roles.md).

### Teambeheer

* [Een team maken](#create-a-team)
* [Meldingsopties voor team instellen](#set-team-notification-options)

#### Een team maken

Eigenaars en beheerders van organisaties kunnen teams maken.

Een team maken:

1. Klik in het navigatievenster links op **[!UICONTROL Organization]**
1. Selecteer de tab **[!UICONTROL Team]** .
1. Klik op **[!UICONTROL Add a new team]** onder de lijst met teams.
1. Ga een naam voor het nieuwe team in, en klik **toevoegen**.

#### Meldingsopties voor team instellen

>[!NOTE]
>
>Als uw organisatie aan Verenigde Shell is bewogen, ontvangt u berichten door het gebied van de Berichten van de Adobe. U moet de Verenigde ervaring van Shell gebruiken om berichten op het gebied van de Berichten van de Adobe te kunnen zien.
>
>Om de Verenigde Ervaring van Shell, met inbegrip van het gebied van de Berichten van de Adobe te gebruiken, klik de Uitgezochte Nieuwe Fusie UI in Verenigde knoop van de Ervaring dichtbij de bovenkant van de pagina. Deze knoop is slechts beschikbaar als uw organisatie aan Verenigde Shell heeft bewogen.
>
>Voor meer informatie, zie [ Toegang tot uw berichten ](/help/quicksilver/workfront-fusion/fusion-in-admin-console/fusion-unified-experience.md#access-your-notifications) in [!DNL Adobe Unified Experience] voor [!DNL Workfront Fusion].

De opties voor e-mailmeldingen worden ingesteld op teamniveau.

1. Klik in het navigatievenster links op **[!UICONTROL Team]**
1. Selecteer de tab **[!UICONTROL Notification Options]** .
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
      <td><p>Ontvang een e-mail wanneer een scenario deactiveert.</p><p><b> Nota:</b> u wordt op de hoogte gebracht over scenario deactivatie slechts wanneer het scenario automatisch wegens fouten is gedeactiveerd. U ontvangt geen meldingen over scenario's die handmatig worden gedeactiveerd.</p><p>In sommige gevallen wordt een scenario mogelijk gedeactiveerd door het engineeringteam van [!DNL Workfront Fusion] omdat het scenario prestaties of andere problemen veroorzaakt. In deze gevallen ontvangt u geen meldingen in [!DNL Workfront Fusion] . </p></td>

</tr>
</tbody>
</table>

Wijzigingen in meldingsopties worden automatisch opgeslagen

#### Schakelen tussen teams

U kunt deel uitmaken van meer dan één team in Fusion. Aangezien de teams geen middelen delen, kunt u teams moeten schakelen om tot specifieke scenario&#39;s of andere middelen toegang te hebben.

Als uw organisatie niet op de Adobe Verenigde Ervaring is, kunt u teams schakelen door de teamnaam in de linkernavigatie te klikken, dan selecterend een team van dropdown.

Als uw team op de Adobe Verenigde Ervaring is, kunt u een nieuw team selecteren door op de teamnaam in de kopbal te klikken, dan selecterend een team van dropdown. Deze optie is beschikbaar bij alle pagina&#39;s die voor een bepaald team, zoals een scenario pagina of de pagina van Verbindingen specifiek zijn.

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode"> <img src="assets/organization-add-team-350x181.png" style="width: 350;height: 181;"> </p>
-->