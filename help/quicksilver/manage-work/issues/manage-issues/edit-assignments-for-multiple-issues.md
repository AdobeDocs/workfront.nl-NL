---
product-area: projects
navigation-topic: manage-issues
title: Gebruikerstoewijzingen wijzigen voor meerdere uitgaven in een lijst
description: Gebruikerstoewijzingen wijzigen voor meerdere uitgaven in een lijst
author: Alina
feature: Work Management
exl-id: e1e75027-1847-44cf-afeb-b19394dc3ea5
source-git-commit: daba001c28df268721c87df7d2516ffb76e535d9
workflow-type: tm+mt
source-wordcount: '773'
ht-degree: 0%

---

# Gebruikerstoewijzingen wijzigen voor meerdere uitgaven in een lijst

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: similar article exists for tasks)</p>
-->

U kunt gebruikerstoewijzingen aan veelvoudige kwesties gelijktijdig wijzigen. Zie ook de volgende artikelen voor informatie over het bewerken van uitgaven of het een voor een toewijzen van uitgaven:

* [Problemen bewerken](../../../manage-work/issues/manage-issues/edit-issues.md)
* [Problemen toewijzen](../../../manage-work/issues/manage-issues/assign-issues.md)

Voor algemene informatie over het toewijzen van problemen raadpleegt u [Overzicht van het wijzigen van uitgaven](../../../manage-work/issues/manage-issues/modify-issue-assignments-overview.md).

>[!NOTE]
>
>U moet ten minste over Contribute-machtigingen beschikken om een uitgave te kunnen toewijzen aan de uitgave.

## Toegangsvereisten

U moet de volgende toegang hebben om de stappen in dit artikel uit te voeren:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-abonnement*</td> 
   <td> <p>Alle </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-licenties*</td> 
   <td> <p>Aanvraag of hoger</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraties op toegangsniveau*</td> 
   <td> <p>Toegang tot problemen bewerken</p> <p>Opmerking: als u nog steeds geen toegang hebt, vraag dan aan de Workfront-beheerder of deze aanvullende beperkingen op uw toegangsniveau heeft ingesteld. Voor informatie over hoe een beheerder van Workfront uw toegangsniveau kan wijzigen, zie <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Aangepaste toegangsniveaus maken of wijzigen</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objectmachtigingen</td> 
   <td> <p>Rechten voor het probleem beheren</p> <p>Voor informatie over het aanvragen van aanvullende toegang raadpleegt u <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Toegang tot objecten aanvragen </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Neem contact op met uw Workfront-beheerder om te weten te komen welk plan, licentietype of toegang u hebt.

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<h2>When to modify user assignments on issues</h2>
<p>(NOTE:&nbsp;drafted and moved to the overview article: Modify issue assignments overview)</p>
<p>You might want to modify the user assignments for multiple issues for a variety of&nbsp;reasons, including the following:</p>
<ul>
<li>Users join or leave&nbsp;your team</li>
<li>A user takes a vacation that extends beyond the issue&nbsp;due dates</li>
<li>A specific role or user is set as the assignee for multiple issues and you want to quickly modify all items to be assigned to a different user or role</li>
</ul>
</div>
-->

## Toewijzingen wijzigen voor meerdere problemen

1. Ga naar de lijst van de kwestie die de kwesties bevat waarvan taken u wilt wijzigen.
1. (Optioneel) Maak een filter om alleen uitgaven weer te geven die zijn toegewezen aan de ontvanger die u wilt wijzigen.

   U kunt bijvoorbeeld een filter maken om alleen uitgaven weer te geven die een specifieke rol als toegewezen persoon hebben. Vervolgens kunt u de rol vervangen door een specifieke gebruiker. Ga als volgt te werk:

   1. Klik op de knop **Filter** vervolgkeuzelijst en vervolgens op **Nieuw filter**.

      Het dialoogvenster Nieuw filter wordt weergegeven.

   1. Klikken **Voeg een filterregel toe.**
   1. Om voor een specifieke rol te filteren, breid uit **Toewijzingsrollen,** klik vervolgens op **ID.**

      of

      Als u voor een specifieke gebruiker wilt filteren, vouwt u **gebruikers van de toewijzing,** klik vervolgens op **ID.**

      >[!TIP]
      >
      >Niet gebruiken **Toegewezen aan** omdat dit veld alleen naar de eigenaar van de uitgave verwijst en niet naar alle toegewezen personen.

   1. Selecteer in de vervolgkeuzelijst de optie **Gelijk** als de filterkwalificatie.
   1. Typ de naam van de gebruiker of rol waarvoor u wilt filteren en klik vervolgens op de naam wanneer deze wordt weergegeven in de vervolgkeuzelijst.
   1. Klikken **Filter opslaan.**

1. Selecteer de problemen waarvoor u toewijzingen wilt wijzigen en klik op de knop **Bewerken** pictogram ![](assets/qs-edit-icon.png).

   De **Problemen bewerken** worden weergegeven. De items die worden bewerkt, worden in de linkerbovenhoek van de pagina weergegeven.

1. Ga naar de **Toewijzingen** sectie selecteert u vervolgens **Geadresseerde**.

   ![](assets/classic-assignmens-area-on-edit-box-350x119.png)

1. Voer een van de volgende handelingen uit:

   1. Een nieuwe ontvanger toevoegen:

      1. Begin de naam van een gebruiker, een rol, of een team te typen, dan het te selecteren wanneer het in de lijst toont. De toewijzing wordt toegevoegd en vervangt de huidige toewijzingen voor de geselecteerde uitgaven niet.

         >[!TIP]
         >
         U kunt meerdere gebruikers, taakrollen of teams toewijzen. U kunt alleen actieve gebruikers, taakrollen en teams toewijzen.
         >
         Als een gebruiker, een baanrol, of een team werd toegewezen alvorens zij werden gedeactiveerd, blijven zij toegewezen aan het het werkpunt. In dit geval raden we het volgende aan:
         >
         * Wijs het werkitem opnieuw toe aan actieve bronnen.
         * Koppel de gebruikers in een gedeactiveerd team aan een actief team en wijs het het werkpunt aan het actieve team opnieuw toe.

         Informatie die algemeen is voor alle geselecteerde uitgaven, wordt weergegeven. Als bijvoorbeeld dezelfde gebruiker aan alle uitgaven is toegewezen, wordt die gebruiker in het dialoogvenster **Geadresseerde** kolom. Als er geen algemene informatie wordt weergegeven over de geselecteerde problemen.

   1. Afzonderlijke toewijzingen verwijderen:

      1. Klik op de knop **X-pictogram** naast de naam van de toegewezen persoon die u wilt verwijderen als de toegewezen persoon wordt weergegeven in de lijst Toewijzingen.

         of

         (Voorwaardelijk) Als de toegewezen persoon die u wilt verwijderen niet wordt weergegeven in de sectie Toewijzingen omdat de toegewezen persoon is toegewezen aan slechts een aantal van de geselecteerde problemen, klikt u op **Toegewezen verwijderen** en typ de naam van de toegewezen persoon die u wilt verwijderen. Klik vervolgens op de naam wanneer deze wordt weergegeven in de vervolgkeuzelijst.

      1. Klikken **Toegewezen verwijderen** opnieuw om een andere te verwijderen ontvanger toe te voegen.

   1. Alle bestaande toewijzingen verwijderen:

      1. Klikken **Alle bestaande toewijzingen verwijderen** en klik vervolgens op **Ja, alle toewijzingen verwijderen**.

         Hierdoor worden niet alleen algemene toewijzingen (toewijzingen die in het dialoogvenster Bewerken worden weergegeven), maar ook alle toewijzingen voor alle geselecteerde problemen verwijderd.

1. (Optioneel) Wijzig een of meer van de volgende opties voor de toewijzingen die u hebt geselecteerd om aan de problemen te koppelen:

   * **Eigenaar van uitgave:** Selecteer het keuzerondje om aan te geven welke ontvanger is aangewezen als eigenaar van uitgifte. Als deze optie niet is geselecteerd, wijst Adobe Workfront de eerste toegewezen persoon aan als de eigenaar van de uitgave. Dit is niet beschikbaar voor teamtoewijzingen.
   * **Rol van de gemachtigde**: Selecteer een rol in de vervolgkeuzelijst. Als deze optie niet is geselecteerd, selecteert Workfront automatisch de primaire rol van de gebruiker.

1. Klikken **Wijzigingen opslaan**.
