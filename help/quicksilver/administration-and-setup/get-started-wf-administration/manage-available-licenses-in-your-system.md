---
user-type: administrator
product-area: system-administration;user-management
navigation-topic: start-with-workfront-administration
title: Beschikbare licenties in uw systeem beheren
description: Als Adobe Workfront-beheerder hebt u toegang tot informatie over uw Workfront-account, waaronder het aantal licenties dat voor uw organisatie is aangeschaft en het aantal licenties dat momenteel in gebruik is.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: ea580dd0-efb7-4f56-beb3-07ad044efc8a
source-git-commit: 5ec772260c965b83824ff307bc84755fe06e1ba0
workflow-type: tm+mt
source-wordcount: '1018'
ht-degree: 0%

---

# Beschikbare licenties in uw systeem beheren

Als Adobe Workfront-beheerder hebt u toegang tot informatie over uw Workfront-account, waaronder het aantal licenties dat voor uw organisatie is aangeschaft en het aantal licenties dat momenteel in gebruik is.

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
   <td> <p>U moet een Workfront-beheerder zijn. Zie voor meer informatie <a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Volledige administratieve toegang verlenen aan een gebruiker</a>.</p> <p><b>OPMERKING</b>: Als u nog steeds geen toegang hebt, vraagt u de Workfront-beheerder of deze aanvullende beperkingen op uw toegangsniveau instelt. Voor informatie over hoe een beheerder van Workfront uw toegangsniveau kan wijzigen, zie <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Aangepaste toegangsniveaus maken of wijzigen</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Licenties van uw organisatie bekijken

Het aantal gebruikte licenties dat in gebruik is, wordt automatisch bijgewerkt wanneer u toegangsniveaus toewijst aan gebruikers die u aan Workfront toevoegt. Zie voor meer informatie [Gebruikers toevoegen](../../administration-and-setup/add-users/create-and-manage-users/add-users.md).

U kunt als volgt de licentiegegevens in uw systeem weergeven:

1. Klik op de knop **Hoofdmenu** pictogram ![](assets/main-menu-icon.png) in de rechterbovenhoek van Adobe Workfront klikt u op **Instellen** ![](assets/gear-icon-settings.png).

1. Klik onder aan het linkerdeelvenster op **Systeem** > **Licenties**.

   Voor meer informatie over de licenties die op deze pagina worden vermeld, raadpleegt u [Overzicht van Adobe Workfront-licenties](../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md).

   >[!NOTE]
   >
   >Bewijslicenties zijn alleen beschikbaar voor klanten die de betaalde Workfront Proof Add-on hebben aangeschaft naast hun Workfront-licentie. Voor informatie over deze invoegtoepassing raadpleegt u [Workfront Proof](../../workfront-proof/workfront-proof.md).

1. (Voorwaardelijk) Als u het bericht ziet **Als u een maximum wilt instellen, moet u een thuisgroep toevoegen** voegt u een Home-groep toe aan uw systeem, zoals wordt uitgelegd in de sectie [Een thuisgroep toevoegen aan of verwijderen uit de pagina Licenties](#add-or-remove-a-home-group-to-the-licenses-page) in dit artikel.

## Informatie weergeven over licenties voor Workfront-invoegtoepassingen

In het onderstaande scherm: **5 van 10 Proefvergunningen** geeft aan dat deze organisatie over de betaalde invoegtoepassing Workfront Proof beschikt en momenteel 5 van de 10 door Workfront aangeschafte bewijzen licenties gebruikt.

![](assets/updated-licenses-page.png)

Als uw organisatie Workfront Goals heeft aangeschaft, wordt de licentieinformatie voor dit product ook hier weergegeven. In dit geval kunt u de volgende informatie weergeven:

* Het totale aantal licenties voor Workfront Goals dat uw bedrijf heeft aangeschaft
* Het aantal licenties voor Workfront Goals dat aan gebruikers is gekoppeld. Dit is het aantal gebruikers aan wie minstens de toegang van de Mening tot Doelstellingen in hun toegangsniveau hebben verleend.

Voor informatie over Workfront Goals raadpleegt u [Overzicht van Adobe Workfront-doelen](../../workfront-goals/goal-management/wf-goals-overview.md). Voor informatie over toegang tot Workfront-doelen raadpleegt u [Toegang tot Adobe Workfront-doelen verlenen](../../administration-and-setup/add-users/configure-and-grant-access/grant-access-goals.md)

>[!NOTE]
>
>Met Workfront kunt u meer licenties voor Workfront Goals toewijzen die u hebt aangeschaft. Als u echter meer licenties toewijst dan het Workfront Goals-contract toestaat, neemt een Workfront-accountmanager contact met u op om u te laten weten dat u uw contractnummer hebt overschreden.

<!--
If an organization has other paid add-on products, their license information also displays here. If the organization doesn't have any paid add-on products, nothing displays here. (Drafted this because not sure this is accurate: Scenario Planner is an add-on product and its licenses are not displayed there.)
-->

>[!TIP]
>
>De gebruikers zonder administratieve toegang kunnen een rapport van de Groep gebruiken om vergunningstelling te bekijken. Maak op het tabblad Rapport een nieuw groepsrapport en voeg de volgende kolommen toe:>
>* Limiet licentietype: Arbeidslimiet
>* Limiet licentietype: Plannerlimiet
>
>Ga voor meer informatie over het maken van een rapport naar [Een aangepast rapport maken](../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).

## Een thuisgroep toevoegen aan of verwijderen uit de pagina Licenties {#add-or-remove-a-home-group-to-the-licenses-page}

Een Business of Enterprise Workfront Plan is vereist om deze functie te kunnen gebruiken. Voor meer informatie over de verschillende beschikbare plannen raadpleegt u [Workfront-plannen.](https://www.workfront.com/plans)

Elke gebruiker kan aan slechts ????n Groep van het Huis worden toegewezen. Workfront biedt een aantal licenties voor groepen door te berekenen hoeveel licenties zijn toegewezen en momenteel worden gebruikt in elke Home Group.

Als u het bericht ziet **Als u een maximum wilt instellen, moet u een thuisgroep toevoegen** op de pagina Licenties moet u ten minste ????n startgroep toevoegen aan de pagina Licenties.

>[!IMPORTANT]
>
>* Om vergunningen met huisgroepen effectief te beheren, adviseren wij vestiging specifieke Groepen van het Huis voor bedrijfseenheden alvorens het maximum aantal vergunning bij te werken. Zie voor meer informatie [Overzicht van thuisgroepen](../../administration-and-setup/manage-groups/groups-overview/home-groups.md).
>* U kunt alleen groepen op hoofdniveau toevoegen als thuisgroepen, niet als subgroepen. Als een gebruiker een subgroep heeft die als hun Groep van het Huis wordt toegewezen, wordt hun vergunning toegevoegd aan de vergunningstelling voor de top-level groep boven die subgroep.
>


Een thuisgroep toevoegen aan of verwijderen uit de pagina Licenties:

1. Klik op de knop **Hoofdmenu** pictogram ![](assets/main-menu-icon.png) in de rechterbovenhoek van Adobe Workfront klikt u op **Instellen** ![](assets/gear-icon-settings.png).

1. Klik onder aan het linkerdeelvenster op **Systeem** > **Licenties**.

1. Klikken **Groepenlijst beheren**.
1. Typ de naam van de bovenste groep in het dialoogvenster **Thuisgroepen** doos.
1. Als u de groep wilt toevoegen, klikt u op de naam van de groep wanneer deze wordt weergegeven.

   of

   Als u de groep wilt verwijderen, klikt u op het X-pictogram rechts van de naam.

1. Klikken **Opslaan**.

Als Workfront-beheerder kunt u het maximale aantal licenties voor de Home Group instellen om te voorkomen dat een bedrijfseenheid Workfront-licenties gebruikt die zijn aangeschaft voor andere bedrijfseenheden. Zie voor instructies [Het maximale aantal licenties voor een thuisgroep instellen](#set-the-maximum-license-count-for-a-home-group) in dit artikel.

## Het maximale aantal licenties voor een thuisgroep instellen {#set-the-maximum-license-count-for-a-home-group}

Als beheerder van Workfront, kunt u maximumvergunningstellingen voor de top-level Groepen van het Huis in uw systeem plaatsen. Zo voorkomt u dat een bedrijfseenheid Workfront-licenties gebruikt die zijn aangeschaft voor andere bedrijfseenheden binnen uw organisatie.

Standaard is het maximale aantal licenties ingesteld op N.v.t., wat betekent dat er geen limiet is.

De beheerders van de groep kunnen het aantal vergunningen bekijken die in een Groep van het Huis worden toegewezen en worden gebruikt zij beheren. Zie voor meer informatie [Bekijk het aantal licenties dat is toegewezen en gebruikt in een groep in de nieuwe Adobe Workfront-ervaring](../../administration-and-setup/manage-groups/create-and-manage-groups/view-number-licenses-allocated-used-group.md).

Het maximale aantal licenties voor een thuisgroep instellen:

1. Klik op de knop **Hoofdmenu** pictogram ![](assets/main-menu-icon.png) in de rechterbovenhoek van Adobe Workfront klikt u op **Instellen** ![](assets/gear-icon-settings.png).

1. Klik onder aan het linkerdeelvenster op **Systeem** > **Licenties**.

1. Zoek de thuisgroep in de lijst.
1. In de **Max** Klik op de waarde waarvoor u een maximum wilt instellen.
1. Typ het maximale getal en druk op Enter.

   ![](assets/updated-max.png)

   >[!NOTE]
   >
   >Typ niet 0 als u de maximale licentiewaarde van een groep wilt terugzetten op de standaardwaarde. Verwijder in plaats daarvan het nummer in het vak. Als u de maximale licentiewaarde op 0 instelt, worden er geen licenties toegewezen aan die groep.
