---
user-type: administrator
product-area: system-administration;user-management
navigation-topic: manage-group-statuses
title: De status van een groep maken of bewerken
description: Als groepsbeheerder kunt u aangepaste statussen maken voor een groep die u beheert. Dit helpt de behoefte aan tientallen bedrijfs-brede douanestatus elimineren en staat meer autonomie in uw groepshiërarchieën toe.
author: Becky
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: 75018e0e-ff74-4afb-9a99-34bbb39b6e14
source-git-commit: f1e945ca2508fc7ae1feaa5e97677458d175212f
workflow-type: tm+mt
source-wordcount: '1321'
ht-degree: 0%

---

# Een groepsstatus maken of bewerken

Als groepsbeheerder kunt u aangepaste statussen maken voor een groep die u beheert. Dit helpt de behoefte aan tientallen bedrijfs-brede douanestatus elimineren en staat meer autonomie in uw groepshiërarchieën toe.

U kunt ook een status op systeemniveau bewerken voor een groep die u beheert als een Workfront-beheerder de status heeft ontgrendeld. Voor meer informatie, zie [&#x200B; Vergrendelde en ontgrendelde systeem-vlakke statussen &#x200B;](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/lock-or-unlock-a-custom-system-level-status.md).

Als er om het even welke groepen boven uw groep zijn, kunnen hun beheerders deze dingen voor uw groep ook doen. Hetzelfde geldt voor Workfront-beheerders (voor elke groep).

>[!NOTE]
>
>De de groepsstatussen van de douane kunnen niet op een project worden getoond wanneer het bekijken van het project in een Gelijke mening. Alleen standaard- en aangepaste vergrendelde statussen zijn zichtbaar wanneer een project in een flexibele weergave wordt weergegeven. Voor informatie over het aanpassen van een Gelijke mening voor een project, zie de sectie [&#x200B; creëren of aanpassen een Gelijke mening &#x200B;](/help/quicksilver/reports-and-dashboards/reports/reporting-elements/create-edit-views.md#create-or-customize-an-agile-view) in het artikel [&#x200B; creeert of geeft meningen in Adobe Workfront &#x200B;](/help/quicksilver/reports-and-dashboards/reports/reporting-elements/create-edit-views.md) uit.

Voor algemene informatie over statussen, zie [&#x200B; Overzicht van Statussen &#x200B;](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/statuses-overview.md).

## Toegangsvereisten

+++ Breid uit om de toegangseisen voor de functionaliteit in dit artikel weer te geven.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Adobe Workfront-pakket</td> 
   <td><p>Alle</p></td> 
  </tr> 
  <tr> 
   <td>Adobe Workfront-licentie</td> 
   <td><p>Standard</p>
       <p>Plan</p></td>
  </tr>
  <tr> 
   <td>Configuraties op toegangsniveau</td> 
   <td>U moet een groepsbeheerder van de groep of een systeembeheerder zijn.</td>
  </tr>
 </tbody> 
</table>

Voor informatie, zie [&#x200B; vereisten van de Toegang in de documentatie van Workfront &#x200B;](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Een status voor een groep maken of bewerken

{{step-1-to-setup}}

1. In het linkerpaneel, klik **Groepen** ![&#x200B; Groepen &#x200B;](assets/groups-icon.png).

1. Klik op de naam van de groep waar u statussen wilt maken of aanpassen.
1. In het linkerpaneel, klik **Statussen**.

   Als de groep die u bekijkt een groep op hoofdniveau is, bevat de lijst die wordt weergegeven het volgende:

   * Vergrendelde status op systeemniveau.
   * Aangepaste statussen die al voor de groep zijn gemaakt.

   Als de groep die u bekijkt een subgroep is, bevat de lijst ook:

   * Vergrendelde statussen die tot de groepen boven de subgroep behoren.
   * Ontgrendelde statussen die bij het maken van de subgroep behoorden tot de groepen boven de subgroep.

     Nadat een subgroep is gemaakt, worden ontgrendelde statussen die in de bovenstaande groepen zijn gemaakt, niet opgenomen in de statuslijst van de subgroep. Nochtans, als iemand één van hen later sluit, wordt het dan inbegrepen in de de statuslijst van subgroup. Voor meer informatie, zie [&#x200B; Hoe de groepen statussen &#x200B;](../../../administration-and-setup/manage-groups/manage-group-statuses/how-groups-inherit-statuses.md) erven.

1. Selecteer het lusje van het objecten type (**Project**, **Taken**, of **Kwesties**) dat u met de status wilt associëren.

1. (Voorwaardelijk) als de status een uitgevende status is, zorg ervoor dat **Hoofdlijst** wordt geselecteerd.

   ![&#x200B; Hoofdlijst &#x200B;](assets/master-list.png)

   Voor informatie over het aanpassen van de andere uitgevende types (het Rapport van de Bug, de Orde van de Verandering, Uitgave, Verzoek), zie [&#x200B; standaardkwesties &#x200B;](../../../administration-and-setup/set-up-workfront/configure-system-defaults/customize-default-issue-types.md) aanpassen.

1. (Voorwaardelijk) om een nieuwe status tot stand te brengen, klik **voeg een Nieuwe Status** toe.

   of

   Om een bestaande status uit te geven, muis over de status u wilt uitgeven, dan klik **uitgeven** optie die aan uiterst rechts toont.

   ![&#x200B; status van de Groep &#x200B;](assets/group-statuses-edit.jpg)

   >[!NOTE]
   >U kunt een status voor uw groep alleen bewerken als:
   >      
   >* U beheert de groep waarvoor de status is gemaakt
   >* Een Workfront-beheerder heeft de status op systeemniveau ontgrendeld
   >* Een groepsbeheerder van een groep boven uw groep ontgrendelde de status
   >      
   >      
   >Wanneer u een bestaande status bewerkt, kunt u alleen de naam, beschrijving en kleur van die status wijzigen.
   >
   >Wanneer u een vergrendelde status bewerkt, zijn de wijzigingen van toepassing op alle subgroepen die de status van uw groep hebben overgenomen.
   >   
   >Omgekeerd heeft het bewerken van een ontgrendelde status geen invloed op de subgroepen die de status van de groep hebben overgenomen.

1. Geef de volgende informatie op.

   Als u een status bewerkt, kunnen alleen de eerste 3 instellingen worden gewijzigd.

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Statusnaam</td> 
      <td> <p>Typ een naam voor de status. Dit is een verplicht veld.</p> <p>Wanneer u een statusnaam maakt, moet u er rekening mee houden dat anderen in het systeem een status met dezelfde naam kunnen maken. We raden u aan een unieke naam te gebruiken om verwarring te voorkomen bij het selecteren van statussen in Workfront.</p><p>Als er dubbele statussen bestaan, moet de groepsbeheerder de namen bijwerken om ze van elkaar te onderscheiden. De enige unieke indicator in het systeem is de status Key.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Beschrijving</td> 
      <td>(Optioneel) Typ een beschrijving van de status. Dit deelt zijn doel aan degenen mee die het gebruiken.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Kleur</td> 
      <td> <p>Pas de kleur van de status aan door te klikken op het kleurveld en een kleur te selecteren in het deelvenster Stalen. U kunt ook een hexadecimaal getal in het veld invoeren.</p> <p>De statuskleur wordt in de rechterbovenhoek van Workfront weergegeven wanneer een gebruiker het object bekijkt.</p> <p> <img src="assets/status-color.png"> </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Vergelijkt met</td> 
      <td> <p>Selecteer een van de opties in de lijst die de functie van de status het best beschrijft. Als de statusnaam bijvoorbeeld Gereed is, moet de optie waarmee deze overeenkomt voltooid zijn.</p> <p>Elke status moet overeenkomen met een van deze opties, omdat dit bepaalt hoe de status werkt.</p> <p>Deze optie kan niet worden gewijzigd nadat de status is gemaakt.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Sleutel</td> 
      <td> <p>Als u een nieuwe status maakt, typt u een code of afkorting voor de status of gebruikt u de code die voor u is gegenereerd. Deze sleutel moet uniek zijn in Workfront omdat deze kan worden gebruikt voor rapportagedoeleinden. Als u een toets probeert op te geven die al in gebruik is in het systeem, wordt het veld rood.</p> <p>Het zou nuttig kunnen zijn om een afkorting te gebruiken die voor degenen herkenbaar is die het zullen gebruiken.</p> <p>Deze optie kan niet worden gewijzigd nadat de status is gemaakt.</p> <p>U kunt de toetscode voor de statussen Planning, Huidig en Voltooid niet wijzigen. Dit is belangrijk als u een rapport opstelt in de tekstmodus.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Status verbergen</td> 
      <td> <p>(Alleen status van project en taak)</p> <p>Schakel deze optie in als u de status wilt verbergen voor gebruikers. Wanneer deze is uitgeschakeld (de standaardinstelling), kunnen alle subgroepen onder de groep de status gebruiken.</p> <p>Tip: U kunt de status van een probleem verbergen door alle vier de typen problemen uit te schakelen (Foutenrapport, Wijzigingsvolgorde, Uitgave, Verzoek).</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Vergrendelen voor alle groepen</td> 
      <td> 
       <p>Als u deze optie ingeschakeld laat, kunnen de gebruikers in uw groep en de subgroepen de status zien en gebruiken en kunnen groepsbeheerders de status niet aanpassen voor lagere subgroepen.</p> 
       <p>Als deze optie is uitgeschakeld, kunnen groepsbeheerders de status voor lagere subgroepen aanpassen.</p> 
       <p><b> NOTA </b>: U kunt zowel gesloten als ontgrendelde statussen in een proces van de groepsgoedkeuring gebruiken. Als u een proces van de groepsgoedkeuring met een ontgrendelde groepsstatus creeert, kunnen de gebruikers het goedkeuringsproces aan om het even welk project, taak, of kwestie vastmaken die met de groep wordt geassocieerd.</p> 
       <p>Voor meer informatie over het sluiten van statussen, zie <a href="../../../administration-and-setup/manage-groups/manage-group-statuses/lock-or-unlock-a-custom-group-status.md" class="MCXref xref"> Vergrendelde en ontgrendelde groepsstatussen </a>.</p> 
       </td> 
     </tr>
    </tbody> 
   </table>

1. Klik **sparen**.

   De status is nu beschikbaar voor alle projecten die aan uw groep of subgroep zijn gekoppeld. Als u deze hebt vergrendeld, kunt u deze gebruiken door lagere subgroepen.

   U kunt de status zo configureren dat deze een standaardstatus voor de groep is. Voor meer informatie, zie [&#x200B; Gebruik een douanestatus als standaardstatus voor een groep &#x200B;](../../../administration-and-setup/manage-groups/manage-group-statuses/use-custom-statuses-as-default-statuses-group.md).

## Een aangepaste status maken voor meerdere groepen

Als u een Workfront-beheerder bent, kunt u een aangepaste status voor meerdere groepen maken door een status voor het hele systeem te maken en die status vervolgens te verbergen voor groepen die deze status niet nodig hebben.

Als u een groepsbeheerder (of een beheerder van Workfront) bent, kunt u een douanestatus voor veelvoudige subgroepen binnen een groepshiërarchie tot stand brengen u door een status voor een hogere niveaugroep te creëren beheert, dan het verbergen van die status voor lagere subgroepen die het niet nodig hebben.

1. Als u een beheerder van Workfront bent, creeer een systeem-brede ontgrendelde status zoals die in [&#x200B; wordt beschreven creeer of geef een status &#x200B;](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-or-edit-a-status.md) uit.
1. In de doos in de hoger-juiste hoek, schrap **Statussen van het Systeem**, begin typend de naam van een groep waar u de status wilt verbergen, dan klik de naam wanneer het verschijnt.
1. Beweeg over de status u van de groep wilt verbergen, dan **&#x200B;**&#x200B;klikken uitgeven wanneer het verschijnt.

   ![&#x200B; geeft status &#x200B;](assets/hover-click-edit.jpg) uit

1. Laat de **optie van de Status van de Verbergen** toe die verschijnt.

   ![&#x200B; de status van de Huid &#x200B;](assets/hide-group-status.png)

1. Klik **sparen**.

   De status wordt grijs weergegeven en is niet meer zichtbaar voor alle gebruikers in die groep.

1. Herhaal stap 3 tot en met 5 om de aangepaste status te verbergen voor andere groepen die deze niet nodig hebben.

