---
product-previous: workfront-goals
product-area: projects
navigation-topic: results-and-activities
title: Resultaten toevoegen aan doelen in Adobe Workfront-doelen
description: De resultaten meten de vooruitgang van een doel. Zonder resultaten, activiteiten of uitgelijnde doelen aan een doel te koppelen, kunt u het doel niet activeren en kunt u de voortgang niet vastleggen.
author: Alina
feature: Workfront Goals
exl-id: 30e22482-22e2-432d-bb73-7f9a9160aba2
source-git-commit: afc2124a7fd0d9d52c04be1c174fdba314beec7a
workflow-type: tm+mt
source-wordcount: '534'
ht-degree: 0%

---

# Resultaten toevoegen aan doelen in Adobe Workfront-doelen

De resultaten meten de vooruitgang van een doel. Zonder resultaten, activiteiten of uitgelijnde doelen aan een doel te koppelen, kunt u het doel niet activeren en kunt u de voortgang niet vastleggen.

## Toegangsvereisten

<!--drafted for P&P release: 

<table style="table-layout:auto">
 <col>
 </col>
 <col>
 </col>
 <tbody>
  <tr>
   <td role="rowheader">Adobe Workfront plan*</td>
   <td>
   <p>Current plan: Select or higher</p>
   Or
   <p>Legacy plan: Pro or higher</p>
   
   </td>
  </tr>
  <tr>
   <td role="rowheader">Adobe Workfront license*</td>
   <td>
   <p>Current license: Contributor or higher</p>
   Or
   <p>Legacy license: Request or higher</p> <p>For more information, see <a href="../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref">Adobe Workfront licenses overview</a>.</p> </td>
  </tr>
  <tr>
   <td role="rowheader">Product</td>
   <td>
   <p> Current product requirement: If you have the Select or Prime Adobe Workfront plan, you must also buy an additional Adobe Workfront Goals license.  Workfront Goals are included in the Ultimate Workfront Plan.</p>
   Or
   <p>Legacy product requirement: You must purchase an additional license for the Adobe Workfront Goals to access functionality described in this article. </p> <p>For information, see <a href="../../workfront-goals/goal-management/access-needed-for-wf-goals.md" class="MCXref xref">Requirements to use Workfront Goals</a>. </p> </td>
  </tr>
  <tr>
   <td role="rowheader">Access level*</td>
   <td> <p>Edit access to Goals</p> <p><b>NOTE</b><p>If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can change your access level, see:</p>
     <ul>
      <li> <p><a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a> </p> </li>
      <li> <p><span href="../../administration-and-setup/add-users/configure-and-grant-access/grant-access-goals.md"><a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-access-goals.md" class="MCXref xref">Grant access to Adobe Workfront Goals</a></span> </p> </li>
     </ul> </p> </td>
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
 </tbody>
</table>

-->

U moet het volgende hebben:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-abonnement*</td> 
   <td> <p>Pro of hoger</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-licentie*</td> 
   <td> <p>Aanvraag of hoger</p> <p>Zie voor meer informatie <a href="../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref">Overzicht van Adobe Workfront-licenties</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Product</td> 
   <td> <p>U moet een extra licentie voor de Adobe Workfront Goals aanschaffen om toegang te krijgen tot de functionaliteit die in dit artikel wordt beschreven. </p> <p>Zie voor meer informatie <a href="../../workfront-goals/goal-management/access-needed-for-wf-goals.md" class="MCXref xref">Vereisten voor het gebruik van Workfront-doelen</a>. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraties op toegangsniveau*</td> 
   <td> <p>Toegang tot doelen bewerken</p> <p><b>OPMERKING</b>

<p>Als u nog steeds geen toegang hebt, vraagt u de Workfront-beheerder of deze aanvullende beperkingen op uw toegangsniveau instelt. Voor informatie over hoe een beheerder van Workfront uw toegangsniveau kan veranderen, zie:</p> 
     <ul> 
      <li> <p><a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Aangepaste toegangsniveaus maken of wijzigen</a> </p> </li> 
      <li> <p><span href="../../administration-and-setup/add-users/configure-and-grant-access/grant-access-goals.md"><a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-access-goals.md" class="MCXref xref">Toegang tot Adobe Workfront-doelen verlenen</a></span> </p> </li> 
     </ul> </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">Objectmachtigingen</td> 
   <td> 
    <div> 
     <p>Rechten voor het doel beheren</p> 
     <p>Voor informatie over het delen van doelstellingen, zie <a href="../../workfront-goals/workfront-goals-settings/share-a-goal.md" class="MCXref xref">Een doel delen in Workfront-doelen</a>. </p> 
    </div> </td> 
  </tr> 
 </tbody> 
</table>

*Neem contact op met uw Workfront-beheerder om te weten te komen welk abonnement, licentietype of toegang u hebt.

## Vereisten

U moet het volgende hebben voordat u kunt beginnen:

* Een lay-outsjabloon die het gebied Doelen in het hoofdmenu bevat.
* Een bestaand doel.

   Voor informatie over het creëren van doelstellingen, zie [Doelen maken voor Adobe Workfront-doelen](../../workfront-goals/goal-management/create-goals.md).

>[!IMPORTANT]
>Een doel kan niet meer dan 1000 activiteiten, resultaten, projecten, of gerichte doelstellingen hebben.

## Een resultaat toevoegen aan een doel

<!--

Adding results to goals differs depending on which environment you use.

### Add a result to a goal in the Production environment

1. Go to the goal for which you want to add a result and click the name to open the **Goal Details** panel.
1. Click **Add results**.

   ![](assets/add-result-inside-goal-details-highlighted-350x145.png)

1. Start typing the result you want to achieve in the **Result** field. This is the name of the result and it displays wherever the goal displays. 
1. (Optional) If you want to set the Result Owner as someone other than yourself, click your name in the **Owner** field and start typing the name of the user that you want to assign as the owner of the result, then click it when it appears in the drop-down list.

   >[!NOTE]
   >
   >You cannot assign a team or group as a result owner.

1. In the Value drop-down menu, select the type of value that you want to measure your success by.

   ![](assets/results-value-initial-target-boxes-350x49.png)

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

1. Klik op het hoofdmenu ![](assets/main-menu-icon.png)vervolgens **Doelen**.

1. Van de **Lijst met doelen** klikt u op de naam van een doel om de doelpagina te openen.
1. Klikken **Voortgangsindicatoren** in het linkerdeelvenster.
1. Breid uit **Nieuwe voortgangsindicator** vervolgkeuzemenu en vervolgens op **Resultaat maken**.

   Het vak Nieuw resultaat wordt geopend.

   ![](assets/new-result-box-unshimmed.png)

1. Voer een naam in voor het resultaat in het dialoogvenster **Resultaatnaam** veld. Dit is een verplicht veld.
1. (Optioneel) Verwijder uw naam uit het dialoogvenster **Resultaateigenaar** veld als u het resultaat aan een andere gebruiker wilt toewijzen. Standaard bent u de eigenaar van een activiteit die u maakt.

   >[!NOTE]
   >
   >U kunt geen team, groep, of het bedrijf als resultaateigenaar toewijzen.

1. In de **Hoe wilt u het resultaat meten?** in het gebied, geeft u de volgende informatie op:
   * **Type waarde**: Dit geeft aan hoe u de voortgang van het resultaat wilt meten. U kunt de voortgang numeriek meten met een percentage of met een valutabedrag.

      Selecteer een waardetype van de opties die in de volgende lijst worden vermeld:

      | Type waarde | Beschrijving |
      |---------------------------------------------------------|------------------|
      | Getal | Nummerwaarde |
      | % | Waarde percentage |
      | CN ¥,DKK,KR,Mex$, R, R$, zł, ¥ , € , ₹, ฿, MYR, ₪, $ | Valuta |

   * **Beginwaarde**: De waarde die het resultaat in het begin heeft, voordat er enige voortgang is opgenomen.
   * **Doelwaarde**: De waarde die het resultaat beoogt te bereiken wanneer het als voltooid wordt beschouwd.
1. Klikken **Resultaat maken**.

   Het resultaat wordt weergegeven in de sectie Voortgangsindicatoren van de doelpagina, onder de resultatengroep.

   Nadat u het doel hebt geactiveerd, wordt de voortgang van het doel automatisch bijgewerkt wanneer u de voortgang van een resultaat bijwerkt. Voor informatie over het activeren van een doel raadpleegt u [Doelen in Adobe Workfront-doelen activeren](../goal-management/activate-goals.md).
