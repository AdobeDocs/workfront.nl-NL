---
title: Volledige administratieve toegang verlenen aan een gebruiker
description: U kunt gebruikers volledige beheerrechten verlenen voor Workfront.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 46bcb65a-1cb7-443b-88ba-6d0e516e3050
source-git-commit: 253a116e04e0b3a729331f5d0a29405e82808390
workflow-type: tm+mt
source-wordcount: '1614'
ht-degree: 0%

---

# Volledige administratieve toegang verlenen aan een gebruiker

>[!IMPORTANT]
>
>De op deze pagina beschreven procedure is alleen van toepassing op organisaties die nog niet aan boord van de Admin Console zijn gegaan. Als uw organisatie is aangemeld bij de Adobe Admin Console, moet u deze handeling uitvoeren via de Adobe Admin Console.
>
>Voor instructies over het verlenen van volledige beheerdertoegang in de Adobe Admin Console:
>
>* Zie [Systeembeheerders in Workfront maken met de Adobe Admin Console](../../../administration-and-setup/add-users/create-and-manage-users/admin-console.md#create2)
>* Zie de sectie &quot;Gebruikersdetails bewerken&quot; in het artikel [Gebruikers individueel beheren](https://helpx.adobe.com/enterprise/using/manage-users-individually.html) in de documentatie van Adobe Admin Console.
>* Neem contact op met uw Adobe Admin Console-beheerder.
>
>Voor een lijst met procedures die verschillen afhankelijk van de vraag of uw organisatie al dan niet is aangemeld bij de Adobe Admin Console, raadpleegt u [Op Platform gebaseerde verschillen in beheer (Adobe Workfront/Adobe Business Platform)](../../../administration-and-setup/get-started-wf-administration/actions-in-admin-console.md).

Als beheerder van Adobe Workfront, kunt u een andere beheerder van Workfront tot stand brengen door hen het de toegangsniveau van de Beheerder van het Systeem toe te wijzen. Een gebruiker met dit toegangsniveau heeft volledige administratieve toegang tot alles in Workfront, met inbegrip van punten zij niet creeerden zelf.

>[!NOTE]
>
>Dit verschilt van het gebruik van een toegangsniveau om gebruikers administratieve toegang tot bepaalde gebieden van het systeem te verlenen. Raadpleeg de volgende secties voor meer informatie:
>
>* [Gebruikers administratieve toegang verlenen tot bepaalde gebieden](../../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md)
>* [Toegang tot een Workfront-beheerder versus toegang tot een Abonnementsgebruiker met beheerrechten](#access-of-a-workfront-administrator-vs-access-of-a-plan-user-with-administrative-rights) in dit artikel
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
   <td> <p>U moet een Workfront-beheerder zijn. Zie voor meer informatie <a href="#" class="MCXref xref selected">Volledige administratieve toegang verlenen aan een gebruiker</a>.</p> <p><b>OPMERKING</b>: Als u nog steeds geen toegang hebt, vraagt u de Workfront-beheerder of deze aanvullende beperkingen op uw toegangsniveau instelt. Voor informatie over hoe een beheerder van Workfront uw toegangsniveau kan wijzigen, zie <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Aangepaste toegangsniveaus maken of wijzigen</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Volledige toegang van de Beheerder van het Systeem tot ????n enkele gebruiker verlenen

1. Klik op de knop **Hoofdmenu** pictogram ![](assets/main-menu-icon.png) in de rechterbovenhoek van Adobe Workfront klikt u op **Gebruikers** ![](assets/users-icon-in-main-menu.png).

1. Klik op de naam van de gebruiker aan wie u beheerdersrechten wilt verlenen.
1. Klik op het menu Meer ![](assets/more-icon.png)en klik vervolgens op **Bewerken**.

1. Op de **Persoon bewerken** vak dat wordt weergegeven, klikt u op **Toegang**.

1. In de **toegangsniveau** vervolgkeuzelijst selecteert u de **Systeembeheerder** toegangsniveau.

   Afhankelijk van de wijzigingen die in uw systeem zijn aangebracht, kan de naam van dit toegangsniveau zijn gewijzigd.

1. Klikken **Wijzigingen opslaan.**

   De gebruiker heeft nu de volledige rechten van de Beheerder van het Systeem in het systeem.

## Toegang tot een Workfront-beheerder versus toegang tot een Abonnementsgebruiker met beheerrechten  {#access-of-a-workfront-administrator-vs-access-of-a-plan-user-with-administrative-rights}

In de twee onderstaande tabellen ziet u het verschil tussen de toegangsrechten van een gebruiker met een Workfront-beheerdertoegangsniveau en die van een gebruiker met een licentie voor abonnementen met bepaalde beheerrechten.

Workfront-beheerders kunnen alle objecten in het systeem bekijken (ongeacht wie ze heeft gemaakt), nieuwe maken en bestaande objecten wijzigen of verwijderen. Ze hebben volledige toegang tot alle objecten in het systeem.

Gebruikers met een licentie voor abonnementen die functies in ????n gebied kunnen bewerken, hebben volledige toegang tot de functionaliteit in dat gebied.

>[!NOTE]
>
>De gebruikers met een vergunning van het Plan die als groepsbeheerders worden aangewezen kunnen sommige acties uitvoeren toegestaan voor de beheerders van Workfront. Ze mogen deze handelingen alleen uitvoeren voor de groepen die ze beheren, hun subgroepen en de gebruikers in deze groepen en subgroepen. Zie voor meer informatie [Groepbeheerders](../../../administration-and-setup/manage-groups/group-roles/group-administrators.md).

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
   <td>Projectvoorkeuren: Statussen</td> 
   <td>Volledige toegang</td> 
   <td> <p>Geen toegang</p> </td> 
  </tr> 
  <tr> 
   <td>Projectvoorkeuren: Prioriteiten</td> 
   <td>Volledige toegang</td> 
   <td>Geen toegang</td> 
  </tr> 
  <tr> 
   <td>Projectvoorkeuren: Ernst</td> 
   <td>Volledige toegang</td> 
   <td>Geen toegang</td> 
  </tr> 
  <tr> 
   <td>Projectvoorkeuren: Wisselkoersen</td> 
   <td>Volledige toegang</td> 
   <td>Volledige toegang</td> 
  </tr> 
  <tr> 
   <td>Processen: Goedkeuringen</td> 
   <td> <p>Volledige toegang</p> </td> 
   <td>Volledige toegang</td> 
  </tr> 
  <tr> 
   <td>Processen: Mijlpaden</td> 
   <td>Volledige toegang</td> 
   <td>Volledige toegang</td> 
  </tr> 
  <tr> 
   <td>Aangepaste Forms</td> 
   <td>Volledige toegang</td> 
   <td> <p>Aangepaste formulieren beheren die ze hebben gemaakt of aangepaste formulieren die met ze worden gedeeld.</p> <p>Aangepaste formulieren die ze hebben gemaakt of aangepaste formulieren die met ze worden gedeeld, koppelen aan objecten die ze beheren of waaraan ze machtigingen kunnen bijdragen.</p> </td> 
  </tr> 
  <tr> 
   <td>Prullenbak: Onlangs verwijderd</td> 
   <td>Volledige toegang</td> 
   <td> <p>De gebruikers die groepsbeheerders zijn kunnen projecten herstellen die aan Groepen worden toegewezen zij, en taken, kwesties, of documenten verbonden aan die projecten beheren.</p> </td> 
  </tr> 
  <tr> 
   <td>Prullenbak: Onlangs hersteld</td> 
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
   <td> <p>Als hun groep administratieve toegang op hun toegangsniveau wordt toegelaten en zij als groepsbeheerder worden aangewezen, kunnen zij login als gebruikers in de groep zij en hun subgroepen beheren. Ze kunnen zich niet aanmelden als systeembeheerder.<br>Voor meer informatie over het toelaten van groep administratieve toegang voor gebruikers, zie <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md" class="MCXref xref">Toegang verlenen aan gebruikers</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>Planningen</td> 
   <td>Volledige toegang</td> 
   <td> <p>Geen toegang tot schema's bewerken.</p> <p>Toegang om bestaande programma's aan andere gebruikers, op het gebruikersniveau toe te voegen. </p> </td> 
  </tr> 
  <tr> 
   <td>Tijdschema en uren: Tijdbladprofielen</td> 
   <td>Volledige toegang</td> 
   <td> <p>Toegang tot het toewijzen van bestaande tijdlijnprofielen aan gebruikers op gebruikersniveau.</p> <p>Gebruikers die groepsbeheerders zijn, kunnen tijdlijnprofielen maken voor de groepen die zij beheren en hun subgroepen. </p> </td> 
  </tr> 
  <tr> 
   <td>Tijdschema en uren: Uurtypen</td> 
   <td>Volledige toegang</td> 
   <td> <p>Toegang om de Types van Uur aan gebruikers, op het gebruikersniveau toe te wijzen.</p> </td> 
  </tr> 
  <tr> 
   <td>Tijdschema en uren: Voorkeuren</td> 
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
   <td>E-mail: Automatische herinneringen</td> 
   <td>Volledige toegang</td> 
   <td>Geen toegang</td> 
  </tr> 
  <tr> 
   <td>E-mail: Uitnodigingen</td> 
   <td>Volledige toegang</td> 
   <td> <p>Geen toegang om e-mailuitnodigingen te bewerken.</p> <p>U kunt e-mailuitnodigingen alleen via het tabblad Personen opnieuw verzenden naar niet-geregistreerde gebruikers.</p> </td> 
  </tr> 
  <tr> 
   <td>E-mail: Instellen</td> 
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
   <td>Interface: Lay-outsjablonen</td> 
   <td>Volledige toegang</td> 
   <td> <p>Toegang tot het toewijzen van bestaande lay-outsjablonen aan andere gebruikers op gebruikersniveau. </p> <p>Gebruikers die zijn aangewezen als groepsbeheerders, kunnen lay-outsjablonen maken voor groepen en subgroepen die zij beheren.</p> </td> 
  </tr> 
  <tr> 
   <td>Interface: Feeds bijwerken</td> 
   <td>Volledige toegang</td> 
   <td> <p>Geen toegang om Update Feeds te wijzigen.</p> <p>Toegang tot velden die u wilt bijhouden in de Update Feeds wanneer u Aangepaste Forms bewerkt.</p> </td> 
  </tr> 
  <tr> 
   <td>Interface: Filters</td> 
   <td>Volledige toegang</td> 
   <td> <p>Geen toegang om Filters in het gebied van de Opstelling tot stand te brengen.</p> <p>Toegang tot het maken van nieuwe filters in een lijst met objecten.</p> </td> 
  </tr> 
  <tr> 
   <td>Interface: Weergaven</td> 
   <td>Volledige toegang</td> 
   <td> <p>Geen toegang tot het maken van weergaven in het gedeelte Setup.</p> <p>Toegang tot het maken van nieuwe weergaven in een lijst met objecten.</p> </td> 
  </tr> 
  <tr> 
   <td>Interface: Groepen</td> 
   <td>Volledige toegang</td> 
   <td> <p>Geen toegang om Groepen in het gebied van de Opstelling tot stand te brengen.</p> <p>Toegang tot het maken van nieuwe groepen in een lijst met objecten.</p> </td> 
  </tr> 
  <tr> 
   <td>Interface: Besturingselementen lijst</td> 
   <td>Volledige toegang</td> 
   <td> <p>Geen toegang</p> </td> 
  </tr> 
  <tr> 
   <td>Documenten: Cloud Providers</td> 
   <td>Volledige toegang</td> 
   <td> <p>Geen toegang om cloudproviders te configureren.</p> <p>Toegang tot documenten van en naar cloudproviders via het tabblad Documenten nadat de cloudproviders zijn ge??ntegreerd met Workfront.</p> </td> 
  </tr> 
  <tr> 
   <td>Documenten: Metagegevenstoewijzing</td> 
   <td>Volledige toegang</td> 
   <td>Geen toegang</td> 
  </tr> 
  <tr> 
   <td>Documenten: SharePoint-integratie</td> 
   <td>Volledige toegang</td> 
   <td> <p>Geen toegang om een integratie van SharePoint te vormen.</p> <p>Toegang tot koppelingsdocumenten van en naar SharePoint vanaf het tabblad Documenten, nadat de integratie van SharePoint met Workfront is geconfigureerd.</p> </td> 
  </tr> 
  <tr> 
   <td>Documenten: Aangepaste integratie</td> 
   <td>Volledige toegang</td> 
   <td> <p>Geen toegang om een Integratie van de Douane te vormen.</p> <p>Toegang tot koppelingsdocumenten van en naar externe providers vanaf het tabblad Documenten, nadat de externe providers zijn ge??ntegreerd met Workfront.</p> </td> 
  </tr> 
  <tr> 
   <td>Systeem: Branding</td> 
   <td>Volledige toegang</td> 
   <td>Geen toegang</td> 
  </tr> 
  <tr> 
   <td>Systeem: Klantgegevens</td> 
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
   <td>Systeem: Diagnostiek</td> 
   <td>Volledige toegang</td> 
   <td>Geen toegang</td> 
  </tr> 
  <tr> 
   <td>Systeem: Voorkeuren</td> 
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
   <td>De kalenders beheren die ze maken en kalenders die met hen worden gedeeld.</td> 
  </tr> 
  <tr> 
   <td>Dashboards</td> 
   <td>Volledige toegang</td> 
   <td>De dashboards beheren die zij cre??ren en dashboards delen met hen.</td> 
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
   <td>Portfolio</td> 
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
   <td>De rapporten beheren die zij maken of die met hen worden gedeeld. Systeemrapporten weergeven, kopi??ren en bewerken.</td> 
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
   <td> <p>Beperkte toegang</p> <p>Zij kunnen geen groepen aan gebruikers toewijzen waarvoor zij geen groepsbeheerder of groepen zijn die niet openbaar zijn.</p> <p>Zij kunnen geen toegangsniveau aan gebruikers toewijzen die dan hun eigen toegangsniveau hoger is.</p> <p>Als hun groep administratieve toegang op hun toegangsniveau wordt toegelaten en zij als groepsbeheerder op een groep worden aangewezen, kunnen zij het wachtwoord van terugstellen en login als gebruikers in de groep zij en hun subgroepen beheren. Ze kunnen het wachtwoord van of aanmelden als systeembeheerder niet opnieuw instellen.<br>Voor meer informatie over het toelaten van groep administratieve toegang voor gebruikers, zie <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md" class="MCXref xref">Toegang verlenen aan gebruikers</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>
