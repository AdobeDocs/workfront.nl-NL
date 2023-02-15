---
product-area: resource-management
navigation-topic: resource-planning
title: De middelen van de begroting in de Planner van het Middel gebruikend de meningen van het Project en van de Rol
description: U kunt middelen in de Planner van het Middel van Adobe Workfront begroten gebruikend de mening van het Project en van de Rol. U kunt geen middelen begroten gebruikend de mening van de Gebruiker in de Planner van het Middel.
author: Alina
feature: Resource Management
exl-id: b1b48529-68e7-4aee-aaa1-d78e91fbb39c
source-git-commit: 3486a2523a038bdd83c3c2001001a119fd0508ad
workflow-type: tm+mt
source-wordcount: '2160'
ht-degree: 0%

---

# De middelen van de begroting in de Planner van het Middel gebruikend de meningen van het Project en van de Rol

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: broken off of another larger article (Planning in the RP); reformat, restructure, relink)</p>
-->

De belangrijkste functie van de Planner van het Middel is uw middelen voor het werk te begroten dat aan projecten moet worden voltooid.

>[!IMPORTANT]
>
>U kunt uw middelen alleen begroten als u de **Weergeven op project** of **Weergeven op rol** weergaven naar de bronnenplanner.

Lees de volgende artikelen voordat u begint met budgetinformatie in de functie voor middelenplanning:

* [Overzicht van de bronnenplanner](../../resource-mgmt/resource-planning/get-started-resource-planner.md)
* [Toegang tot begrotingsmiddelen in Adobe Workfront](../../resource-mgmt/resource-planning/access-needed-to-budget-resources.md)
* [Overzicht van uren, FTE, en kosteninformatie in de mening van het Project en van de Rol van de Planner van het Middel](../../resource-mgmt/resource-planning/overview-of-planner-hour-fte-cost-information-in-role-project-views.md)

## Toegangsvereisten

U moet de volgende toegang hebben om de stappen in dit artikel uit te voeren:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-abonnement*</td> 
   <td> <p>Pro en hoger</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-licentie*</td> 
   <td> <p>Plan </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraties op toegangsniveau*</td> 
   <td> <p>Toegang tot resourcebeheer bewerken, inclusief toegang tot bewerkingsprioriteiten en begrotingstijden in de bronnenplanner</p> <p>Toegang tot financiële gegevens voor begrotingsmiddelen via kostenaanpassing bewerken</p> <p>Toegang tot projecten en gebruikers bewerken</p> <p><b>OPMERKING</b>

Als u nog steeds geen toegang hebt, vraagt u de Workfront-beheerder of deze aanvullende beperkingen op uw toegangsniveau instelt. Voor informatie over hoe een beheerder van Workfront uw toegangsniveau kan veranderen, zie <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Aangepaste toegangsniveaus maken of wijzigen</a>.</p> </td>
</tr> 
  <tr> 
   <td role="rowheader">Objectmachtigingen</td> 
   <td> <p>Rechten beheren voor de projecten waarvoor u begrotingsgegevens wilt opgeven</p> <p>Voor informatie over het aanvragen van aanvullende toegang raadpleegt u <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Toegang tot objecten aanvragen </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Neem contact op met uw Workfront-beheerder om te weten te komen welk plan, licentietype of toegang u hebt.

## Begrotingsmiddelen in de middelenplanner

* [Begrotingsmiddelen in de projectweergave](#budget-resources-in-the-project-view)
* [Begrotingsmiddelen in de weergave Rol](#budget-resources-in-the-role-view)
* [Begrotingsmiddelen in bulk](#budget-resources-in-bulk)

### Begrotingsmiddelen in de projectweergave {#budget-resources-in-the-project-view}

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: this section is linked to the Budgeting Project Resources in the Business Case article)</p>
-->

1. Klik op de knop **Hoofdmenu** pictogram ![](assets/main-menu-icon.png) in de rechterbovenhoek van Adobe Workfront.

1. Klikken **Bronnen**.
1. De **Planner** worden standaard weergegeven.
1. (Voorwaardelijk) Selecteer **Weergeven op project** weergeven.
1. Breid de projecten en de baanrollen uit om de toewijzing voor het project, baanrollen, of gebruikers te beheren.
1. Voer een van de volgende handelingen uit om uw budget toe te wijzen aan gebruikers:

   * In de **BDG** voor de gebruikers handmatig een aantal begrote uren, FTE of kosten opgeven.

   * Klik op de knop **Meer** menu voor de taakrol van de gebruiker en klik vervolgens op **Geplande uren van gebruikers instellen als begroot**.\
      De begrotingsuren van elke gebruiker worden berekend met behulp van de volgende formule:

      ```
      User Budgeted Hours = User Planned Hours
      ```

1. Voer een van de volgende handelingen uit om begrotingstoewijzing voor taakrollen toe te wijzen:

   * In de **BDG** kolom, geeft u handmatig een aantal begrote uren, FTE of kosten voor de rol van de taak op.

      >[!NOTE]
      >
      >De rol begrotingsuren wordt toegevoegd aan het voor het project begrote uren uur.

   * (Voorwaardelijk) Als u de uren voor gebruikers in de begroting hebt opgenomen, klikt u op **Meer** menu voor de taakrol en klik vervolgens op **Totaal aantal bestede uren van gebruikers voor rol**.\
      De begrotingsuren voor elke rol worden berekend met behulp van de volgende formule:

      ```
      Role Budgeted Hours = SUM(User Budgeted Hours)
      ```

   * Klik op de knop **Meer** menu voor het project en klik vervolgens op **Geplande uren voor rollen instellen als begroot**.\
      De begrotingsuren voor elke rol worden berekend met behulp van de volgende formule:\
      *

      ```
      Role Budgeted Hours = Role Planned Hours
      ```

      >[!NOTE]
      >   
      >* De rol begrotingsuren wordt toegevoegd aan het voor het project begrote uren uur.
      >* De gebruikers kunnen voor zowel Primaire als Andere (of secundaire) Rollen in de begroting worden opgenomen.
      >* De **Percentage van de beschikbaarheid van VTE** voor de rollen van de gebruiker moet een aantal verschillend zijn dan 0% voor de Beschikbare Uren om een waarde in de Planner van het Middel voor een baanrol te tonen. Als een gebruiker aan een rol met 0% wordt geassocieerd **Percentage van de beschikbaarheid van VTE** De waarde voor Beschikbare uren is nul voor die taakrol. In dit geval kan de rol negatief zijn **Nettowaarde**.\
         >Voor meer informatie over de **Percentage van de beschikbaarheid van VTE** zie het artikel voor taakrollen [Gebruikersprofiel bewerken](../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).


   * In de **BDG** kolom, geeft u handmatig een aantal begrote uren, FTE of kosten voor het project op. Hierdoor wordt het aantal begrote uren projecturen verdeeld over elke rol in het kader van het project. De volgende scenario&#39;s bestaan:

      * Als het aantal begrote uren uren van het Project uw specificeert de Geplande Uren van het Project evenaart, past de Rol Geplande Uren de Rol de Geplande Uren.
      * Als het aantal begrote uren uren van het Project u specificeert niet de Geplande Uren van het Project evenaart, wordt de Rol Geboedgeted Uren verdeeld volgens het percentage Geplande Uren nodig voor elke rol.\
         Bijvoorbeeld, als een project 20 Geplande Uren heeft, en zij tussen twee baanrollen worden verdeeld (de Consultant vereist 12 Geplande Uren en de Ingenieur vereist 8 Geplande Uren), en u begroot 30 uren voor het Project, worden de uren verdeeld als volgt: de rol van consultant ontvangt 18 begrotingsuren en de rol van ingenieur krijgt 12 begrotingsuren.

1. Voer een van de volgende handelingen uit om een budget voor het project toe te wijzen:

   * Begroting van de rollen in het kader van het project, zoals beschreven in Stap 7.\
      Het voor het project uitgetrokken aantal uren wordt berekend aan de hand van de volgende formule:

      ```
      Project Budgeted Hours = SUM(Role Budgeted Hours)
      ```

   * In de **BDG** kolom, geeft u handmatig een aantal begrote uren, FTE of kosten voor het project op.\
      Hiermee werkt u de rol die is toegewezen aan uren bij, zoals beschreven in stap 7.\
      ![budget_for_project.png](assets/budget-for-project-350x182.png)

1. Klikken **Opslaan**.\
   Nadat u uw middelen in de Planner van het Middel begroot, zijn de Begrotingstijd voor uw middelen en om het even welke kosten verbonden aan hen vermeld in het BedrijfsGeval van elk project.\
   Voor meer informatie over het begrijpen van het gebied van de Begroting van het Middel van het BedrijfsGeval, zie de sectie &quot;het Leiden van het Middel&quot;in het artikel [Overzicht van de gebieden van de bedrijfscase](../../manage-work/projects/define-a-business-case/areas-of-business-case.md).

1. (Optioneel) Selecteer de weergave Gebruiker om te zien of de gebruiker teveel of te weinig gebruikmaakt van de beschikbare en geplande uren voor elke gebruiker. De begrote uren uren zijn niet zichtbaar in de mening van de Gebruiker.

   Voor informatie over hoe Workfront de beschikbaarheid van een gebruiker berekent, raadpleegt u [Voorkeuren voor beheer van bronnen configureren](../../administration-and-setup/set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md).

### Begrotingsmiddelen in de weergave Rol {#budget-resources-in-the-role-view}

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<p>(NOTE: THIS IS WRONG - I LOGGED A BUG TO FIX THIS LINK - IT SHOULD GO TO"ACCESS NEEDED TO BUDGET IN THE RP":</p>
<p>Planning in the resource planner has links to the UI - ensure Flare notes are there for this: https://workfront.zendesk.com/hc/en-us/articles/115006356928 - the "Budgeting resources in the role view" is linked to this tooltip: ***This is linked to the product in the RP when the user does not have Manage rights on one of the projects under the role. This tool tip is linked here: "You don't have Manage permissions for all projects. Budget hours by individual project instead. Learn more...")</p>
</div>
-->

U moet Edit toegang tot het Beheer van het Middel en Financiële Gegevens hebben en de toestemmingen van de Financiën van het Beheer op de projecten om middelen in de Planner van het Middel te begroten. Als u slechts de toegang van de Mening tot minstens één project hebt dat onder een baanrol wordt vermeld, kunt u geen toewijzingen voor de rol in de mening van de Rol begroten. U kunt budgettoewijzing voor de projecten nog steeds uitvoeren waarvoor u beheermachtigingen hebt.

Zie het artikel voor informatie over de toegang die nodig is voor het begroten van middelen [Toegang tot begrotingsmiddelen in Adobe Workfront](../../resource-mgmt/resource-planning/access-needed-to-budget-resources.md).

Aan begrotingstoewijzingen in de Planner van het Middel in de*** mening van de Rol:

1. Klik op de knop **Hoofdmenu** pictogram ![](assets/main-menu-icon.png) in de rechterbovenhoek van Adobe Workfront.

1. Klikken **Bronnen**.
1. De **Planner** worden standaard weergegeven.
1. (Voorwaardelijk) Selecteer **Weergeven op rol** weergeven.
1. Breid de baanrollen en de projecten uit om de toewijzing voor het project, baanrollen, of gebruikers te beheren.
1. Voer een van de volgende handelingen uit om uw budget toe te wijzen aan gebruikers:

   * In de **BDG** voor de gebruikers handmatig een aantal begrote uren, FTE of kosten opgeven.
   * Klik op de knop **Meer** menu voor het project en klik vervolgens op **Geplande uren van gebruikers instellen als begroot**.\
      De begrotingsuren van elke gebruiker worden berekend met behulp van de volgende formule:

      ```
      User Budgeted Hours = User Planned Hours
      ```

1. Voer een van de volgende handelingen uit om begrotingstoewijzing voor taakrollen toe te wijzen:

   * In de **BDG** kolom, geeft u handmatig een aantal begrote uren, FTE of kosten voor de taakrollen op.\
      Dit verdeelt de Rol Geboedde Uren aan het Project Geplande Uren voor de projecten die u toegang hebt om te leiden.

   * Klik op de knop **Meer** Klik vervolgens op **Stel de geplande uren voor projecten in op de begrote waarde.**De Rol die in de begroting wordt opgenomen Uren wordt berekend gebruikend de volgende formule:\
      *

      ```
      Role Budgeted Hours = SUM(Project Budgeted Hours)
      ```

      *Het voor het project uitgetrokken aantal uren wordt berekend met behulp van de volgende formule:

      ```
      Project Budgeted Hours = Project Planned Hours
      ```

   * In de **BDG** kolom, geeft u handmatig een aantal begrote uren, FTE of kosten op voor de projecten die onder de taakrol worden vermeld.\
      Hiermee voegt u het aantal begrote uren projecturen toe aan de rol.
   >[!NOTE]
   >
   >De gebruikers kunnen voor zowel Primaire als Andere (of secundaire) Rollen in de begroting worden opgenomen. De **Percentage van de beschikbaarheid van VTE** voor de rollen van de gebruiker moet een aantal verschillend zijn dan 0% voor de Beschikbare Uren om een waarde in de Planner van het Middel voor een baanrol te tonen. Als een gebruiker aan een rol met 0% wordt geassocieerd **Percentage van de beschikbaarheid van VTE** De waarde voor Beschikbare uren is nul voor die taakrol. In dit geval kan de rol negatief zijn **Nettowaarde**.\
   >Voor meer informatie over de **Percentage van de beschikbaarheid van VTE** zie het artikel voor taakrollen [Gebruikersprofiel bewerken](../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

1. Voer een van de volgende handelingen uit om een budget voor het project toe te wijzen:

   * In de **BDG** kolom, geeft u handmatig een aantal begrote uren, FTE of kosten voor de projecten op.\
      Dit werkt ook de begrotingsuren bij voor de rollen waaronder het project wordt vermeld.

   * Klik op de knop **Meer** menu voor de taakrol en klik vervolgens op **Geplande uren voor projecten instellen als begroot**.\
      De voor het project uitgetrokken uren worden berekend aan de hand van de volgende formule:

      ```
      Project Budgeted Hours = Project Planned Hours
      ```

      De begrote uren projecturen worden toegevoegd aan de Rol Geforceerde Uren.

   * (Voorwaardelijk) Als u de uren voor de gebruikers in de begroting hebt opgenomen, klikt u op **Meer** menu voor het project en klik vervolgens op **Totaal aantal bestede uren van gebruikers voor project**.\
      Het budget voor het project wordt berekend met behulp van de volgende formule:

      ```
      Project Budgeted Hours = SUM(User Budgeted Hours)
      ```

      ![budget_by_rol.png](assets/budget-by-role-350x181.png)

1. Klikken **Opslaan**.\
   Nadat u uw middelen in de Planner van het Middel begroot, zijn de Begrotingstijd voor uw middelen en om het even welke kosten verbonden aan hen vermeld in het BedrijfsGeval van elk project.\
   Raadpleeg het artikel voor meer informatie over het budgetteren van bronnen in de Business Case [Begrotingsmiddelen in het bedrijfscase](../../manage-work/projects/define-a-business-case/budget-resources-in-business-case.md).

1. (Optioneel) Selecteer de optie **Weergeven op gebruiker** om te zien hoe gebruikers te veel of te weinig gebruikmaken van de beschikbare en geplande uren voor elke gebruiker. De begrote Uren zijn niet zichtbaar in de Mening door Gebruiker.

### Begrotingsmiddelen in bulk {#budget-resources-in-bulk}

U kunt begrotingstoewijzingen voor uw middelen in bulk wanneer het gebruiken van snelle verbindingen. De snelle verbindingen zijn beschikbaar slechts voor de Mening van het Project en van de Rol.

![](assets/rp-project-view-with-automatic-budgeting-options-on-project-350x173.png)

>[!NOTE]
>
>Wanneer de snelle koppelingen naar begrotingstoewijzingen voor middelen worden gebruikt, wordt de begroting automatisch alleen toegepast op de tijdsperiodes die op het scherm worden weergegeven. Als de tijdlijn van een project langer duurt dan de tijdlijn die op uw scherm wordt weergegeven, moet u van links naar rechts schuiven en de snelle koppelingen gebruiken om uw bronnen automatisch te begroten.

Om uw middelen in massa te begroten:

1. Ga naar de .\
   Voor meer informatie over de toegang tot van de Planner van het Middel, zie de &quot;Toegang tot de Planner van het Middel&quot;sectie in het artikel [Overzicht van de bronnenplanner](../../resource-mgmt/resource-planning/get-started-resource-planner.md).\
   Een lijst met projecten die u kunt beheren, wordt weergegeven in de lijst.

1. (Optioneel) Vouw elk project uit om een lijst met functies weer te geven die aan het project zijn gekoppeld.\
   of
1. (Optioneel) Selecteer **Weergeven op rol**, dan breid elke rol uit om een lijst van projecten te zien verbonden aan het.
1. Houd de aanwijzer boven de naam van een project of een functie.
1. Klik op de knop **Meer** pictogram ![options_icon_resource_planner.png](assets/options-icon-resource-planner.png)die uiterst rechts van de project- of rolnaam wordt weergegeven.

1. Klik op een van de beschikbare opties om automatisch de hoeveelheid begrote uren uren (BDG) voor andere objecten op te geven.

   Afhankelijk van het feit of u op het pictogram Meer op een project of een rol hebt geklikt, zijn de opties voor het bulksgewijs in de begroting opnemen verschillend. In de onderstaande tabel worden de opties weergegeven die beschikbaar zijn voor projecten en rollen:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td> </td> 
      <td><strong>Projectweergave</strong> </td> 
      <td><strong>Rolweergave</strong> </td> 
     </tr> 
     <tr> 
      <td>Projectopties</td> 
      <td> 
       <ul> 
        <li><strong>Geplande uren voor rollen instellen als begroot</strong>: Selecteer deze optie als u de begrotingsuren van de rol identiek wilt maken aan de geplande uren. Het totaal van de begrote uren uren voor de rollen zal voor het Project worden getoond die Uren wordt begroot. </li> 
        <li><strong>Bochtingsdatums aanpassen</strong> : Selecteer deze optie als u de begrote uren uren naar een ander tijdpad wilt verplaatsen.<br>Voor meer informatie over het aanpassen van de begrotingsdata raadpleegt u <a href="../../resource-mgmt/resource-planning/adjust-budgeting-dates.md" class="MCXref xref">Datums voor budgettering aanpassen in de functie voor middelenplanning</a>.</li> 
       </ul> </td> 
      <td> 
       <ul> 
        <li><strong>Geplande uren van gebruikers instellen als begroot</strong>: Schakel deze optie in om de begrote uren uren van de gebruiker gelijk te maken aan de geplande uren. </li> 
        <li><strong>Totaal aantal bestede uren van gebruikers voor project</strong>: Selecteer deze optie als u alle door de gebruiker begrote uren uren uren samen wilt toevoegen en het totaal als de begrote uren uren uren voor het project en voor de rol wilt weergeven. We raden u aan deze optie te gebruiken nadat u de gebruikers handmatig in de begroting hebt opgenomen of de vorige optie eerst hebt gebruikt. </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td>Rolopties</td> 
      <td> 
       <ul> 
        <li><strong>Geplande uren van gebruikers instellen als begroot</strong>: Selecteer deze optie om de begrote uren uren van de gebruiker identiek te maken aan hun Geplande uren. </li> 
        <li><strong>Totaal aantal bestede uren van gebruikers voor rol</strong>: Selecteer deze optie als u alle begrote uren uren van de gebruiker bij elkaar wilt optellen en het totaal als de begrote uren uren voor de rol en het project wilt weergeven. We raden u aan deze optie te gebruiken nadat u de gebruikers handmatig in de begroting hebt opgenomen of de vorige optie eerst hebt gebruikt. </li> 
       </ul> </td> 
      <td> 
       <ul> 
        <li><strong>Geplande uren voor projecten instellen als begroot</strong>: Selecteer deze optie om het project begrotingsuren identiek te maken aan het project Geplande Uren. </li> 
       </ul> </td> 
     </tr> 
    </tbody> 
   </table>

   >[!NOTE]
   >
   >Sommige opties worden mogelijk niet weergegeven als aan een aantal voorwaarden voor het werken in de functie Bronnen ontbreekt.
   >
   >
   >Voor meer informatie over de eerste vereisten waaraan moet worden voldaan voor een juiste budgettering in de functie voor middelentoewijzing raadpleegt u de sectie &quot;Voorwaarden voor het werken in de functie voor middelenplanner&quot; in het gedeelte [Overzicht van de bronnenplanner](../../resource-mgmt/resource-planning/get-started-resource-planner.md) artikel.\
   >Sommige opties worden bijvoorbeeld niet weergegeven in de volgende scenario&#39;s:
   >
   >   
   >   
   >   * Wanneer de projecten niet met de Pool van het Middel worden geassocieerd
   >   * Wanneer de Groepen van het Middel die met projecten worden geassocieerd geen gebruikers bevatten
   >   * Wanneer de Pools van het Middel die met projecten worden geassocieerd gebruikers zonder baanrol verbonden aan hen bevatten.

