---
user-type: administrator
product-area: system-administration;user-management
navigation-topic: start-with-workfront-administration
title: Beschikbare licenties in uw systeem beheren
description: Als Adobe Workfront-beheerder hebt u toegang tot informatie over uw Workfront-account, waaronder het aantal licenties dat voor uw organisatie is aangeschaft en het aantal licenties dat momenteel in gebruik is.
author: Lisa, Becky
feature: System Setup and Administration
role: Admin
exl-id: ea580dd0-efb7-4f56-beb3-07ad044efc8a
source-git-commit: 15ea03bf586054f7ef421f8cacede6f42835a6e4
workflow-type: tm+mt
source-wordcount: '1178'
ht-degree: 0%

---

# Beschikbare licenties in uw systeem beheren

<!-- Audited: 12/2023 -->

Als Adobe Workfront-beheerder hebt u toegang tot informatie over uw Workfront-account, waaronder het aantal licenties dat voor uw organisatie is aangeschaft en het aantal licenties dat momenteel in gebruik is.

## Toegangsvereisten

+++ Breid uit om de toegangseisen voor de functionaliteit in dit artikel weer te geven.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Workfront-pakket</td> 
   <td><p>Alle</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-licentie</td> 
   <td><p>Standard</p> <p>Plan</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraties op toegangsniveau</td> 
   <td>U moet een Workfront-beheerder zijn. </td> 
  </tr> 
 </tbody> 
</table>

Voor informatie, zie [ vereisten van de Toegang in de documentatie van Workfront ](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).


>[!NOTE]
>
>De volgende verklaringen zijn alleen van toepassing op de nieuwe plannen.
>
>Voor het Uitgezochte plan:
>
>1. Systeembeheerders kunnen geen limieten instellen voor Thuisgroepen.
>2. Systeembeheerders kunnen alleen het totale aantal licenties zien dat wordt gebruikt voor alle Thuisgroepen.
>3. Groepbeheerders hebben helemaal geen toegang tot de pagina Licenties.
>
>Voor de plannen van Prime en Ultimate:
>
>1. Systeembeheerders kunnen Thuisgroepen toevoegen aan de pagina Licenties om het gebruik van licenties in deze groepen weer te geven en kunnen ook licentielimieten instellen.
>2. Groepbeheerders kunnen toegang krijgen tot de pagina Licenties en het gebruik bekijken van licenties in de groepen die ze beheren en die door systeembeheerders zijn toegevoegd aan de pagina Licenties.
>3. Groepbeheerders kunnen geen informatie weergeven voor andere startgroepen of maximum&#39;s toevoegen.

+++

## Licenties van uw organisatie bekijken

Het aantal licenties dat in gebruik is, wordt automatisch bijgewerkt wanneer u toegangsniveaus toewijst aan gebruikers die u aan Workfront toevoegt. Voor meer informatie, zie [ gebruikers ](../../administration-and-setup/add-users/create-and-manage-users/add-users.md) toevoegen.

U kunt als volgt de licentiegegevens in uw systeem weergeven:

{{step-1-to-setup}}

1. Bij de bodem van het linkerpaneel, klik **Systeem** > **Vergunningen**.

   Voor meer informatie over de vergunningen die op deze pagina worden vermeld, zie [ overzicht van Vergunningen ](../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md).

   >[!NOTE]
   >
   >Bewijslicenties zijn alleen beschikbaar voor klanten die de betaalde Workfront Proof-add-on hebben aangeschaft naast hun Workfront-licentie. Voor informatie over dit toe:voegen-op, zie [ Workfront Proof: artikelindex ](../../workfront-proof/workfront-proof.md).

1. (Voorwaardelijk) als u het bericht **ziet om een maximum te plaatsen, moet u een Groep van het Huis** toevoegen, een Groep van het Huis in uw systeem zoals die in de sectie [ wordt verklaard toevoegen of een Groep van het Huis aan de pagina van Vergunningen ](#add-or-remove-a-home-group-to-the-licenses-page) in dit artikel verwijderen.

   >[!NOTE]
   >
   >Voor de nieuwe plannen, staat het Uitgezochte plan beheerders niet toe om vergunningen door de Groep van het Huis te bekijken. U kunt alleen het totale aantal gebruikte licenties zien. De plannen van Prime en Ultimate bieden de mogelijkheid om het maximumaantal licenties per thuisgroep in te stellen.

## Informatie weergeven over licenties voor Workfront-invoegtoepassingen

Als uw organisatie over de betaalde Workfront Proof-invoegtoepassing beschikt, worden het aantal gebruikte licenties en het aantal beschikbare licenties weergegeven. Bijvoorbeeld, **5 van 10 vergunningen van het Bewijs** wijst erop dat de organisatie momenteel 5 van de 10 Workfront Proof vergunningen gebruikt die zij kochten.

![ Vergunning voor Workfront toe:voegen-ons ](assets/updated-licenses-page.png)

Als uw organisatie Workfront Goals heeft aangeschaft, wordt de licentieinformatie voor dit product ook hier weergegeven. In dit geval kunt u de volgende informatie weergeven:

* Het totale aantal licenties voor Workfront Goals dat uw bedrijf heeft aangeschaft
* Het aantal licenties voor Workfront Goals dat aan gebruikers is gekoppeld. Dit is het aantal gebruikers aan wie minstens de toegang van de Mening tot Doelstellingen in hun toegangsniveau hebben verleend.

Voor informatie over de Doelen van Workfront, zie [ overzicht van de Doelen van Adobe Workfront ](../../workfront-goals/goal-management/wf-goals-overview.md). Voor informatie over toegang tot de Doelen van Workfront, zie [ Toegang van de Verlening tot de Doelen van Adobe Workfront ](../../administration-and-setup/add-users/configure-and-grant-access/grant-access-goals.md).

>[!NOTE]
>
>Met Workfront kunt u meer licenties voor Workfront Goals toewijzen die u hebt aangeschaft. Als u echter meer licenties toewijst dan het Workfront Goals-contract toestaat, neemt een Workfront-accountmanager contact met u op om u te laten weten dat u uw contractnummer hebt overschreden.
>

<!--
If an organization has other paid add-on products, their license information also displays here. If the organization doesn't have any paid add-on products, nothing displays here. (Drafted this because not sure this is accurate: Scenario Planner is an add-on product and its licenses are not displayed there.)
-->

>[!TIP]
>
>De gebruikers zonder administratieve toegang kunnen een rapport van de Groep gebruiken om vergunningstelling te bekijken. Maak op het tabblad Rapport een nieuw groepsrapport en voeg de volgende kolommen toe:
>
>* Limiet voor licentietype: limiet voor werknemers
>* Limiet licentietype: limiet planner
>
>Meer leren over het creëren van een rapport, zie [ een douanerapport ](../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md) creëren.

## Informatie weergeven over maandelijkse toegewezen bewijzen en documenten

>[!IMPORTANT]
>
>De limieten voor het bewijs van bevoegdheid en het document gelden alleen voor gebruikers van de nieuwe licenties. Voor meer informatie, zie [ Nieuw vergunningsoverzicht ](/help/quicksilver/administration-and-setup/add-users/how-access-levels-work/licenses-overview.md).

Voor alle niet-betaalde Workfront-licenties geldt een beperking van het aantal bewijzen en documentbeschikkingen. Beperkingen worden elke maand opnieuw ingesteld op basis van afzonderlijke gebruikers.

De beslissingslimieten voor elke licentie verschillen afhankelijk van het abonnement dat u gebruikt. U kunt uw maandelijkse toewijzing bekijken in Opstelling > Vergunningen.

Voor meer informatie over bewijs en documentbeslissingsgrenzen, zie [ Beperkt document en bewijsbesluit voor niet-betaalde gebruikers overzicht ](/help/quicksilver/review-and-approve-work/proof-doc-decision-limits.md).

![ Maandelijkse beslissingstoewijzing ](assets/monthly-decision-allotment.png)

## Een thuisgroep toevoegen aan of verwijderen uit de pagina Licenties {#add-or-remove-a-home-group-to-the-licenses-page}

<!--A Business or Enterprise Workfront Plan is required to use this feature. For more information about the various plans available, see [Workfront Plans.](https://www.workfront.com/plans)-->

Elke gebruiker kan aan slechts één Groep van het Huis worden toegewezen. Workfront biedt een aantal licenties voor groepen door te berekenen hoeveel licenties zijn toegewezen en momenteel worden gebruikt in elke Home Group.

Als u het bericht **ziet om een maximum te plaatsen, moet u een Groep van het Huis** op de pagina van Vergunningen toevoegen, moet u minstens één Groep van het Huis aan de pagina van Vergunningen toevoegen.

>[!IMPORTANT]
>
>* Om vergunningen met huisgroepen effectief te beheren, adviseren wij vestiging specifieke Groepen van het Huis voor bedrijfseenheden alvorens het maximum aantal vergunning bij te werken. Voor meer informatie, zie [ overzicht van de Groepen van het Huis ](../../administration-and-setup/manage-groups/groups-overview/home-groups.md).
>* U kunt alleen groepen op hoofdniveau toevoegen als thuisgroepen, niet als subgroepen. Als een gebruiker een subgroep heeft die als hun Groep van het Huis wordt toegewezen, wordt hun vergunning toegevoegd aan de vergunningstelling voor de top-level groep boven die subgroep.
>

Een thuisgroep toevoegen aan of verwijderen uit de pagina Licenties:

{{step-1-to-setup}}

1. Bij de bodem van het linkerpaneel, klik **Systeem** > **Vergunningen**.

1. Klik **beheren de Lijst van de Groep**.
1. Begin typend de naam van de top-level groep in de **doos van de Groepen van het Huis**.
1. Als u de groep wilt toevoegen, klikt u op de naam van de groep wanneer deze wordt weergegeven.

   of

   Als u de groep wilt verwijderen, klikt u op het X-pictogram rechts van de naam.

1. Klik **sparen**.

Als Workfront-beheerder kunt u het maximale aantal licenties voor de Home Group instellen om te voorkomen dat een bedrijfseenheid Workfront-licenties gebruikt die zijn aangeschaft voor andere bedrijfseenheden. Voor instructies, zie [ de maximumvergunningstelling voor een Groep van het Huis ](#set-the-maximum-license-count-for-a-home-group) in dit artikel plaatsen.

## Het maximale aantal licenties voor een thuisgroep instellen {#set-the-maximum-license-count-for-a-home-group}

Als beheerder van Workfront, kunt u maximumvergunningstellingen voor de top-level Groepen van het Huis in uw systeem plaatsen. Zo voorkomt u dat een bedrijfseenheid Workfront-licenties gebruikt die zijn aangeschaft voor andere bedrijfseenheden binnen uw organisatie.

Standaard is het maximale aantal licenties ingesteld op N.v.t., wat betekent dat er geen limiet is.

De beheerders van de groep kunnen het aantal vergunningen bekijken die in een Groep van het Huis worden toegewezen en worden gebruikt zij beheren. Voor meer informatie, zie [ Mening het aantal vergunningen die in een groep ](../../administration-and-setup/manage-groups/create-and-manage-groups/view-number-licenses-allocated-used-group.md) worden toegewezen en worden gebruikt.

Het maximale aantal licenties voor een thuisgroep instellen:

{{step-1-to-setup}}

1. Bij de bodem van het linkerpaneel, klik **Systeem** > **Vergunningen**.

1. Zoek de thuisgroep in de lijst.
1. In de **Max** kolom van de groep, klik de waarde die u een maximum voor wilt plaatsen.
1. Typ het maximale getal en druk op Enter.

   ![ Maximum vergunningen voor groep ](assets/updated-max.png)

   >[!NOTE]
   >
   >Typ niet 0 als u de maximale licentiewaarde van een groep wilt terugzetten op de standaardwaarde. Verwijder in plaats daarvan het nummer in het vak. Als u de maximale licentiewaarde op 0 instelt, worden er geen licenties toegewezen aan die groep.
