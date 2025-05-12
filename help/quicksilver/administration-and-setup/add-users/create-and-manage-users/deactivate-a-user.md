---
title: Een gebruiker deactiveren of opnieuw activeren
user-type: administrator
product-area: system-administration;user-management
navigation-topic: create-and-manage-users
description: Workfront-beheerders kunnen een gebruiker deactiveren of opnieuw activeren.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: aba243ba-46c2-4eb7-b704-4368bf0ae3cc
source-git-commit: b235945deb3254feaf671083fc992786851a3286
workflow-type: tm+mt
source-wordcount: '1104'
ht-degree: 0%

---

# Een gebruiker deactiveren of opnieuw activeren {#deactivate-or-reactivate-a-user}

>[!CONTEXTUALHELP]
>id="wf_users_deactivate_user"
>title="Een gebruiker deactiveren"
>abstract="Als u een gebruiker deactiveert, worden deze verwijderd uit Workfront en Frame.io. Gedetactiveerde gebruikers kunnen later opnieuw worden geactiveerd."

<!--Audited 5/2025-->

<!--

>[!IMPORTANT]
>
>The procedure described on this page applies only to organizations that have not yet been onboarded to the Admin Console. If your organization has been onboarded to the Adobe Admin Console, you must perform this action through the Adobe Admin Console.
>
>For instructions on deactivating a user in the Adobe Admin Console, see the section "Remove users" in the article [Manage users individually](https://helpx.adobe.com/nl/enterprise/using/manage-users-individually.html) or contact your Adobe Admin Console Administrator.
>
>For a list of procedures that differ based on whether your organization has been onboarded to the Adobe Admin Console, see [Platform-based administration differences (Adobe Workfront/Adobe Business Platform)](../../../administration-and-setup/get-started-wf-administration/actions-in-admin-console.md).

-->

Als een gebruiker de organisatie verlaat, is het raadzaam deze in het systeem te deactiveren om verwarring voor andere gebruikers te voorkomen wanneer ze aan updates toevoegen of ze aan updates toewijzen. Wanneer u een gebruiker deactiveert, zien andere gebruikers niet langer hun naam wanneer zij naar mensen in het systeem zoeken.

De beheerders kunnen inactieve gebruikers in het gebied van de Opstelling zien.

U kunt een gebruiker op elk gewenst moment opnieuw activeren.

>[!IMPORTANT]
>
>* Wij adviseren dat u gebruikers deactiveert die de organisatie hebben verlaten eerder dan hen te schrappen. Als een gebruiker wordt verwijderd, gaat alle aan die gebruiker gekoppelde geschiedenis in Workfront verloren. Hieronder vallen hun werktoewijzingen, hun koppeling met notities, uren, documenten en alle andere objecten die ze ooit hebben gemaakt.
>
>* Als u een gebruiker in Workfront deactiveert, worden de gebruikerslicenties zowel voor Workfront als voor digitale proefdrukken verwijderd. Bovendien kan aan de gebruiker geen werk meer worden toegewezen. Wanneer een gebruiker wordt gedeactiveerd, wordt de Workfront-licentie en -proeflicentie van die gebruiker beschikbaar voor gebruik door een andere gebruiker. Alle andere informatie in het profiel van de gedeactiveerde gebruiker blijft ongewijzigd.
>
>* Als u een gebruiker deactiveert in Workfront, wordt de gebruiker niet verwijderd uit het Workfront-productprofiel in de Adobe Admin Console. Voor meer informatie, zie [ gebruikers van de Schrapping ](../../../administration-and-setup/add-users/create-and-manage-users/delete-a-user.md).


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
   <td><p>Nieuw: Standaard</p><p>of</p><p>Huidig: Plan</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraties op toegangsniveau</td> 
   <td> <p>U moet een van de volgende opties hebben:</p> 
    <ul> 
     <li> <p>Het toegangsniveau voor systeembeheerders. </li> 
     <li> <p>Gebruikers die in uw toegangsniveau instellen, zijn geconfigureerd voor het bewerken van toegang, met Maken en ten minste een van de twee opties voor gebruikersbeheer ingeschakeld onder Uw instellingen nauwkeurig instellen <img src="assets/gear-icon-in-access-levels.png"> . </p> <p>Van deze twee opties, als de Gebruiker Admin (de Gebruikers van de Groep) wordt toegelaten, moet u een groepbeheerder van een groep zijn waar de gebruiker een lid is.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

Voor meer detail over de informatie in deze lijst, zie [ vereisten van de Toegang in de documentatie van Workfront ](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Vereisten

Voordat u een Workfront-beheerder of een gebruiker van een Standard- of Plan-licentie deactiveert, moet u de objecten en activiteiten aan een andere gebruiker koppelen.

Voor meer informatie, zie [ Ongeveer het deactiveren van de beheerders van Workfront en de gebruikers van de vergunning van het Plan ](#about-deactivating-workfront-administrators-and-plan-license-users) in dit artikel.

## Een gebruiker deactiveren

Houd rekening met het volgende wanneer u een gebruiker deactiveert:

* De gebruiker zal niet tot het systeem kunnen toegang hebben.
<!--* The user will be removed from Frame.io review links, assets, projects, and accounts.
   * Reactivating the user does not automatically add them back to the Frame.io items. You must reassign the user manually to Workfront projects, tasks, and assets that require Frame.io collaboration.-->
* Alle gegevens die aan de gebruiker zijn gekoppeld, blijven behouden.
* U kunt een gedeactiveerde gebruikerslicentie toewijzen aan een andere gebruiker.

Een gebruiker deactiveren:

{{step-1-to-users}}

1. Selecteer een gebruiker in de gebruikerslijst.
1. Klik het **Meer** pictogram ![ Meer pictogram ](assets/more-icon.png), dan klik **deactivate**.

1. In het **Deactivate gebruikers** dialoogvakje, klik **&#x200B;**&#x200B;deactivate.

## Gebruikers plannen voor deactivering

Als manager, kunt u gebruikers voor deactivering willen merken alvorens zij eigenlijk uw organisatie verlaten. Bijvoorbeeld, als u met een gebruiker werkt die contractueel verbindend is, zijn zij in uw systeem voor een beperkte periode, en u kent hun beëindigingsdatum. U kunt ze plannen om op die datum gedeactiveerd te worden.

Workfront-beheerders en gebruikers van een abonnement kunnen de datum van deactivering in hun gebruikersprofiel zien.

Een gebruiker plannen voor deactivering:

{{step-1-to-users}}

1. Selecteer de gebruiker in de gebruikerslijst.

   of

   (Optioneel) Selecteer meerdere gebruikers om ze bulksgewijs te deactiveren.

1. Klik **uitgeven** pictogram ![ uitgeven pictogram ](assets/edit-icon.png).
1. In het linkerpaneel van **geef de doos van de Gebruiker** uit, klik **Planning van het Middel**.
1. Selecteer het **checkbox van de Deactivering van het Programma**.

1. Selecteer de datum en de tijd voor de **Geplande Datum van Deactivering**.

   >[!NOTE]
   >
   >* In het tijdvak kunt u alleen stappen van een heel uur selecteren, geen minuten.
   >* Als u een tijd voor de huidige dag selecteert die is overgegaan, zal Workfront de deactivering voor de volgende dag om 12:00 plannen.
   >* De geselecteerde tijd komt overeen met de tijdzone van de computer van de gebruiker die de deactivering plant.

1. Klik **sparen Veranderingen**.

De gebruiker wordt op de geselecteerde dag ergens na de geselecteerde tijd gedeactiveerd. Als u meerdere gebruikers hebt geselecteerd om bulksgewijs te deactiveren, worden alle geselecteerde gebruikers op de geselecteerde dag gedeactiveerd ergens na de geselecteerde tijd.

Wij adviseren dat u een rapport voor gebruikers bouwt die u voor deactivering hebt gepland om op de hoogte te houden van welke gebruikers om te worden gedeactiveerd. Er is geen bevestiging dat de deactivering heeft plaatsgevonden nadat de gebruikers zijn gedeactiveerd.

## Een gebruiker opnieuw activeren

{{step-1-to-users}}

1. Selecteer een gebruiker, klik het **Meer** pictogram ![ Meer pictogram ](assets/more-icon.png), dan klik **activeert**.

1. In het **Reactivate gebruiker** dialoog, selecteer een nieuw **niveau van de Toegang** in het drop-down menu, dan klik **Reactivate**.
<!--
### Asset review and approval impact when you reactivate a user

Deactivated users lose access to their assigned Frame.io accounts as well as assigned projects, assets, and review links. If you choose to reactivate the user, you must manually reassign them to projects, tasks, and assets that require Frame.io collaboration. -->

### Bewijseffect wanneer u een gebruiker opnieuw activeert

Gedeactiveerde gebruikers verliezen hun toegewezen standaardproofingrol en hun proefdruklicentie (als u op een Workfront Premium Legacy Plan bent). Als u ervoor kiest de gebruiker opnieuw te activeren, moet u:

* Wijs de licentie opnieuw toe (als u een Workfront Premium Legacy Plan gebruikt). Voor meer informatie over het proefdrukken van Workfront plannen, zie [ Toegang tot het proefdrukken functionaliteit in Workfront ](../../../administration-and-setup/manage-workfront/configure-proofing/access-to-proofing-functionality.md).
* Controleer of ze de juiste proefdrukrol hebben. De opnieuw geactiveerde proefdrukgebruikers worden toegewezen wat als standaardproefrol voor nieuwe gebruikers wordt gespecificeerd. Zie [ standaard het proef rollen ](../../../administration-and-setup/manage-workfront/configure-proofing/configure-default-proofing-roles.md) voor meer informatie vormen.

## Informatie over het deactiveren van Workfront-beheerders en gebruikers van een Standard- of Plan-licentie

Alvorens u een beheerder van Workfront of een gebruiker met een vergunning van het Plan deactiveert, is het belangrijk om op de voorwerpen en de activiteiten van Workfront te controleren die die persoon impliceren, dan hen te associëren met een andere beheerder van Workfront of de vergunningsgebruiker van het Plan zonodig.

Deze objecten en activiteiten kunnen het volgende omvatten:

* Taken of problemen die aan de gebruiker zijn toegewezen.
* Projecten van de gebruiker.
* Rapporten die zijn ingesteld voor uitvoering met de toegangsrechten van de gebruiker.
* Templates van de gebruiker.
* Projecten en sjablonen waarop de gebruiker is ingesteld als middelmanager.
* De rij die van het verzoek regels verplettert de beheerder van Workfront of de de vergunningsgebruiker van het Plan is StandaardToegewezen.
* Goedkeuringsprocessen met een werkgebied waarin de gebruiker is opgenomen (met name als dit de enige fiatteur in het werkgebied was).
* Timesheets die de gebruiker als fiatteur vermelden.
* Tijdbladprofielen waarin de gebruiker als fiatteur wordt vermeld.
* Bewijzen van geautomatiseerde workflows die de gebruiker bevatten.

## De gevolgen van de planning van het middel wanneer u een gebruiker voor deactivering plant

Wanneer u een gebruiker voor deactivering plant, verschijnen zij niet meer in de Planner van het Middel zoals beschikbaar voor het opnemen van uren. Als zij deel van de Pools van het Middel blijven, verschijnen zij in de Planner van het Middel, maar hun beschikbaarheid zal aan nul uren die met de datum van hun geplande deactivering beginnen worden geplaatst.

De Planner van het Middel houdt rekening met alle baanrollen van de gebruikers en Geplande Datums van de Voltooiing van de taken en berekent dienovereenkomstig middelen.

Voor meer informatie over de Planner van het Middel, zie [ Overzicht van de Planner van het Middel ](../../../resource-mgmt/resource-planning/get-started-resource-planner.md).

