---
user-type: administrator
product-area: system-administration;user-management
navigation-topic: create-and-manage-users
title: Gebruikers toevoegen
description: Als Workfront-beheerder of een gebruiker met volledige beheertoegang kunt u gebruikers toevoegen in Workfront.
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: e95dbc32-915b-4ea7-a5ad-e1da99edfbe3
source-git-commit: c711541f3e166f9700195420711d95ce782a44b2
workflow-type: tm+mt
source-wordcount: '1276'
ht-degree: 0%

---

# Gebruikers toevoegen

<!--Audited 2/2024-->

>[!IMPORTANT]
>
>* **als uw organisatie aan Adobe Admin Console is bezet, moet u systeembeheerders door Adobe Admin Console tot stand brengen.**
>
>   Voor instructies bij het creëren van systeembeheerders in Adobe Admin Console, zie [&#x200B; gebruikers in Adobe Admin Console &#x200B;](/help/quicksilver/administration-and-setup/add-users/create-and-manage-users/admin-console.md) leiden.
>
>   De beheerders van de groep in organisaties die aan Adobe Admin Console zijn genegeerd kunnen deze procedure gebruiken om gebruikers tot stand te brengen en de gebruiker voor admin goedkeuring voor te leggen.
>
>   Voor een lijst van procedures die verschillen gebaseerd op of uw organisatie aan Adobe Admin Console is genegeerd, zie [&#x200B; Op platform-gebaseerde beleidsverschillen (Adobe Workfront/Adobe Bedrijfsplatform) &#x200B;](../../../administration-and-setup/get-started-wf-administration/actions-in-admin-console.md).
>
>* **als uw organisatie Enige Sign-On (SSO)** gebruikt, adviseren wij het creëren van gebruikers en het toewijzen van hen aan Workfront in Adobe Admin Console. Het is mogelijk deze gebruikers te maken in Workfront, maar er kunnen zich problemen voordoen bij het doorgeven van die informatie naar de Adobe Admin Console, op basis van de configuratie van de Admin Console van uw organisatie.
>  &#x200B;>   Nadat u de gebruiker in de Adobe Admin Console hebt gemaakt, kunt u de gebruikersgegevens in Workfront configureren, zoals het toewijzen van rollen, groepen, teams en toegangsniveaus.
>* **als uw organisatie geen Enige Sign-On (SSO)** gebruikt, kunt u niet-systeembeheerdergebruikers direct in Workfront toevoegen. Het is mogelijk om gebruikers toe te voegen in de Adobe Admin Console, maar als u ze toevoegt in Workfront, kunt u hun toegangsniveau instellen terwijl u ze maakt. Op die manier kunt u tijd besparen.



U kunt gebruikers toevoegen in Adobe Workfront door nieuwe individuele gebruikers te maken of bestaande gebruikers te kopiëren.

Voor informatie over hoe te om veelvoudige gebruikers gelijktijdig in te voeren, zie [&#x200B; de gebruikers van de Invoer &#x200B;](../../../administration-and-setup/add-users/create-and-manage-users/import-users.md).

<!--
Replace this intro with something like the following when we switch to Admin Console:
As an Adobe administrator, you can add users in Adobe Workfront by adding them to your Workfront product profile in the Adobe Admin Console. For instructions, see <a href="../../../administration-and-setup/add-users/create-and-manage-users/admin-console.md" class="MCXref xref">Manage users in the Adobe Admin Console</a>.
-->

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
   <td><p>Standard</p><p>Plan</p></td> 
  </tr> 
  <tr> 
   <td>Configuraties op toegangsniveau</td> 
   <td> <p>U moet een van de volgende opties hebben:</p> 
    <ul> 
     <li> <p>Het toegangsniveau voor systeembeheerders. </li> 
     <li> <p><b> Gebruikers </b> het plaatsen in uw toegangsniveau dat aan <b> wordt gevormd geeft </b> toegang uit, met <b> creeert </b> en minstens één van de twee <b> die gebruikers Admin </b> opties onder <b> worden toegelaten verfijnen uw montages </b> <img src="assets/gear-icon-in-access-levels.png">. </p> <p>Van deze twee opties, als <b> Admin van de Gebruiker (de Gebruikers van de Groep) </b> wordt toegelaten, moet u een groepsbeheerder van een groep zijn waar de gebruiker een lid is.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

Voor informatie, zie [&#x200B; vereisten van de Toegang in de documentatie van Workfront &#x200B;](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Vereisten

Voordat u een gebruiker toevoegt, verzamelt u de informatie over de hieronder vermelde gebruiker en bepaalt u welke informatie u aan die gebruiker wilt koppelen:

* Wat is de persoonlijke informatie van de gebruiker? U hebt minimaal het volgende nodig:

   * Volledige naam
   * Een gebruikersnaam
   * Standaardwachtwoord
   * E-mailadres

  >[!NOTE]
  >
  >U kunt bepalen of gebruikers de contactinformatie van andere gebruikers kunnen bekijken door het plaatsen van de Mening van Gebruikers te verfijnen wanneer het specificeren van toegangsniveaus voor de voorwerpen van Workfront. Voor meer informatie, zie [&#x200B; tot douanetoegangsniveaus &#x200B;](../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md) leiden of wijzigen.

* Wat is de positie van de nieuwe gebruiker binnen het bedrijf? Heeft deze persoon directe meldingen? Aan wie rapporteert deze persoon?
* Welke functie vervult de persoon? Bestaat deze functie in Workfront? Bestaat er een limiet voor het aantal mensen dat deze functie kan vervullen? Voor informatie over het creëren van baanrollen, zie [&#x200B; baanrollen &#x200B;](../../../administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md) creëren en beheren.
* Welk toegangsniveau zou de gebruiker moeten hebben? Bestaat deze al of moet u een nieuwe maken? Voor meer informatie, zie [&#x200B; tot douanetoegangsniveaus &#x200B;](../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md) leiden of wijzigen.
* In welke thuisgroep moet deze gebruiker zich bevinden? Moet de persoon in meer dan één groep zijn? Voor informatie over groepen, zie [&#x200B; Overzicht van Groepen &#x200B;](../../../administration-and-setup/manage-groups/groups-overview/groups.md).
* Welk huisteam zou deze gebruiker binnen moeten zijn? Moet de persoon in meer dan één team zitten? Voor informatie over teams, zie [&#x200B; Overzicht van Teams &#x200B;](../../../people-teams-and-groups/create-and-manage-teams/teams-overview.md).
* Welke douaneinformatie moet u met deze gebruiker associëren?

  Als informatie over gebruikers wordt vastgelegd in aangepaste velden die u hebt gemaakt, moet u een aangepast formulier klaar hebben wanneer u een gebruiker maakt. Voor informatie over douaneformulieren, zie [&#x200B; een douaneformulier &#x200B;](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md) creëren.

## Een nieuwe gebruiker maken

{{step-1-to-users}}

1. Klik **Nieuwe Gebruiker > Nieuwe Gebruiker** om een gebruiker toe te voegen die nog niet aan Workfront is toegevoegd.

   of

   Klik **Nieuwe Gebruiker > de Gebruikers van de Invoer** om gebruikers toe te voegen door een spreadsheetinvoerdossier te uploaden.

   Als u gebruikers importeert, hoeft u deze stappen niet uit te voeren. Voor meer informatie, zie [&#x200B; de gebruikers van de Invoer &#x200B;](../../../administration-and-setup/add-users/create-and-manage-users/import-users.md).

1. In het **Nieuwe vakje van de Gebruiker** dat verschijnt, klik **tonen Geavanceerde Opties**, dan vormen de beschikbare opties om de informatie van de persoon in te gaan.

   Voor informatie over deze opties, zie [&#x200B; het profiel van een gebruiker &#x200B;](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md) uitgeven.

1. Voer een van de volgende handelingen uit:

   * Het verlaten **verzendt een uitnodigingsE-mail naar deze persoon** toegelaten. Als u dit doet, ontvangt de gebruiker een e-mail waar hij of zij een koppeling kan volgen om zijn of haar eigen wachtwoord voor Workfront te maken. Gebruikers die de e-mailuitnodiging niet accepteren en een Workfront-wachtwoord maken, worden in Workfront vermeld als Niet-geregistreerd.
   * Schakel **uit verzend een uitnodigingsE-mail naar deze persoon**, dan type a **Wachtwoord** voor de persoon en bevestig het in **Bevestig Wachtwoord** doos. U moet dit wachtwoord delen met de gebruiker buiten Workfront.

   >[!NOTE]
   >
   >* Als uw Workfront-beheerder een SSO-integratie met Workfront heeft ingeschakeld, wordt het veld Alleen verificatie toestaan verborgen als u de e-mailuitnodiging uitschakelt. Het veld Federation ID of &lt;SSO Configuration> Gebruikersnaam blijft zichtbaar.
   >
   >* Als uw organisatie is aangemeld bij de Admin Console en u een gebruiker toevoegt via Workfront, kunt u geen e-mailuitnodiging verzenden.
   >
   >   Voor bestaande Adobe-gebruikers kan de gebruiker al dan niet een e-mail ontvangen over de beschikbaarheid van Workfront. Deze voorkeur wordt door de Adobe-beheerder voor het product bepaald.

1. Klik **toevoegen Deze persoon**.

   of

   Klik **Add Persoon &amp; Begin een andere** om de nieuwe gebruiker te bewaren en een andere toe te voegen.

   >[!NOTE]
   >
   >* Als u een groepsbeheerder bent die een gebruiker aan een organisatie toevoegt die aan Adobe Admin Console is bezet, zijn de opties voor deze stap **gebruikers voor Goedkeuring Admin** en **voorleggen voor Goedkeuring &amp; Begin een andere**. De gebruiker wordt aangemaakt in een gedeactiveerde en in afwachting van de goedkeuringsstatus.
   > 
   >* Als de gebruiker zich niet binnen een paar minuten uit de status Gedetactiveerd en In afwachting van goedkeuring beweegt, en het scherm vernieuwt verwijdert niet het symbool In afwachting van goedkeuring, kunt u de gebruiker manueel goedkeuren.
   >
   >   1. Ga naar Instellingen > Gebruikers.
   >   1. Selecteer de gebruiker of gebruikers in de lijst Gebruikers.
   >   1. Klik op het menu met drie punten in de lijstkop.
   >   1. Selecteer **goedkeuren**.
   >   1. Vernieuw de pagina na een paar minuten.


## Een gebruiker kopiëren om een nieuwe te maken

U kunt een gebruiker maken door een bestaande gebruiker te kopiëren.

>[!NOTE]
>
>Wanneer u op deze manier een gebruiker maakt, wordt alle informatie van de oorspronkelijke gebruiker naar de nieuwe gebruiker gekopieerd, behalve de volgende:
>
>* De informatie in de Persoonlijke sectie van Info.
>* Wanneer ik login, toon: Het standaardlandende lusje voor het toegangsniveau wordt geselecteerd in dit vakje.
>* Directe rapporten
>

Nieuwe gebruiker maken door een bestaande gebruiker te kopiëren:

{{step-1-to-users}}

1. Selecteer de gebruiker die u wilt kopiëren, dan het pictogram van het Exemplaar ![&#x200B; pictogram van het Exemplaar &#x200B;](assets/copy-icon.png) klikken.
1. In het **vakje van de Gebruiker van het Exemplaar** dat toont, geef de gebieden beschikbaar voor de nieuwe gebruiker uit.

   Voor informatie over alle gebieden verbonden aan een gebruiker, zie [&#x200B; het profiel van een gebruiker &#x200B;](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md) uitgeven.

1. Klik **toevoegen Deze persoon**.

   of

   Klik **Add Persoon &amp; Begin een andere** om de nieuwe gebruiker te bewaren en een andere toe te voegen.

Hiermee maakt u in Workfront een nieuwe account voor de gebruiker.

Als u de optie hebt geselecteerd om een uitnodiging naar de gebruiker te verzenden, ontvangt u een e-mail waarin deze een koppeling kan volgen om het Workfront-wachtwoord te maken.

>[!NOTE]
>
>Als uw organisatie is aangemeld bij de Admin Console en u een gebruiker toevoegt via Workfront, kunt u geen e-mailuitnodiging verzenden.
>
>Voor bestaande Adobe-gebruikers kan de gebruiker al dan niet een e-mail ontvangen over de beschikbaarheid van Workfront. Deze voorkeur wordt door de Adobe-beheerder voor het product bepaald.
