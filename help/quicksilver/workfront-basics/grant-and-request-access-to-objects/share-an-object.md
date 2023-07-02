---
product-area: projects
navigation-topic: grant-and-request-access-to-objects
title: Een object delen
description: Uw Adobe Workfront-beheerder verleent gebruikers toegang tot weergave- of bewerkingsobjecten wanneer zij toegangsniveaus toewijzen. Zie Aangepaste toegangsniveaus maken of wijzigen voor meer informatie over het verlenen van toegang tot objecten.
author: Alina
feature: Get Started with Workfront
exl-id: 27a1beb9-e83a-4ef6-bf5f-ad52575a993c
source-git-commit: 5b4aa5c806d0f930250e9238d460833cd1aed71a
workflow-type: tm+mt
source-wordcount: '1185'
ht-degree: 0%

---

# Een object delen

Uw Adobe Workfront-beheerder verleent gebruikers toegang tot weergave- of bewerkingsobjecten wanneer zij toegangsniveaus toewijzen. Ga voor meer informatie over het verlenen van toegang tot objecten naar [Aangepaste toegangsniveaus maken of wijzigen](../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).

Samen met het toegangsniveau dat de gebruikers worden verleend, kunt u hen toestemmingen ook verlenen om specifieke voorwerpen te bekijken of uit te geven die u creeerde of toegang om hebt te delen. Voor meer informatie over toegangsniveaus en toestemmingen, zie [Hoe de toegangsniveaus en de toestemmingen samenwerken](../../administration-and-setup/add-users/access-levels-and-object-permissions/how-access-levels-permissions-work-together.md).

Machtigingen gelden specifiek voor één item in Workfront en definiëren welke handelingen u op dat item kunt uitvoeren.

Voor informatie over het delen van machtigingen voor objecten raadpleegt u [Overzicht van het delen van machtigingen voor objecten](../../workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md).

>[!NOTE]
>
>Een Workfront-beheerder kan machtigingen toevoegen of verwijderen voor alle items in het systeem, zonder de eigenaar van die items te zijn.

In dit artikel wordt beschreven hoe u de volgende objecten kunt delen: 

* Projecten, taken, problemen
* Portfolio, programma&#39;s
* Documenten

Zie ook de volgende artikelen voor informatie over het delen van alle andere objecten in Workfront:

* Zie voor sjablonen [Projectsjablonen delen](../../manage-work/projects/create-and-manage-templates/share-project-template.md).
* Voor proefdrukken raadpleegt u [Een proefexemplaar delen in Workfront-proefdrukken](../../workfront-proof/wp-work-proofsfiles/share-proofs-and-files/share-proof.md).
* Raadpleeg de volgende artikelen voor rapporten, dashboards en kalenders:

   * [Een rapport delen in Adobe Workfront](../../reports-and-dashboards/reports/creating-and-managing-reports/share-report.md)
   * [Een dashboard delen](../../reports-and-dashboards/dashboards/creating-and-managing-dashboards/share-dashboard.md)
   * [Een kalenderrapport delen](../../reports-and-dashboards/reports/calendars/share-a-calendar-report.md)

  Zie ook [Rapporten, dashboards en kalenders delen](../../workfront-basics/grant-and-request-access-to-objects/permissions-reports-dashboards-calendars.md) voor algemene informatie over het delen van rapporten, dashboards, en kalenders. 

* Zie voor filters, weergaven en groepen [Een filter, weergave of groep delen](../../reports-and-dashboards/reports/reporting-elements/share-filter-view-grouping.md).
* Zie voor documentmappen [Een documentmap delen](../../workfront-basics/grant-and-request-access-to-objects/share-a-document-folder.md).
* Zie voor plannen [Een abonnement delen in de Scenario-planner](../../scenario-planner/share-a-plan.md).

  Hiervoor is een aanvullende licentie vereist.

* Voor doelstellingen raadpleegt u [Een doel delen in Workfront-doelen](../../workfront-goals/workfront-goals-settings/share-a-goal.md). Hiervoor is een aanvullende licentie vereist.

## Toegangsvereisten

<!--drafted for P&P:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan*</td> 
   <td> <p>Any </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license*</td> 
   <td> <p>Current license: Standard</p> 
   Or
   <p>Legacy license: Work or higher</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>View access or higher to the objects you want to share</p> <p><b>NOTE</b>
   
   If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can modify your access level, see <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>View permissions or higher to the objects you want to share</p> <p>For information on requesting additional access, see <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>
-->

U moet het volgende hebben om objecten te delen:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-abonnement*</td> 
   <td> <p>Alle </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-licentie*</td> 
   <td> <p>Werk of hoger</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraties op toegangsniveau*</td> 
   <td> <p>Toegang tot of hoger weergeven voor de objecten die u wilt delen</p> <p><b>OPMERKING</b>

Als u nog steeds geen toegang hebt, vraagt u de Workfront-beheerder of deze aanvullende beperkingen op uw toegangsniveau instelt. Voor informatie over hoe een beheerder van Workfront uw toegangsniveau kan wijzigen, zie <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Aangepaste toegangsniveaus maken of wijzigen</a>.</p> </td>
</tr> 
  <tr> 
   <td role="rowheader">Objectmachtigingen</td> 
   <td> <p>Machtigingen of hoger weergeven voor de objecten die u wilt delen</p> <p>Voor informatie over het aanvragen van aanvullende toegang raadpleegt u <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Toegang tot objecten aanvragen </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Neem contact op met uw Workfront-beheerder om te weten te komen welk plan, licentietype of toegang u hebt.

## Eén object delen {#share-a-single-object}

1. Ga naar het object dat u wilt delen.

   Voor informatie over welke objecten kunnen worden gedeeld, raadpleegt u [Overzicht van het delen van machtigingen voor objecten](../../workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md).
1. Voor projecten, taken en kwesties:

   Klik op de knop **Delen** naast de objectnaam.

   ![](assets/new-share-button.png)

   OF

   Voor documenten, portfolio&#39;s en programma&#39;s:

   Klik op de knop **Meer** pictogram ![](assets/more-icon.png)naast de objectnaam klikt u op **Delen** of **Delen.**

   ![](assets/share-a-document-350x160.png)

1. In de **Geef `<Object Name>` toegang tot** typt u de naam van de gebruiker, het team, de rol, de groep of het bedrijf met wie u het object wilt delen. Klik vervolgens op de naam wanneer deze wordt weergegeven in de vervolgkeuzelijst.

   Als u bijvoorbeeld een project deelt, gebruikt u de opdracht **Projecttoegang verlenen aan** veld.

   >[!TIP]
   >
   >U kunt een object alleen delen met actieve gebruikers, teams, rollen of bedrijven.

   ![](assets/nwe-project-sharing-modal-350x456.png)

   >[!TIP]
   >
   >Als u meerdere entiteiten een soortgelijke naam hebt gegeven, worden deze allemaal vermeld onder hun type. De namen van de entiteiten worden in alfabetische volgorde weergegeven. De volgorde waarin de entiteitstypen worden weergegeven, is echter willekeurig.
   >
   >
   >![](assets/sharing-entities-named-similarly-in-sharing-box-350x179.png)   >
   >

1. (Optioneel) Herhaal stap 3 voor elke gebruiker, elk team, elke rol of elke groep aan wie u toegang tot het object wilt verlenen.

   <!--
   <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
   (NOTE: esnure this stays accurate; in the editor it looks like step 4 but one step is conditioned entirely for one version or another)
   </MadCap:conditionalText>
   -->

1. Specificeer de toestemmingen voor elke gebruiker, het team, de rol, de groep, of het bedrijf die u in Stap 3 toevoegde door het drop-down menu te klikken, dan het toestemmingsniveau te selecteren dat u wilt verlenen.

   De volgende opties zijn beschikbaar:

   * **Weergave:** Gebruikers kunnen het item bekijken en delen. 
   * **Contribute****:** Gebruikers kunnen updates uitvoeren, gegevens registreren, kleine bewerkingen uitvoeren en delen, plus alle weergavemachtigingen.

     >[!TIP]
     >
     >U kunt Contribute-machtigingen alleen verlenen voor de volgende objecten: 
     >
     >   
     >   
     * Projecten
     * Taken
     * Problemen
     >   
     >

   * **Beheren:**Gebruikers hebben volledige toegang tot het object zonder beheerrechten, die op toegangsniveau worden verleend, plus alle weergave- en Contribute-machtigingen.

     >[!NOTE]
     >
     > De Workfront-beheerder of de maker van het object kan machtigingen van deze entiteiten verwijderen.

      

     ![](assets/screen-shot-2013-12-04-at-1.13.11-pm.png)

1. (Optioneel) Klik op **Geavanceerde opties** specifieke machtigingen voor het object configureren.

   Afhankelijk van het geselecteerde object zijn er verschillende geavanceerde opties voor weergave, beheer en Contribute.\
   Voor meer informatie over de toestemmingsniveaus, zie [Overzicht van het delen van machtigingen voor objecten](../../workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md).

   ![](assets/screen-shot-2013-12-04-at-1.14.11-pm.png)

1. (Optioneel) Als u dit object beschikbaar wilt maken voor alle gebruikers in het systeem, klikt u op de knop **Tandwiel** pictogram ![](assets/gear-icon-settings-with-dn-arrow.jpg) klikt u vervolgens in de vervolgkeuzelijst op **Dit voor het hele systeem zichtbaar maken**.

   Alle gebruikers kunnen het object zien op basis van de machtigingen die u instelt.

1. (Optioneel en voorwaardelijk) Klik tijdens het delen van een project op de knop **Tandwiel** pictogram ![](assets/gear-icon-settings-with-dn-arrow.jpg)klikt u vervolgens in de vervolgkeuzelijst op **Instellen als sjabloon voor mijn projecttoegang** om de machtigingen als een sjabloon in te stellen.\
   Nadat u toestemmingen op één project hebt bepaald, worden deze zelfde toestemmingen automatisch toegepast de volgende tijd u een project van kras creeert.

   >[!NOTE]
   >
   Het malplaatje van de projecttoegang treedt de het delen gebreken met voeten die aan u door de beheerder van Workfront in uw Niveau van de Toegang worden verleend.\
   Voor meer informatie over het specificeren van het delen gebreken voor projecten in het Niveau van de Toegang, zie [Toegang verlenen tot projecten](../../administration-and-setup/add-users/configure-and-grant-access/grant-access-projects.md) . >
   >
   <!--   >
   ><MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">   >
   >(NOTE: (this note also appears in Understanding Project Permissions.))   >
   ></MadCap:conditionalText>   >
   >-->   >
   >

   U kunt toestemmingen op de projecten specificeren die van een malplaatje zullen worden gecreeerd wanneer u het malplaatje deelt. Zie voor meer informatie [Projectsjablonen delen](../../manage-work/projects/create-and-manage-templates/share-project-template.md).

1. (Optioneel) Als u het object openbaar wilt maken, klikt u op **Dit openbaar maken voor externe gebruikers**.

   >[!TIP]
   >
   Deze optie is niet beschikbaar voor alle objecten.

   ![](assets/make-public-system-wide-settings-sharing-box-on-document-nwe-350x481.png)

1. (Voorwaardelijk) Als u het object openbaar hebt gemaakt voor externe gebruikers, klikt u op **koppeling kopiëren,** verdeel de koppeling vervolgens naar externe gebruikers.\
   Gebruikers met de koppeling kunnen het object weergeven.

   >[!CAUTION]
   >
   We raden u aan voorzichtig te zijn wanneer u een object met vertrouwelijke informatie deelt met externe gebruikers. Op deze manier kunnen ze informatie weergeven zonder dat ze een Workfront-gebruiker of onderdeel van uw organisatie zijn.

1. Klikken **Opslaan**.

## Objecten bulksgewijs delen

Vanuit een lijst met objecten kunt u meerdere objecten tegelijk delen met andere gebruikers, teams, groepen, taakrollen of bedrijven.

>[!IMPORTANT]
>
Wanneer u objecten in bulk deelt, worden de namen van de entiteiten die machtigingen hebben voor de afzonderlijke objecten niet weergegeven. Wanneer u objecten in bulk deelt, worden de entiteiten die u toevoegt aan de lijst voor gedeeld gebruik toegevoegd aan de geselecteerde objecten. Ze overschrijven niet de entiteiten die aan de afzonderlijke objecten zijn gekoppeld. 

Objecten bulksgewijs delen:

1. Navigeer naar een lijst met objecten.
1. Selecteer twee of meer objecten in de lijst.
1. Klik op de knop **Delen** pictogram ![](assets/share-icon.png).\
   Gebruikers die al toegang tot het object hebben, worden niet vermeld als beschikbaar bij het delen van grote hoeveelheden.

   >[!NOTE]
   >
   Als u geen machtigingen hebt om een geselecteerd object te delen, kunt u het volgende doen: **Delen** is niet zichtbaar.

1. In de **Bewerken `<Object Name>` toegang voor** veld, typ de naam van een gebruiker, team, groep, taakrol of bedrijf waaraan u machtigingen wilt verlenen.

   Als u bijvoorbeeld een project deelt, gebruikt u de opdracht **Projecttoegang verlenen voor** veld.

   ![](assets/share-multiple-projects-people-box-nwe-350x480.png)

1. Doorgaan met het delen van de geselecteerde objecten, zoals beschreven in stap 4-9 in de sectie [Eén object delen](#share-a-single-object) in dit artikel.

   <!--
   <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
   (NOTE: ensure these steps stay accurate; always look at them in the viewer; because of condiitoning, the steps numbers in the editor are different!!!!!!*****)
   </MadCap:conditionalText>
   -->

1. Klikken **Opslaan**.
