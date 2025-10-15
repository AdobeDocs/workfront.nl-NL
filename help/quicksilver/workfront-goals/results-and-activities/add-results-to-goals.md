---
product-previous: workfront-goals
product-area: projects
navigation-topic: results-and-activities
title: Resultaten toevoegen aan doelen in Adobe Workfront-doelen
description: De resultaten meten de vooruitgang van een doel. Zonder resultaten, activiteiten of uitgelijnde doelen aan een doel te koppelen, kunt u het doel niet activeren en kunt u de voortgang niet vastleggen.
author: Alina
feature: Workfront Goals
exl-id: 30e22482-22e2-432d-bb73-7f9a9160aba2
source-git-commit: 4ef71db5d93e314b746e8acdbf90fd041c6e71ae
workflow-type: tm+mt
source-wordcount: '527'
ht-degree: 0%

---

# Resultaten toevoegen aan doelen in Adobe Workfront-doelen

<!--Audited for P&P only: 10/2025-->

De resultaten meten de vooruitgang van een doel. Zonder resultaten, activiteiten of uitgelijnde doelen aan een doel te koppelen, kunt u het doel niet activeren en kunt u de voortgang niet vastleggen.

## Toegangsvereisten

>[!NOTE]
>
>Uw bedrijf zou kunnen verkiezen om de Doelen van Adobe Workfront verder te gebruiken als zij dit pakket in het verleden kochten. U moet voor meer informatie contact opnemen met uw accountvertegenwoordiger.
>
>Adobe Workfront Goals kan niet meer worden aangeschaft.

+++ Breid uit om de toegangseisen voor de functionaliteit in dit artikel weer te geven. 

<table style="table-layout:auto">
<col>
</col>
<col>
</col>
<tbody>
 <tr>
  <td> <p>Adobe Workfront-pakket</p> </td> 
   <td> 
   <p>Adobe Workfront Ultimate</p>
   </td> 
  </tr>
 <tr>
 <td role="rowheader">Adobe Workfront-licentie</td>
 <td>
 <p>Medewerker of hoger</p>
<p>Aanvraag of hoger</p></td>
 </tr>
  <tr>
 <td role="rowheader">Configuratie op toegangsniveau</td>
 <td> <p>Toegang tot doelen bewerken</p> </td>
 </tr>
 <tr data-mc-conditions="">
 <td role="rowheader">Objectmachtigingen</td>
 <td>
  <div>
  <p>De toestemmingen van de mening of hoger aan het doel om het te bekijken</p>
  <p>Machtigingen beheren om het te bewerken</p>
  </div> </td>
 </tr>
<tr>
   <td role="rowheader"><p>Lay-outsjabloon</p></td>
   <td> <p>Aan alle gebruikers, inclusief Systeembeheerders, moet een lay-outsjabloon worden toegewezen die het gebied Doelen in het hoofdmenu bevat. </p>  
</td>
  </tr>
</tbody>
</table>

Voor meer informatie, zie [&#x200B; vereisten van de Toegang in de documentatie van Workfront &#x200B;](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

<!--Old:

<table style="table-layout:auto">
<col>
</col>
<col>
</col>
<tbody>
 <tr> 
   <td role="rowheader">Adobe Workfront plan*</td> 
   <td> 
   <p>For the new plan and license structure:
  <ul><li>An Ultimate plan </li></ul>
   </p>
<p>For the current plan and license structure: 
<ul><li> A Pro or higher </li>
  <li>An Adobe Workfront Goals license in addition to a Workfront license.</li></ul></p>
   </td> 
  </tr>
 <tr>
 <td role="rowheader">Adobe Workfront license*</td>
 <td>
 <p>New license: Contributor or higher</p>
 Or
 <p>Current license: Request or higher</p> <p>For more information, see <a href="../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref">Adobe Workfront licenses overview</a>.</p> </td>
 </tr>
 <tr>
 <td role="rowheader">Product*</td>
 <td>
 <p> New product requirement, one of the following: </p>
<ul>
<li>A Select or Prime Adobe Workfront plan and an additional Adobe Workfront Goals license.</li>
<li>An Ultimate Workfront plan which includes Workfront Goals by default. </li></ul>
 <p>Or</p>
 <p>Current product requirement: A Workfront plan and an additional license for Adobe Workfront Goals. </p> <p>For information, see <a href="../../workfront-goals/goal-management/access-needed-for-wf-goals.md" class="MCXref xref">Requirements to use Workfront Goals</a>. </p> </td>
 </tr>
 <tr>
 <td role="rowheader"><p>Access level</p></td>
 <td> <p>Edit access to Goals</p>  </td>
 </tr>
 <tr data-mc-conditions="">
 <td role="rowheader">Object permissions</td>
 <td>
  <div>
  <p>View or higher permissions to the goal to view it</p>
  <p>Manage permissions to the goal to edit it</p>
  <p>For information about sharing goals, see <a href="../../workfront-goals/workfront-goals-settings/share-a-goal.md" class="MCXref xref">Share a goal in Workfront Goals</a>. </p>
  </div> </td>
 </tr>
 <tr>
   <td role="rowheader"><p>Layout template</p></td>
   <td> <p>All users, including Workfront administrators,  must be assigned a layout template that includes the Goals area in the Main Menu. </p>  
</td>
  </tr>
</tbody>
</table>-->

## Vereisten

U moet het volgende hebben voordat u kunt beginnen:

* Een lay-outsjabloon die het gebied Doelen in het hoofdmenu bevat.
* Een bestaand doel.

  Voor informatie over het creëren van doelstellingen, zie [&#x200B; doelstellingen in de Doelen van Adobe Workfront &#x200B;](../../workfront-goals/goal-management/create-goals.md) creëren.

>[!IMPORTANT]
>Een doel kan niet meer dan 1000 activiteiten, resultaten, projecten, of gerichte doelstellingen hebben.

## Een resultaat toevoegen aan een doel

<!--

Adding results to goals differs depending on which environment you use.

### Add a result to a goal in the Production environment

1. Go to the goal for which you want to add a result and click the name to open the **Goal Details** panel.
1. Click **Add results**.

   ![Add result inside goal](assets/add-result-inside-goal-details-highlighted-350x145.png)

1. Start typing the result you want to achieve in the **Result** field. This is the name of the result and it displays wherever the goal displays. 
1. (Optional) If you want to set the Result Owner as someone other than yourself, click your name in the **Owner** field and start typing the name of the user that you want to assign as the owner of the result, then click it when it appears in the drop-down list.

   >[!NOTE]
   >
   >You cannot assign a team or group as a result owner.

1. In the Value drop-down menu, select the type of value that you want to measure your success by.

   ![Results value](assets/results-value-initial-target-boxes-350x49.png)

   Select from the following options:

   |Option|Value type|
   |---|---|
   | # |Number value |
   | % |Percentage value |
   |$, CN¥, DKK, KR, Mex$, R, R$, zł, £ , ¥ , &euro; , ₹, ฿, MYR, ₪  |Currency values |

   For example, if you want to increase profit to 8%, and profit is currently at 4%, you can select % as the Measured Value.

   >[!TIP]
   >
   >The result Type is always Metric and cannot be edited.

1. In the Initial field, indicate the value that the result has in the beginning, before any progress on it has been recorded. For example, if you want to increase profit to 8%, and profit is currently at 4%, you can enter 4 as the Starting At value. 
1. In the Target field, indicate the value that the result aims to achieve. For example, if you want to increase profit to 8%, and profit is currently at 4%, you can enter 8 as the Ending At value.
1. Click **Save**.

   The result is saved for the selected goal. The progress of the goal automatically updates when you update the progress of a result.

-->

1. Klik het Belangrijkste pictogram van het Menu ![&#x200B; Hoofd &#x200B;](assets/main-menu-icon.png), toen **Doelen**.

1. Van de **Lijst van het Doel**, klik de naam van een doel om de doelpagina te openen.
1. Klik **indicatoren van de Voortgang** in het linkerpaneel.
1. Vouw de **Nieuwe voortgangsindicator** drop-down menu uit, dan klik **creeer resultaat**.

   Het vak Nieuw resultaat wordt geopend.

   ![&#x200B; Nieuwe resultaatdoos &#x200B;](assets/new-result-box-unshimmed.png)

1. Ga een naam voor het resultaat in het **gebied van de Naam van het Resultaat** in. Dit is een verplicht veld.
1. (Facultatief) verwijder uw naam uit het **gebied van de resultaateigenaar** als u het resultaat aan een andere gebruiker wilt toewijzen. Standaard bent u de eigenaar van een activiteit die u maakt.

   >[!NOTE]
   >
   >U kunt geen team, groep, of het bedrijf als resultaateigenaar toewijzen.

1. In **hoe wilt u uw resultaat meten?** , geeft u de volgende informatie op:
   * **Type van Waarde**: Dit wijst erop hoe u de vooruitgang op het resultaat wilt meten. U kunt de voortgang numeriek meten met een percentage of met een valutabedrag.

     Selecteer een waardetype van de opties die in de volgende lijst worden vermeld:

     | Type waarde | Beschrijving |
     |---------------------------------------------------------|------------------|
     | Getal | Nummerwaarde |
     | % | Waarde percentage |
     | CN ¥,DKK,KR,Mex$, R, R$, zł, ¥ , € , ₹, ฿, MYR, ₪, $ | Valuta |

   * **Aanvankelijke Waarde**: De waarde die het resultaat in het begin heeft, alvorens om het even welke vooruitgang op het is geregistreerd.
   * **Waarde van het Doel**: De waarde die het resultaat probeert te bereiken wanneer het wordt beschouwd als voltooid.
1. Klik **creeer resultaat**.

   Het resultaat wordt weergegeven in de sectie Voortgangsindicatoren van de doelpagina, onder de resultatengroep.

   Nadat u het doel hebt geactiveerd, wordt de voortgang van het doel automatisch bijgewerkt wanneer u de voortgang van een resultaat bijwerkt. Voor informatie over het activeren van een doel, zie [&#x200B; doelstellingen in de Doelen van Adobe Workfront &#x200B;](../goal-management/activate-goals.md) activeren.
