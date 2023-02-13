---
user-type: administrator
product-area: system-administration;user-management
navigation-topic: create-and-manage-users
title: Gebruikers toevoegen
description: Als Workfront-beheerder of een gebruiker met volledige beheertoegang kunt u gebruikers toevoegen in Workfront.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: e95dbc32-915b-4ea7-a5ad-e1da99edfbe3
source-git-commit: 9bcd792139f8f2f0198da943e5c63a2add32e856
workflow-type: tm+mt
source-wordcount: '1176'
ht-degree: 0%

---

# Gebruikers toevoegen

>[!IMPORTANT]
>
>De op deze pagina beschreven procedure is alleen van toepassing op organisaties die nog niet aan boord van de Admin Console zijn gegaan. Als uw organisatie is aangemeld bij de Adobe Admin Console, moet u deze handeling uitvoeren via de Adobe Admin Console.
>
>Voor instructies voor het toevoegen van een gebruiker in de Adobe Admin Console:
>
>* Zie [Gebruikers in Workfront maken met de Adobe Admin Console](../../../administration-and-setup/add-users/create-and-manage-users/admin-console.md#create)
>* Zie de sectie Gebruikers toevoegen in het artikel [Gebruikers individueel beheren](https://helpx.adobe.com/enterprise/using/manage-users-individually.html)
>* Neem contact op met uw Adobe Admin Console-beheerder.
>
>Voor een lijst met procedures die verschillen afhankelijk van de vraag of uw organisatie al dan niet is aangemeld bij de Adobe Admin Console, raadpleegt u [Op Platform gebaseerde verschillen in beheer (Adobe Workfront/Adobe Business Platform)](../../../administration-and-setup/get-started-wf-administration/actions-in-admin-console.md).

U kunt gebruikers toevoegen in Adobe Workfront door nieuwe individuele gebruikers te maken of bestaande gebruikers te kopiëren.

Voor informatie over hoe u meerdere gebruikers tegelijk kunt importeren, raadpleegt u [Gebruikers importeren](../../../administration-and-setup/add-users/create-and-manage-users/import-users.md).

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
   <td>Plan</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraties op toegangsniveau</td> 
   <td> <p>U moet een van de volgende opties hebben:</p> 
    <ul> 
     <li> <p>Het toegangsniveau van de Beheerder van het Systeem. Zie voor meer informatie <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Volledige administratieve toegang verlenen aan een gebruiker</a>. </p> </li> 
     <li> <p><b>Gebruikers</b> het plaatsen in uw toegangsniveau dat wordt gevormd aan <b>Bewerken</b> toegang, met <b>Maken</b> en ten minste één van beide <b>Gebruikersbeheerder</b> opties ingeschakeld onder <b>Uw instellingen nauwkeurig afstellen</b> <img src="assets/gear-icon-in-access-levels.png">. </p> <p>Van deze twee opties, als Gebruiker <b>Admin (Groepgebruikers)</b> wordt toegelaten, moet u een groepsbeheerder van een groep zijn waar de gebruiker een lid is.</p> <p>Voor meer informatie over de <b>Gebruikers</b> het plaatsen in een toegangsniveau, zie <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md" class="MCXref xref">Toegang verlenen aan gebruikers</a>.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

## Vereisten

Voordat u een gebruiker toevoegt, verzamelt u de informatie over de hieronder vermelde gebruiker en bepaalt u welke informatie u aan die gebruiker wilt koppelen:

* Wat is de persoonlijke informatie van de gebruiker? U hebt minimaal het volgende nodig:

   * Volledige naam
   * Een gebruikersnaam
   * Standaardwachtwoord
   * E-mailadres

   >[!NOTE]
   >
   >U kunt bepalen of gebruikers de contactinformatie van andere gebruikers kunnen bekijken door het plaatsen van de Mening van Gebruikers te verfijnen wanneer het specificeren van toegangsniveaus voor de voorwerpen van Workfront. Zie voor meer informatie [Aangepaste toegangsniveaus maken of wijzigen](../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).

* Wat is de positie van de nieuwe gebruiker binnen het bedrijf? Heeft deze persoon directe meldingen? Aan wie rapporteert deze persoon?
* Welke functie vervult de persoon? Bestaat deze functie in Workfront? Bestaat er een limiet voor het aantal mensen dat deze functie kan vervullen? Voor informatie over het maken van taakrollen raadpleegt u [Taakrollen maken en beheren](../../../administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md).
* Welk toegangsniveau zou de gebruiker moeten hebben? Bestaat deze al of moet u een nieuwe maken? Zie voor meer informatie [Aangepaste toegangsniveaus maken of wijzigen](../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).
* In welke thuisgroep moet deze gebruiker zich bevinden? Moet de persoon in meer dan één groep zijn? Voor informatie over groepen raadpleegt u [Overzicht van groepen](../../../administration-and-setup/manage-groups/groups-overview/groups.md).
* Welk huisteam zou deze gebruiker binnen moeten zijn? Moet de persoon in meer dan één team zitten? Voor informatie over teams, zie [Teams overzicht](../../../people-teams-and-groups/create-and-manage-teams/teams-overview.md).
* Welke douaneinformatie moet u met deze gebruiker associëren?

   Als informatie over gebruikers wordt vastgelegd in aangepaste velden die u hebt gemaakt, moet u een aangepast formulier klaar hebben wanneer u een gebruiker maakt. Voor informatie over aangepaste formulieren raadpleegt u [Een aangepast formulier maken of bewerken](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md).

## Een nieuwe gebruiker maken

1. Klik op de knop **Hoofdmenu** pictogram ![](assets/main-menu-icon.png) in de rechterbovenhoek van Adobe Workfront klikt u op **Gebruikers** ![](assets/users-icon-in-main-menu.png).

1. Klikken **Nieuwe gebruiker > Nieuwe gebruiker** om een gebruiker toe te voegen die nog niet aan Workfront is toegevoegd.

   of

   Klikken **Nieuwe gebruiker > Gebruikers importeren** om gebruikers toe te voegen door een spreadsheet-importbestand te uploaden.

   Als u gebruikers importeert, hoeft u deze stappen niet uit te voeren. Zie voor meer informatie [Gebruikers importeren](../../../administration-and-setup/add-users/create-and-manage-users/import-users.md).

1. In de **Nieuwe gebruiker** vak dat wordt weergegeven, klikt u op **Geavanceerde opties tonen** en configureert u vervolgens de beschikbare opties om de gegevens van de persoon in te voeren.

   Voor informatie over deze opties raadpleegt u [Gebruikersprofiel bewerken](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

1. Voer een van de volgende handelingen uit:

   * Verlaten **Een uitnodigingsbericht sturen naar deze persoon** ingeschakeld. Als u dit doet, ontvangt de gebruiker een e-mail waar hij of zij een koppeling kan volgen om zijn of haar eigen wachtwoord voor Workfront te maken. Gebruikers die de e-mailuitnodiging niet accepteren en een Workfront-wachtwoord maken, worden in Workfront vermeld als Niet-geregistreerd.
   * Uitschakelen **Een uitnodigingsbericht sturen naar deze persoon** Typ vervolgens een **Wachtwoord** voor de persoon en bevestig deze in de **Wachtwoord bevestigen** doos. U moet dit wachtwoord delen met de gebruiker buiten Workfront.

   >[!NOTE]
   >
   >Als uw Workfront-beheerder een SSO-integratie met Workfront heeft ingeschakeld, is de optie Alleen toestaan &lt;sso configuration=&quot;&quot;> Het verificatieveld is verborgen als u de e-mailuitnodiging uitschakelt. De federatie-id of &lt;sso configuration=&quot;&quot;> Het veld Gebruikersnaam blijft zichtbaar.

   >[!NOTE]
   Als uw organisatie is aangemeld bij de Admin Console en u een gebruiker toevoegt via Workfront, kunt u geen e-mailuitnodiging verzenden.
   De nieuwe gebruikers van de Adobe worden toegevoegd aan de Admin Console, en de Admin Console levert een e-mail om hen uit te nodigen om het registratieproces te voltooien. Alle gebruikers moeten het registratieproces voltooien om tot om het even welk systeem van de Adobe toegang te hebben.
   Voor bestaande Adobe-gebruikers kan de gebruiker al dan niet een e-mail ontvangen over de beschikbaarheid van Workfront. Dit is een voorkeur die door de beheerder van de Adobe voor het product wordt gecontroleerd.

1. Klikken **Deze gebruiker toevoegen**.

   of

   Klikken **Personen gebruiker toevoegen en een andere gebruiker starten** om de nieuwe gebruiker op te slaan en een andere gebruiker toe te voegen.

## Een gebruiker kopiëren om een nieuwe te maken

U kunt een gebruiker maken door een bestaande gebruiker te kopiëren.

>[!NOTE]
Wanneer u op deze manier een gebruiker maakt, wordt alle informatie van de oorspronkelijke gebruiker naar de nieuwe gebruiker gekopieerd, behalve de volgende:
* De informatie in de Persoonlijke sectie van Info.
* Wanneer ik inlog, toon: Het standaardlandingslusje voor het toegangsniveau wordt geselecteerd in dit vakje.
* Directe rapporten
>


Nieuwe gebruiker maken door een bestaande gebruiker te kopiëren:

1. Klik op de knop **Hoofdmenu** pictogram ![](assets/main-menu-icon.png) in de rechterbovenhoek van Adobe Workfront klikt u op **Gebruikers** ![](assets/users-icon-in-main-menu.png).
1. Selecteer de gebruiker die u wilt kopiëren en klik op het pictogram Kopiëren ![](assets/copy-icon.png).
1. In de **Nieuwe gebruiker** de velden die beschikbaar zijn voor de nieuwe gebruiker bewerken.

   Voor informatie over alle gebieden verbonden aan een gebruiker, zie [Gebruikersprofiel bewerken](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

1. Klikken **Deze gebruiker toevoegen**.

   of

   Klikken **Personen gebruiker toevoegen en een andere gebruiker starten** om de nieuwe gebruiker op te slaan en een andere gebruiker toe te voegen.

Hiermee maakt u in Workfront een nieuwe account voor de gebruiker.

Als u de optie hebt geselecteerd om een uitnodiging naar de gebruiker te verzenden, ontvangt u een e-mail waarin deze een koppeling kan volgen om het Workfront-wachtwoord te maken.

>[!NOTE]
Als uw organisatie is aangemeld bij de Admin Console en u een gebruiker toevoegt via Workfront, kunt u geen e-mailuitnodiging verzenden.
De nieuwe gebruikers van de Adobe worden toegevoegd aan de Admin Console, en de Admin Console levert een e-mail om hen uit te nodigen om het registratieproces te voltooien. Alle gebruikers moeten het registratieproces voltooien om tot om het even welk systeem van de Adobe toegang te hebben.
Voor bestaande Adobe-gebruikers kan de gebruiker al dan niet een e-mail ontvangen over de beschikbaarheid van Workfront. Dit is een voorkeur die door de beheerder van de Adobe voor het product wordt gecontroleerd.
