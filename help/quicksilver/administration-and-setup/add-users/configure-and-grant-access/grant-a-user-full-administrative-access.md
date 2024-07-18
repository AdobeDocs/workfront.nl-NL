---
title: Volledige administratieve toegang verlenen aan een gebruiker
description: U kunt gebruikers volledige beheerrechten verlenen voor Workfront.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 46bcb65a-1cb7-443b-88ba-6d0e516e3050
source-git-commit: 5d4434d090c4b6cdefc9c313fecccf6d6e9a510b
workflow-type: tm+mt
source-wordcount: '1583'
ht-degree: 0%

---

# Volledige administratieve toegang verlenen aan een gebruiker

>[!IMPORTANT]
>
>De op deze pagina beschreven procedure is alleen van toepassing op organisaties die nog niet aan de Admin Console zijn geregistreerd. Als uw organisatie is aangemeld bij de Adobe Admin Console, moet u deze handeling uitvoeren via de Adobe Admin Console.
>
>Voor instructies bij het verlenen van volledige beheerdertoegang in Adobe Admin Console, zie [ systeembeheerders in Adobe Admin Console beheren ](../../../administration-and-setup/add-users/create-and-manage-users/admin-console.md).
>
>Voor een lijst van procedures die verschillen gebaseerd op of uw organisatie aan Adobe Admin Console is genegeerd, zie [ Op platform-gebaseerde beleidsverschillen (Adobe Workfront/Adobe Bedrijfs Platform) ](../../../administration-and-setup/get-started-wf-administration/actions-in-admin-console.md).

Als beheerder van Adobe Workfront, kunt u een andere beheerder van Workfront tot stand brengen door hen het de toegangsniveau van de Beheerder van het Systeem toe te wijzen. Een gebruiker met dit toegangsniveau heeft volledige administratieve toegang tot alles in Workfront, met inbegrip van punten zij niet creeerden zelf.

>[!NOTE]
>
>Dit verschilt van het gebruik van een toegangsniveau om gebruikers administratieve toegang tot bepaalde gebieden van het systeem te verlenen. Raadpleeg de volgende secties voor meer informatie:
>
>* [ gebruikers administratieve toegang van de vergunning tot bepaalde gebieden ](../../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md)
>* [ Toegang van een beheerder van Workfront vs. toegang van een gebruiker van het Plan met administratieve rechten ](#access-of-a-workfront-administrator-vs-access-of-a-plan-user-with-administrative-rights) in dit artikel
>

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
   <td> <p>U moet een Workfront-beheerder zijn. Voor meer informatie, zie <a href="#" class="MCXref xref selected"> een gebruiker volledige administratieve toegang verlenen </a>.</p> <p><b> NOTA </b>: Als u nog geen toegang hebt, vraag uw beheerder van Workfront als zij extra beperkingen in uw toegangsniveau plaatsen. Voor informatie over hoe een beheerder van Workfront uw toegangsniveau kan wijzigen, zie <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref"> tot douanetoegangsniveaus </a> leiden of wijzigen.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Volledige toegang van de Beheerder van het Systeem tot één enkele gebruiker verlenen

1. Klik het **Belangrijkste pictogram van het Menu** ![](assets/main-menu-icon.png) in de hoger-juiste hoek van Adobe Workfront, dan klik **Gebruikers** ![](assets/users-icon-in-main-menu.png).

1. Klik op de naam van de gebruiker aan wie u beheerdersrechten wilt verlenen.
1. Klik het Meer menu ![](assets/more-icon.png), dan klik **uitgeven**.

1. Op **geef Persoon** doos uit die verschijnt, klik **Toegang**.

1. In het **toegangsniveau** drop-down lijst, selecteer het **toegangsniveau van de Beheerder van het Systeem**.

   Afhankelijk van de wijzigingen die in uw systeem zijn aangebracht, kan de naam van dit toegangsniveau zijn gewijzigd.

1. Klik **sparen Veranderingen.**

   De gebruiker heeft nu volledige rechten voor systeembeheerders in het systeem.

## Toegang tot een Workfront-beheerder versus toegang tot een Abonnementsgebruiker met beheerrechten  {#access-of-a-workfront-administrator-vs-access-of-a-plan-user-with-administrative-rights}

In de twee onderstaande tabellen ziet u het verschil tussen de toegangsrechten van een gebruiker met een Workfront-beheerdertoegangsniveau en die van een gebruiker met een licentie voor abonnementen met bepaalde beheerrechten.

Workfront-beheerders kunnen alle objecten in het systeem bekijken (ongeacht wie ze heeft gemaakt), nieuwe maken en bestaande objecten wijzigen of verwijderen. Ze hebben volledige toegang tot alle objecten in het systeem.

Gebruikers met een licentie voor abonnementen die functies in één gebied kunnen bewerken, hebben volledige toegang tot de functionaliteit in dat gebied.

>[!NOTE]
>
>De gebruikers met een vergunning van het Plan die als groepsbeheerders worden aangewezen kunnen sommige acties uitvoeren toegestaan voor de beheerders van Workfront. Ze mogen deze handelingen alleen uitvoeren voor de groepen die ze beheren, hun subgroepen en de gebruikers in deze groepen en subgroepen. Voor meer informatie, zie [ de beheerders van de Groep ](../../../administration-and-setup/manage-groups/group-roles/group-administrators.md).

* [Toegang tot het gedeelte Instellen](#access-to-the-setup-area)
* [Toegang tot objecten](#access-to-objects)

### Toegang tot het gedeelte Instellen {#access-to-the-setup-area}

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Gebied/object</th> 
   <th>Workfront-beheerder </th> 
   <th>Gebruiker met een licentie voor abonnementen en enkele beheerrechten</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>Projectvoorkeuren: Projecten</td> 
   <td>Volledige toegang</td> 
   <td>Geen toegang</td> 
  </tr> 
  <tr> 
   <td>Projectvoorkeuren: Taken en problemen</td> 
   <td>Volledige toegang</td> 
   <td>Geen toegang</td> 
  </tr> 
  <tr> 
   <td>Projectvoorkeuren: statussen</td> 
   <td>Volledige toegang</td> 
   <td> <p>Geen toegang</p> </td> 
  </tr> 
  <tr> 
   <td>Projectvoorkeuren: Prioriteiten</td> 
   <td>Volledige toegang</td> 
   <td>Geen toegang</td> 
  </tr> 
  <tr> 
   <td>Projectvoorkeuren: ernst</td> 
   <td>Volledige toegang</td> 
   <td>Geen toegang</td> 
  </tr> 
  <tr> 
   <td>Projectvoorkeuren: Exchange-tarieven</td> 
   <td>Volledige toegang</td> 
   <td>Volledige toegang</td> 
  </tr> 
  <tr> 
   <td>Processen: goedkeuringen</td> 
   <td> <p>Volledige toegang</p> </td> 
   <td>Volledige toegang</td> 
  </tr> 
  <tr> 
   <td>Processen: mijlpaden</td> 
   <td>Volledige toegang</td> 
   <td>Volledige toegang</td> 
  </tr> 
  <tr> 
   <td>Aangepaste Forms</td> 
   <td>Volledige toegang</td> 
   <td> <p>Aangepaste formulieren beheren die ze hebben gemaakt of aangepaste formulieren die met ze worden gedeeld.</p> <p>Aangepaste formulieren die ze hebben gemaakt of aangepaste formulieren die met ze worden gedeeld, koppelen aan objecten die ze beheren of waaraan ze machtigingen kunnen bijdragen.</p> </td> 
  </tr> 
  <tr> 
   <td>Prullenbak: onlangs verwijderd</td> 
   <td>Volledige toegang</td> 
   <td> <p>De gebruikers die groepsbeheerders zijn kunnen projecten herstellen die aan Groepen worden toegewezen zij, en taken, kwesties, of documenten verbonden aan die projecten beheren.</p> </td> 
  </tr> 
  <tr> 
   <td>Prullenbak: onlangs hersteld</td> 
   <td>Volledige toegang</td> 
   <td>Gebruikers die groepsbeheerders zijn, kunnen de items zien die zij onlangs hebben hersteld.</td> 
  </tr> 
  <tr> 
   <td>Taken rollen</td> 
   <td>Volledige toegang</td> 
   <td> <p>Bestaande taakrollen wijzigen maar niet verwijderen.</p> <p>Nieuwe taakrollen toevoegen.</p> </td> 
  </tr> 
  <tr> 
   <td>Teams</td> 
   <td>Volledige toegang</td> 
   <td> <p>Geen toegang om teams te maken.</p> <p>Voeg bestaande teams toe aan gebruikers wanneer u gebruikers maakt of bewerkt.</p> </td> 
  </tr> 
  <tr> 
   <td>Groepen</td> 
   <td>Volledige toegang</td> 
   <td> <p>Geen toegang om groepen te maken.</p> <p>Alleen groepsbeheerders kunnen groepslidmaatschap, subgroepen en status op groepsniveau beheren voor de groepen die zij beheren. </p> </td> 
  </tr> 
  <tr> 
   <td>Bedrijven</td> 
   <td>Volledige toegang</td> 
   <td>Volledige toegang</td> 
  </tr> 
  <tr> 
   <td>Aanmelden als</td> 
   <td>Volledige toegang </td> 
   <td> <p>Als hun groep administratieve toegang op hun toegangsniveau wordt toegelaten en zij als groepsbeheerder worden aangewezen, kunnen zij login als gebruikers in de groep zij en hun subgroepen beheren. Ze kunnen zich niet aanmelden als systeembeheerder.<br> voor meer informatie over het toelaten van groep administratieve toegang voor gebruikers, zie <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md" class="MCXref xref"> de toegang van de Verlening tot gebruikers </a>.</p> </td> 
  </tr> 
  <tr> 
   <td>Planningen</td> 
   <td>Volledige toegang</td> 
   <td> <p>Geen toegang tot schema's bewerken.</p> <p>Toegang om bestaande programma's aan andere gebruikers, op het gebruikersniveau toe te voegen. </p> </td> 
  </tr> 
  <tr> 
   <td>Tijdschema en uren: tijdbladprofielen</td> 
   <td>Volledige toegang</td> 
   <td> <p>Toegang tot het toewijzen van bestaande tijdlijnprofielen aan gebruikers op gebruikersniveau.</p> <p>Gebruikers die groepsbeheerders zijn, kunnen tijdlijnprofielen maken voor de groepen die zij beheren en hun subgroepen. </p> </td> 
  </tr> 
  <tr> 
   <td>Tijdschema en uren: uurtypen</td> 
   <td>Volledige toegang</td> 
   <td> <p>Toegang om de Types van Uur aan gebruikers, op het gebruikersniveau toe te wijzen.</p> </td> 
  </tr> 
  <tr> 
   <td>Tijdschema en uren: voorkeuren</td> 
   <td>Volledige toegang</td> 
   <td>Geen toegang</td> 
  </tr> 
  <tr> 
   <td>E-mail: Meldingen: Gebeurtenismeldingen</td> 
   <td>Alles activeren/deactiveren</td> 
   <td>Geen toegang</td> 
  </tr> 
  <tr> 
   <td>E-mail: Meldingen: Herinneringsmeldingen</td> 
   <td>Volledige toegang</td> 
   <td>Volledige toegang</td> 
  </tr> 
  <tr> 
   <td>E-mail: Meldingen: E-mailsjablonen</td> 
   <td>Volledige toegang</td> 
   <td> <p>Geen toegang om e-mailsjablonen te bewerken.</p> <p>Toegang tot bestaande e-mailsjablonen toevoegen aan herinneringsberichten.</p> </td> 
  </tr> 
  <tr> 
   <td>E-mail: automatische herinneringen</td> 
   <td>Volledige toegang</td> 
   <td>Geen toegang</td> 
  </tr> 
  <tr> 
   <td>E-mail: Uitnodigingen</td> 
   <td>Volledige toegang</td> 
   <td> <p>Geen toegang om e-mailuitnodigingen te bewerken.</p> <p>U kunt e-mailuitnodigingen alleen via het tabblad Personen opnieuw verzenden naar niet-geregistreerde gebruikers.</p> </td> 
  </tr> 
  <tr> 
   <td>E-mail: instellen</td> 
   <td>Volledige toegang</td> 
   <td> <p>Geen toegang</p> </td> 
  </tr> 
  <tr> 
   <td>Scorecards</td> 
   <td>Volledige toegang</td> 
   <td> <p>Volledige toegang</p> </td> 
  </tr> 
  <tr> 
   <td>Typen kosten</td> 
   <td>Volledige toegang</td> 
   <td> <p>Geen toegang</p> </td> 
  </tr> 
  <tr> 
   <td>Risicotypes</td> 
   <td>Volledige toegang</td> 
   <td>Geen toegang</td> 
  </tr> 
  <tr> 
   <td>Toegangsniveaus</td> 
   <td> <p>Volledige toegang om alle toegangsniveaus te wijzigen.</p> <p>De toegangsniveaus van de Beheerder van het Systeem en van de Externe Gebruiker kunnen, door gebrek niet worden gewijzigd.</p> </td> 
   <td> <p>Geen toegang tot toegangsniveaus bewerken.</p> <p>Wijs een toegangsniveau aan andere gebruikers toe dat lager of gelijk aan hun op het gebruikersniveau is.</p> </td> 
  </tr> 
  <tr> 
   <td>Interface: lay-outsjablonen</td> 
   <td>Volledige toegang</td> 
   <td> <p>Toegang tot het toewijzen van bestaande lay-outsjablonen aan andere gebruikers op gebruikersniveau. </p> <p>Gebruikers die zijn aangewezen als groepsbeheerders, kunnen lay-outsjablonen maken voor groepen en subgroepen die zij beheren.</p> </td> 
  </tr> 
  <tr> 
   <td>Interface: feeds bijwerken</td> 
   <td>Volledige toegang</td> 
   <td> <p>Geen toegang om Update Feeds te wijzigen.</p> <p>Toegang tot velden die u wilt bijhouden in de Update Feeds wanneer u Aangepaste Forms bewerkt.</p> </td> 
  </tr> 
  <tr> 
   <td>Interface: filters</td> 
   <td>Volledige toegang</td> 
   <td> <p>Geen toegang om Filters in het gebied van de Opstelling tot stand te brengen.</p> <p>Toegang tot het maken van nieuwe filters in een lijst met objecten.</p> </td> 
  </tr> 
  <tr> 
   <td>Interface: weergaven</td> 
   <td>Volledige toegang</td> 
   <td> <p>Geen toegang tot het maken van weergaven in het gedeelte Setup.</p> <p>Toegang tot het maken van nieuwe weergaven in een lijst met objecten.</p> </td> 
  </tr> 
  <tr> 
   <td>Interface: Groupings</td> 
   <td>Volledige toegang</td> 
   <td> <p>Geen toegang om Groepen in het gebied van de Opstelling tot stand te brengen.</p> <p>Toegang tot het maken van nieuwe groepen in een lijst met objecten.</p> </td> 
  </tr> 
  <tr> 
   <td>Interface: lijstbesturingselementen</td> 
   <td>Volledige toegang</td> 
   <td> <p>Geen toegang</p> </td> 
  </tr> 
  <tr> 
   <td>Documenten: cloudproviders</td> 
   <td>Volledige toegang</td> 
   <td> <p>Geen toegang om cloudproviders te configureren.</p> <p>Toegang tot documenten van en naar cloudproviders via het tabblad Documenten nadat de cloudproviders zijn geïntegreerd met Workfront.</p> </td> 
  </tr> 
  <tr> 
   <td>Documenten: metagegevenstoewijzing</td> 
   <td>Volledige toegang</td> 
   <td>Geen toegang</td> 
  </tr> 
  <tr> 
   <td>Documenten: SharePoint-integratie</td> 
   <td>Volledige toegang</td> 
   <td> <p>Geen toegang om een integratie van SharePoint te vormen.</p> <p>Toegang tot koppelingsdocumenten van en naar SharePoint vanaf het tabblad Documenten, nadat de integratie van SharePoint met Workfront is geconfigureerd.</p> </td> 
  </tr> 
  <tr> 
   <td>Documenten: aangepaste integratie</td> 
   <td>Volledige toegang</td> 
   <td> <p>Geen toegang om een Integratie van de Douane te vormen.</p> <p>Toegang tot koppelingsdocumenten van en naar externe providers vanaf het tabblad Documenten, nadat de externe providers zijn geïntegreerd met Workfront.</p> </td> 
  </tr> 
  <tr> 
   <td>Systeem: merken</td> 
   <td>Volledige toegang</td> 
   <td>Geen toegang</td> 
  </tr> 
  <tr> 
   <td>Systeem: klantgegevens</td> 
   <td>Volledige toegang</td> 
   <td>Geen toegang</td> 
  </tr> 
  <tr> 
   <td>Systeem: Single Sign-On (SSO)</td> 
   <td>Volledige toegang</td> 
   <td>Geen toegang</td> 
  </tr> 
  <tr> 
   <td>Systeem: Gebruikers voor SSO bijwerken</td> 
   <td>Volledige toegang</td> 
   <td>Geen toegang</td> 
  </tr> 
  <tr> 
   <td>Systeem: Kick-start</td> 
   <td>Volledige toegang</td> 
   <td>Geen toegang</td> 
  </tr> 
  <tr> 
   <td>Systeem: diagnostiek</td> 
   <td>Volledige toegang</td> 
   <td>Geen toegang</td> 
  </tr> 
  <tr> 
   <td>Systeem: voorkeuren</td> 
   <td>Volledige toegang</td> 
   <td>Geen toegang</td> 
  </tr> 
 </tbody> 
</table>

### Toegang tot objecten {#access-to-objects}

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Gebied/object</th> 
   <th>Workfront-beheerder </th> 
   <th>Gebruiker met een licentie voor abonnementen en enkele beheerrechten</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>Kalenders</td> 
   <td>Volledige toegang</td> 
   <td>De kalenders beheren die ze maken en de kalenders die met hen worden gedeeld.</td> 
  </tr> 
  <tr> 
   <td>Dashboards</td> 
   <td>Volledige toegang</td> 
   <td>De dashboards beheren die zij creëren en dashboards delen met hen.</td> 
  </tr> 
  <tr> 
   <td>Documenten</td> 
   <td>Volledige toegang</td> 
   <td>Documenten die ze uploaden of documenten die met hen worden gedeeld, beheren.</td> 
  </tr> 
  <tr> 
   <td>Problemen</td> 
   <td>Volledige toegang</td> 
   <td>De problemen beheren die ze maken of problemen die met hen worden gedeeld.</td> 
  </tr> 
  <tr> 
   <td>Portfolio's</td> 
   <td>Volledige toegang</td> 
   <td>Portfolio's beheren die zij maken of portfolio's die met hen worden gedeeld. </td> 
  </tr> 
  <tr> 
   <td>Programma's</td> 
   <td>Volledige toegang</td> 
   <td>Beheer programma's die ze maken of programma's die met hen worden gedeeld.</td> 
  </tr> 
  <tr> 
   <td>Project</td> 
   <td>Volledige toegang</td> 
   <td>Projecten beheren die zij maken of projecten die met hen worden gedeeld.</td> 
  </tr> 
  <tr> 
   <td>Rapporten</td> 
   <td>Volledige toegang</td> 
   <td>De rapporten beheren die zij maken of die met hen worden gedeeld. Systeemrapporten weergeven, kopiëren en bewerken.</td> 
  </tr> 
  <tr> 
   <td>Taken</td> 
   <td>Volledige toegang</td> 
   <td>Taken beheren die zij maken of taken die met de</td> 
  </tr> 
  <tr> 
   <td>Sjablonen</td> 
   <td>Volledige toegang</td> 
   <td>Sjablonen beheren die ze maken of die met hen worden gedeeld</td> 
  </tr> 
  <tr> 
   <td>Timesheets</td> 
   <td>Volledige toegang</td> 
   <td>Volledige toegang</td> 
  </tr> 
  <tr> 
   <td>Gebruikers</td> 
   <td>Volledige toegang</td> 
   <td> <p>Beperkte toegang</p> <p>Zij kunnen geen groepen aan gebruikers toewijzen waarvoor zij geen groepsbeheerder of groepen zijn die niet openbaar zijn.</p> <p>Zij kunnen geen toegangsniveau aan gebruikers toewijzen die dan hun eigen toegangsniveau hoger is.</p> <p>Als hun groep administratieve toegang op hun toegangsniveau wordt toegelaten en zij als groepsbeheerder op een groep worden aangewezen, kunnen zij het wachtwoord van terugstellen en login als gebruikers in de groep zij en hun subgroepen beheren. Ze kunnen het wachtwoord van of het aanmelden als systeembeheerder niet opnieuw instellen.<br> voor meer informatie over het toelaten van groep administratieve toegang voor gebruikers, zie <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md" class="MCXref xref"> de toegang van de Verlening tot gebruikers </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>
