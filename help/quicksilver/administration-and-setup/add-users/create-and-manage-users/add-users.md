---
user-type: administrator
product-area: system-administration;user-management
navigation-topic: create-and-manage-users
title: Gebruikers toevoegen
description: Als Workfront-beheerder of een gebruiker met volledige beheertoegang kunt u gebruikers toevoegen in Workfront.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: e95dbc32-915b-4ea7-a5ad-e1da99edfbe3
source-git-commit: 198129edd8690393e3214f5041b183b5516617a7
workflow-type: tm+mt
source-wordcount: '1199'
ht-degree: 0%

---

# Gebruikers toevoegen

<!--Audited 2/2024-->

>[!IMPORTANT]
>
>Als uw organisatie is aangemeld bij de Adobe Admin Console, moet u systeembeheerders maken via de Adobe Admin Console.
>
>Voor instructies bij het creëren van systeembeheerders in Adobe Admin Console, zie [ systeembeheerders in Adobe Admin Console ](/help/quicksilver/administration-and-setup/add-users/create-and-manage-users/admin-console.md) leiden.
>
>De beheerders van de groep in organisaties die aan Adobe Admin Console zijn genegeerd kunnen deze procedure gebruiken om gebruikers tot stand te brengen en de gebruiker voor admin goedkeuring voor te leggen.
>
>Voor een lijst van procedures die verschillen gebaseerd op of uw organisatie aan Adobe Admin Console is genegeerd, zie [ Op platform-gebaseerde beleidsverschillen (Adobe Workfront/Adobe Bedrijfs Platform) ](../../../administration-and-setup/get-started-wf-administration/actions-in-admin-console.md).

U kunt gebruikers toevoegen in Adobe Workfront door nieuwe individuele gebruikers te maken of bestaande gebruikers te kopiëren.

Voor informatie over hoe te om veelvoudige gebruikers gelijktijdig in te voeren, zie [ de gebruikers van de Invoer ](../../../administration-and-setup/add-users/create-and-manage-users/import-users.md).

<!--
Replace this intro with something like the following when we switch to Admin Console:
As an Adobe administrator, you can add users in Adobe Workfront by adding them to your Workfront product profile in the Adobe Admin Console. For instructions, see <a href="../../../administration-and-setup/add-users/create-and-manage-users/admin-console.md" class="MCXref xref">Manage users in the Adobe Admin Console</a>.
-->

## Toegangsvereisten

U moet het volgende hebben om de stappen in dit artikel uit te voeren:

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
   <td><p>Nieuw: Standaard</p><p>of</p><p>Huidig: Plan</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraties op toegangsniveau</td> 
   <td> <p>U moet een van de volgende opties hebben:</p> 
    <ul> 
     <li> <p>Het toegangsniveau voor systeembeheerders. Voor informatie, zie <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref"> een gebruiker volledige administratieve toegang verlenen </a>. </p> </li> 
     <li> <p><b> Gebruikers </b> het plaatsen in uw toegangsniveau dat aan <b> wordt gevormd geeft </b> toegang uit, met <b> creeert </b> en minstens één van de twee <b> die gebruikers Admin </b> opties onder <b> worden toegelaten verfijnen uw montages </b> <img src="assets/gear-icon-in-access-levels.png">. </p> <p>Van deze twee opties, als Gebruiker <b> Admin (de Gebruikers van de Groep) </b> wordt toegelaten, moet u een groepsbeheerder van een groep zijn waar de gebruiker een lid is.</p> <p>Voor meer informatie over <b> Gebruikers </b> die in een toegangsniveau plaatsen, zie <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md" class="MCXref xref"> de toegang van de Verlening tot gebruikers </a>.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

Voor meer detail over de informatie in deze lijst, zie [ vereisten van de Toegang in de documentatie van Workfront ](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

## Vereisten

Voordat u een gebruiker toevoegt, verzamelt u de informatie over de hieronder vermelde gebruiker en bepaalt u welke informatie u aan die gebruiker wilt koppelen:

* Wat is de persoonlijke informatie van de gebruiker? U hebt minimaal het volgende nodig:

   * Volledige naam
   * Een gebruikersnaam
   * Standaardwachtwoord
   * E-mailadres

  >[!NOTE]
  >
  >U kunt bepalen of gebruikers de contactinformatie van andere gebruikers kunnen bekijken door het plaatsen van de Mening van Gebruikers te verfijnen wanneer het specificeren van toegangsniveaus voor de voorwerpen van Workfront. Voor meer informatie, zie [ tot douanetoegangsniveaus ](../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md) leiden of wijzigen.

* Wat is de positie van de nieuwe gebruiker binnen het bedrijf? Heeft deze persoon directe meldingen? Aan wie rapporteert deze persoon?
* Welke functie vervult de persoon? Bestaat deze functie in Workfront? Bestaat er een limiet voor het aantal mensen dat deze functie kan vervullen? Voor informatie over het creëren van baanrollen, zie [ baanrollen ](../../../administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md) creëren en beheren.
* Welk toegangsniveau zou de gebruiker moeten hebben? Bestaat deze al of moet u een nieuwe maken? Voor meer informatie, zie [ tot douanetoegangsniveaus ](../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md) leiden of wijzigen.
* In welke thuisgroep moet deze gebruiker zich bevinden? Moet de persoon in meer dan één groep zijn? Voor informatie over groepen, zie [ Overzicht van Groepen ](../../../administration-and-setup/manage-groups/groups-overview/groups.md).
* Welk huisteam zou deze gebruiker binnen moeten zijn? Moet de persoon in meer dan één team zitten? Voor informatie over teams, zie [ Overzicht van Teams ](../../../people-teams-and-groups/create-and-manage-teams/teams-overview.md).
* Welke douaneinformatie moet u met deze gebruiker associëren?

  Als informatie over gebruikers wordt vastgelegd in aangepaste velden die u hebt gemaakt, moet u een aangepast formulier klaar hebben wanneer u een gebruiker maakt. Voor informatie over douaneformulieren, zie [ een douaneformulier ](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md) creëren of uitgeven.

## Een nieuwe gebruiker maken

1. Klik het **[!UICONTROL Main Menu]** pictogram ![ Belangrijkste Menu ](/help/_includes/assets/main-menu-icon.png) in de hoger-juiste hoek van Adobe Workfront, of (als beschikbaar), klik het **[!UICONTROL Main Menu]** pictogram ![ Belangrijkste Menu ](/help/_includes/assets/main-menu-icon-left-nav.png) in de upper-left hoek, dan klik **Gebruikers** ![](assets/users-icon-in-main-menu.png).

1. Klik **Nieuwe Gebruiker > Nieuwe Gebruiker** om een gebruiker toe te voegen die nog niet aan Workfront is toegevoegd.

   of

   Klik **Nieuwe Gebruiker > de Gebruikers van de Invoer** om gebruikers toe te voegen door een spreadsheetinvoerdossier te uploaden.

   Als u gebruikers importeert, hoeft u deze stappen niet uit te voeren. Voor meer informatie, zie [ de gebruikers van de Invoer ](../../../administration-and-setup/add-users/create-and-manage-users/import-users.md).

1. In het **Nieuwe vakje van de Gebruiker** dat verschijnt, klik **tonen Geavanceerde Opties**, dan vormen de beschikbare opties om de informatie van de persoon in te gaan.

   Voor informatie over deze opties, zie [ het profiel van een gebruiker ](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md) uitgeven.

1. Voer een van de volgende handelingen uit:

   * Het verlaten **verzendt een uitnodigingsE-mail naar deze persoon** toegelaten. Als u dit doet, ontvangt de gebruiker een e-mail waar hij of zij een koppeling kan volgen om zijn of haar eigen wachtwoord voor Workfront te maken. Gebruikers die de e-mailuitnodiging niet accepteren en een Workfront-wachtwoord maken, worden in Workfront vermeld als Niet-geregistreerd.
   * Schakel **uit verzend een uitnodigingsE-mail naar deze persoon**, dan type a **Wachtwoord** voor de persoon en bevestig het in **Bevestig Wachtwoord** doos. U moet dit wachtwoord delen met de gebruiker buiten Workfront.

   >[!NOTE]
   >
   >* Als uw Workfront-beheerder een SSO-integratie met Workfront heeft ingeschakeld, wordt het veld Alleen verificatie toestaan verborgen als u de e-mailuitnodiging uitschakelt. Het veld Federation ID of &lt;SSO Configuration> Gebruikersnaam blijft zichtbaar.
   >
   * Als uw organisatie is aangemeld bij de Admin Console en u een gebruiker toevoegt via Workfront, kunt u geen e-mailuitnodiging verzenden.
   >
   Voor bestaande gebruikers van de Adobe kan de gebruiker al dan niet een e-mail ontvangen over de beschikbaarheid van Workfront. Dit is een voorkeur die door de beheerder van de Adobe voor het product wordt gecontroleerd.

1. Klik **toevoegen Deze persoon**.

   of

   Klik **Add Persoon &amp; Begin een andere** om de nieuwe gebruiker te bewaren en een andere toe te voegen.

   >[!NOTE]
   >
   Als u een groepsbeheerder bent die een gebruiker aan een organisatie toevoegt die aan Adobe Admin Console is bezet, zijn de opties voor deze stap **gebruikers voor Goedkeuring Admin** en **voorleggen voor Goedkeuring &amp; Begin een andere**. De gebruiker wordt aangemaakt in een gedeactiveerde en in afwachting van de goedkeuringsstatus. Een Workfront-beheerder moet de gebruiker goedkeuren, die de gebruiker in Workfront activeert en deze aan de Adobe Admin Console toevoegt.

## Een gebruiker kopiëren om een nieuwe te maken

U kunt een gebruiker maken door een bestaande gebruiker te kopiëren.

>[!NOTE]
>
Wanneer u op deze manier een gebruiker maakt, wordt alle informatie van de oorspronkelijke gebruiker naar de nieuwe gebruiker gekopieerd, behalve de volgende:
>
* De informatie in de Persoonlijke sectie van Info.
* Wanneer ik login, toon: Het standaardlandende lusje voor het toegangsniveau wordt geselecteerd in dit vakje.
* Directe rapporten
>

Nieuwe gebruiker maken door een bestaande gebruiker te kopiëren:

1. Klik het **[!UICONTROL Main Menu]** pictogram ![ Belangrijkste Menu ](/help/_includes/assets/main-menu-icon.png) in de hoger-juiste hoek van Adobe Workfront, of (als beschikbaar), klik het **[!UICONTROL Main Menu]** pictogram ![ Belangrijkste Menu ](/help/_includes/assets/main-menu-icon-left-nav.png) in de upper-left hoek, dan klik **Gebruikers** ![](assets/users-icon-in-main-menu.png).
1. Selecteer de gebruiker die u wilt kopiëren en klik op het pictogram Kopiëren ![](assets/copy-icon.png) .
1. In het **vakje van de Gebruiker van het Exemplaar** dat toont, geef de gebieden beschikbaar voor de nieuwe gebruiker uit.

   Voor informatie over alle gebieden verbonden aan een gebruiker, zie [ het profiel van een gebruiker ](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md) uitgeven.

1. Klik **toevoegen Deze persoon**.

   of

   Klik **Add Persoon &amp; Begin een andere** om de nieuwe gebruiker te bewaren en een andere toe te voegen.

Hiermee maakt u in Workfront een nieuwe account voor de gebruiker.

Als u de optie hebt geselecteerd om een uitnodiging naar de gebruiker te verzenden, ontvangt u een e-mail waarin deze een koppeling kan volgen om het Workfront-wachtwoord te maken.

>[!NOTE]
>
Als uw organisatie is aangemeld bij de Admin Console en u een gebruiker toevoegt via Workfront, kunt u geen e-mailuitnodiging verzenden.
>
Voor bestaande gebruikers van de Adobe kan de gebruiker al dan niet een e-mail ontvangen over de beschikbaarheid van Workfront. Dit is een voorkeur die door de beheerder van de Adobe voor het product wordt gecontroleerd.
