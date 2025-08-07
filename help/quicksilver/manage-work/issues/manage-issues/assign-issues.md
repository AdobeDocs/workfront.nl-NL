---
product-area: projects
navigation-topic: manage-issues
title: Problemen toewijzen
description: U kunt problemen toewijzen aan gebruikers, rollen en teams om aan te geven wie verantwoordelijk is voor het voltooien van de problemen. Voor algemene informatie over het toewijzen van kwesties, zie wijzigen uitgeeft overzicht.
author: Alina
feature: Work Management
role: User
exl-id: e2dce29e-7370-4580-8326-99c4437998bf
source-git-commit: a0b635953245cf307b558d343ad234a27c96da94
workflow-type: tm+mt
source-wordcount: '1433'
ht-degree: 0%

---

# Problemen toewijzen

{{preview-fast-release-general}}

<!--Audited: 07/2024-->

U kunt problemen toewijzen aan gebruikers, rollen en teams om aan te geven wie verantwoordelijk is voor het voltooien van de problemen. Voor algemene informatie over het toewijzen van kwesties, zie [ Overzicht van het wijzigen van uitgiftetaken ](../../../manage-work/issues/manage-issues/modify-issue-assignments-overview.md).

>[!TIP]
>
>U kunt meerdere gebruikers, taakrollen of teams toewijzen. U kunt alleen actieve gebruikers, taakrollen en teams toewijzen.
>
>Als een gebruiker, een baanrol, of een team werden toegewezen alvorens zij werden gedeactiveerd, blijven zij toegewezen aan het het werkpunt. In dit geval raden we het volgende aan:
>
>* Wijs het werkitem opnieuw toe aan actieve bronnen.
>* Koppel de gebruikers in een gedeactiveerd team aan een actief team en wijs het het werkpunt aan het actieve team opnieuw toe.

Naast dit artikel raden we u aan de volgende artikelen te lezen voor meer informatie over het toewijzen van problemen:

* [ Overzicht van het wijzigen van uitgiftetaken ](../../../manage-work/issues/manage-issues/modify-issue-assignments-overview.md)
* [ geeft kwesties ](../../../manage-work/issues/manage-issues/edit-issues.md) uit
* [ wijzig gebruikerstoewijzingen voor veelvoudige kwesties in een lijst ](../../../manage-work/issues/manage-issues/edit-assignments-for-multiple-issues.md)
* [ creeer geavanceerde taken ](../../../manage-work/tasks/assign-tasks/create-advanced-assignments.md)
* [ maak slimme taken ](../../../manage-work/tasks/assign-tasks/make-smart-assignments.md)
* [ Slim overzicht van taken ](../../../manage-work/tasks/assign-tasks/smart-assignments.md)
* [Overzicht van het toewijzen van werk in de werklastverdeler](../../../resource-mgmt/workload-balancer/assign-work-in-workload-balancer.md)

U kunt een kwestie aan één of veelvoudige middelen op het individuele emissieniveau toewijzen, of u kunt veelvoudige middelen aan veelvoudige kwesties in één keer toewijzen.

Het toewijzen van problemen en taken is vergelijkbaar in Adobe Workfront. Voor algemene informatie over het toewijzen van taken, zie [ Overzicht van het wijzigen van taaktaken ](../../../manage-work/tasks/assign-tasks/modify-task-assignments-overview.md).

## Toegangsvereisten

+++ Breid uit om de toegangseisen voor de functionaliteit in dit artikel weer te geven.

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-plan</td> 
   <td> <p>Alle </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-licentie*</td> 
   <td> <p>Nieuw: Medewerker of hoger</p>
   <p>Huidig: Controleren of hoger</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Toegangsniveau</td> 
   <td> <p>Toegang tot problemen bewerken</p> <p>De mening of de hogere toegang tot Projecten en Taken om één kwestie toe te wijzen</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objectmachtigingen</td> 
   <td> <p>Rechten voor het probleem beheren</p> <p> Toestemmingen van de mening of hoger aan het project of de taak waar de kwestie wordt gevestigd, wanneer het toewijzen van één kwestie</p><p>Contribute-machtigingen of hoger voor het project of de taak waar de uitgave zich bevindt, wanneer u meerdere uitgaven toewijst.</p> </td> 
  </tr> 
 </tbody> 
</table>

*For informatie, zie [ vereisten van de Toegang in de documentatie van Workfront ](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Overwegingen voor veelvoudige taken aan baanrollen, teams, en gebruikers

Overweeg het volgende wanneer het toewijzen van veelvoudige middelen aan een het werkpunt:

* Gebruikers kunnen meer dan één taakrol aan hun profiel koppelen. Voor informatie over het associëren van gebruikers met baanrollen, zie [ het profiel van een gebruiker ](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md) uitgeven.

* Taken of problemen worden doorgaans eerst toegewezen aan een of meerdere taakrollen of teams. Wanneer de projecten klaar zijn om te beginnen, zouden zij ook aan gebruikers kunnen moeten worden toegewezen.

  Als een taak of een kwestie aan één of veelvoudige rollen wordt toegewezen en u dan ook een gebruiker toewijst, beslist Adobe Workfront welke baanrol aan de extra gebruiker (als om het even welk) te associëren volgens de volgende regels:

   * Als er slechts één taakrol is toegewezen en deze overeenkomt met de primaire rol van de gebruiker, wordt de taak of kwestie alleen toegewezen aan de gebruiker die zijn primaire rol vervult.
   * Als er veelvoudige toegewezen rollen zijn en minstens één van de rollen de secundaire rollen van de gebruiker aanpast, dan wordt de taak of de kwestie toegewezen aan de gebruiker die één van hun Andere Rollen vervult — die Workfront willekeurig selecteert als er veelvoudige gelijken zijn — evenals om het even welke extra rollen die worden toegewezen.
   * Als er een of meer toegewezen taakrollen zijn en er geen overeenkomsten met de rollen van de gebruiker zijn, dan wordt de taak of kwestie toegewezen aan zowel de rol of de rollen als aan de gebruiker.

* Als een taak of een kwestie aan een team wordt toegewezen en u ook een gebruiker toewijst, blijft de taak of de kwestie toegewezen aan zowel het team als de gebruiker.

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<h2> </h2>
<h2>Considerations about removing assignments from issues</h2> 
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: drafted and moved to Modify issue assignments overview article)</p>
<p>You can remove assignments from one issue at a time, or you can remove assignments from multiple issues in bulk.</p>
<p>For more information about removing assignments from issues in bulk, see <a href="../../../manage-work/issues/manage-issues/edit-assignments-for-multiple-issues.md" class="MCXref xref">Modify user assignments for multiple issues in a list</a>. </p>
<p>Consider the following when removing assignments from issues: </p>
<ul>
<li>When you unassign a user from an issue, the issue remains assigned to the job role that the user fulfilled on the issue.</li>
<li>When you unassign a job role or a team from an issue, the issue remains unassigned if it is not assigned to any other resources. </li>
</ul>
</div>
-->

## Eén probleem toewijzen

1. Ga naar een probleem dat u wilt toewijzen.
1. Klik **toewijzen aan** in de hoger-juiste hoek van de punthoofdbal, in het **gebied van Taken**

   of

   Klik op de naam van de huidige toewijzingen als de uitgave al is toegewezen.

   ![ wijs aan knoop toe ](assets/assign-to-button-in-header.png)

1. Voer een van de volgende handelingen uit:

   * Typ de naam van een gebruiker, rol of team die u wilt toewijzen en klik vervolgens op de naam wanneer deze in de lijst wordt weergegeven.

     ![ het onderzoek van Taken ](assets/smart-assignments-issue-header.png)

   * (Voorwaardelijk) Klik één van de namen, rollen, of teams in de beschikbare lijsten
   * Klik **toewijzen aan me** om het aan zich toe te wijzen
   * Klik **Geavanceerd**.

     Het maken van geavanceerde toewijzingen is vergelijkbaar voor taken en problemen. Voor informatie over hoe te om geavanceerde taken te maken, zie [ Geavanceerde taken ](../../../manage-work/tasks/assign-tasks/create-advanced-assignments.md) creëren.

     >[!TIP]
     >
     >Wanneer u een gebruikerstoewijzing toevoegt, ziet u de avatar, de primaire rol van de gebruiker of hun e-mailadres om onderscheid te maken tussen gebruikers met identieke namen.
     >
     >Gebruikers moeten aan ten minste één taakrol zijn gekoppeld om deze te kunnen bekijken terwijl u ze toevoegt.
     >
     >De instelling Contactinfo weergeven moet zijn ingeschakeld op uw toegangsniveau zodat gebruikers de e-mails van gebruikers kunnen bekijken. Voor informatie, zie [ Toegang van de Verlening tot gebruikers ](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md)
     >

     <!-- this doesn't apply to issues; if it does, add this to the TIP above: 
      ><span class="preview">When adding a job role assignment, you can search for the job role or location. Select a role from the Job roles list to use the default billing rate for the assignment, or select a Rate card job role to use the billing rate from the rate card. For more information on rate cards, see [Manage rate cards](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/manage-rate-cards.md).</span>-->


1. Klik **sparen** om het toewijzen van de kwestie te voltooien.
1. (Facultatief) klik het **pictogram van X** naast de naam van de taken in het gebied van Taken op de kopbal van de kwestie om een taak te verwijderen.

## Een probleem in een lijst toewijzen

U kunt kwesties in een lijst of een rapport toewijzen wanneer om het even welke toewijzingsgebieden in de mening van de lijst zichtbaar zijn. Dit is een snellere manier om problemen toe te wijzen.

Afhankelijk van welk veld zichtbaar is in de weergave, kunt u de volgende entiteiten aan de uitgave toewijzen:

| Optie | Toegewezen entiteiten |
|---|---|
| **toewijzen aan** | Eén gebruiker toewijzen |
| **Toegewezen** | Eén gebruiker toewijzen |
| **Taken** | Wijs gebruikers, baanrollen, of teams toe. |

Om kwesties in een lijst toe te wijzen:

1. Ga naar een lijst met problemen waarvoor de velden Toegewezen aan, Toegewezen of Toewijzingen in de weergave staan.
1. Voer een van de volgende handelingen uit om problemen toe te wijzen:

   * Klik binnen **Toegewezen aan** of **toegewezen** gebieden en begin de naam van een actieve gebruiker te typen die u aan de kwestie wilt toewijzen, dan het te klikken wanneer het in de lijst toont.

     ![ Toegewezen aan gebied ](assets/assigned-to-field-task-list-nwe.png)

   * Klik binnen het **gebied van Taken** en begin de naam van een actieve gebruiker, baanrol, of actief team te typen dat u aan de kwestie wilt toewijzen, dan het klikken wanneer het in de lijst toont.

     <span class="preview"> beeld van de Steekproef in het milieu van de Voorproef:</span>
     ![ het gebied van Taken ](assets/assignments-field-0825.png)

     Voorbeeldafbeelding in de productieomgeving:
     ![ het gebied van Taken ](assets/assignments-field-task-list-0424.png)

   >[!TIP]
   >
   >Wanneer u een gebruikerstoewijzing toevoegt, ziet u de avatar, de primaire rol van de gebruiker of hun e-mailadres om onderscheid te maken tussen gebruikers met identieke namen.
   >
   >Gebruikers moeten aan ten minste één taakrol zijn gekoppeld om deze te kunnen bekijken terwijl u ze toevoegt.
   >
   >De instelling Contactinfo weergeven moet zijn ingeschakeld op uw toegangsniveau zodat gebruikers de e-mails van gebruikers kunnen bekijken. Voor informatie, zie [ toegang van de Verlening tot gebruikers ](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md).

1. (Voorwaardelijk) op het gebied van Taken, klik <span class="preview">**Geavanceerd**</span> of het **pictogram van Mensen** ![ het pictogram van Mensen ](assets/teams.png) in de hoger-juiste hoek van de toewijzingsdoos om de Geavanceerde doos van Toewijzingen te openen en geavanceerde taken tot stand te brengen. Voor meer informatie, zie [ Geavanceerde taken ](../../../manage-work/tasks/assign-tasks/create-advanced-assignments.md) creëren.

   >[!TIP]
   >
   >U kunt geen geavanceerde toewijzingen maken vanuit de velden Toegewezen aan of Toegewezen.

1. Nadat u de toewijzingen aan de uitgave hebt toegevoegd, drukt u op Enter of klikt u ergens op de pagina om de wijzigingen op te slaan.

## Problemen bulksgewijs toewijzen

1. Ga naar een lijst met problemen die u bulksgewijs wilt toewijzen.
1. Selecteer verschillende problemen in de lijst.
1. Klik het **uitgeven pictogram** ![ uitgeven pictogram ](assets/qs-edit-icon.png).

   Het **geeft de dialoogdoos uit van Kwesties** opent.

1. In het **gebied van Taken**, selecteer de **Ontvanger** doos, dan begin de naam van een gebruiker, baanrol, of team te typen die u aan alle kwesties wilt toewijzen.

   >[!IMPORTANT]
   >
   >Als een van de problemen al is toegewezen, worden de bronnen die u hier opgeeft, toegevoegd aan de problemen in plaats van de bestaande bronnen over de problemen te vervangen.

1. (Facultatief) selecteer het radioknoop in de **kolom van de Eigenaar van de Uitgave** om erop te wijzen welke middel de primaire ontvanger of de Eigenaar van de kwestie is, wanneer u meer dan één middel aan de kwestie toewijst. Dit is niet beschikbaar voor teams.
1. (Facultatief) selecteer een rol die de gebruiker op de kwestie van **zou moeten vervullen kies een rol** drop-down menu in de **3} kolom van de Rol van de Ontvanger {wanneer u gebruikers aan kwesties toewijst.** Als u geen rol selecteert, selecteert Workfront automatisch de Primaire Rol van de gebruiker.

1. (Optioneel) Als u bestaande toewijzingen uit alle uitgaven wilt verwijderen, voert u een van de volgende handelingen uit:

   1. Begin de naam van een gebruiker, een rol, of een team te typen u uit de kwestie wilt verwijderen, dan het selecteren wanneer het op de lijst verschijnt en **verwijdert Ontvanger** klikken om extra te verwijderen wijzen toe te voegen.
   1. Klik **verwijderen Alle Bestaande Assignees** om alle toegewezen uit alle geselecteerde kwesties te verwijderen.

1. Klik **sparen Veranderingen**.
1. (Facultatief en voorwaardelijk) wanneer de Toegewezen aan of de gebieden van Taken in uw lijst van kwesties tonen, binnen één van deze kolommen voor een kwestie klikken, dan klik het **X pictogram** naast de naam van een toegewezen om het uit de kwestie te verwijderen.
