---
title: Financiële machtigingen delen op een object
product-area: projects
navigation-topic: grant-and-request-access-to-objects
description: Uw Adobe Workfront-beheerder kan u toegang verlenen tot financiële gegevens wanneer u uw toegangsniveau toewijst. Zie Toegang tot financiële gegevens verlenen voor meer informatie.
author: Courtney
feature: Get Started with Workfront
exl-id: 0d0e13d9-b234-48d3-a818-5b6fb36a4688
last-update: 2026-04-01T18:03:50Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
source-git-commit: e974adc053a076a4370aa0c4ec41fea700d836be
workflow-type: tm+mt
source-wordcount: '560'
ht-degree: 0%

---

# Financiële machtigingen delen op een object

Uw Adobe Workfront-beheerder kan u toegang verlenen tot financiële gegevens wanneer u uw toegangsniveau toewijst. Voor meer informatie, zie [&#x200B; toegang van de Verlening tot financiële gegevens &#x200B;](../../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md).

Samen met het toegangsniveau dat de gebruikers worden verleend, kunt u hen toestemmingen aan Mening verlenen of financiën voor specifieke projecten, taken, of kwesties beheren die u toegang hebt om te delen.

Voor informatie over welke gebruikers in elk toegangsniveau met financiële gegevens kunnen doen, zie de sectie [&#x200B; Financiële gegevens &#x200B;](../../administration-and-setup/add-users/access-levels-and-object-permissions/functionality-available-for-each-object-type.md#financia) in de artikel [&#x200B; Functionaliteit beschikbaar voor elk objecten type &#x200B;](../../administration-and-setup/add-users/access-levels-and-object-permissions/functionality-available-for-each-object-type.md).

## Toegangsvereisten

<!--
drafted for P&P:

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
   <td> <p>Current license: Standard </p> 
   Or
   <p>Legacy license: Plan </p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>View or higher access to Projects, Tasks, Issues, and Financial  Data</p> <p><b>NOTE</b>
   
   If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can modify your access level, see <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>View permissions or higher to projects, tasks, and issues that include at least View Finance permissions</p> <p>For information on requesting additional access, see <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>
-->

+++ Breid uit om de toegangseisen voor de functionaliteit in dit artikel weer te geven. 

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-pakket</td> 
   <td> <p>Alle</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-licentie</td> 
   <td> <p>Standard</p> 
   <p>Plan</p> 
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraties op toegangsniveau</td> 
   <td> <p>De mening of de hogere toegang tot Projecten, Taken, Kwesties, en Financiële Gegevens</p>  </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objectmachtigingen</td> 
   <td> De toestemmingen van de mening of hoger aan projecten, taken, en kwesties die minstens de het factureringspercentages van de Mening, de kostentarieven van de Mening, en de toestemmingen van de Financiën van de Mening omvatten</td> 
  </tr> 
 </tbody> 
</table>

Voor meer detail over de informatie in deze lijst, zie [&#x200B; vereisten van de Toegang in de documentatie van Workfront &#x200B;](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Een object delen en financiële machtigingen verlenen

Houd rekening met het volgende wanneer u financiële machtigingen toekent aan objecten:

* U kunt financiële toestemmingen aan projecten, taken, en kwesties verlenen.
* De toestemmingen kunnen worden geërft: als u de Toestemmingen van de Financiën van de Mening Algemene van een project hebt, erft u automatisch de toestemmingen van de Financiën van de Mening aan de taken en de kwesties op het project.
* Door machtigingen te verlenen voor facturering en kostentarieven kan de gebruiker de tarieven voor dat object bekijken of bewerken. Met machtigingen tot algemene financiering kan de gebruiker algemene financieringsvelden (die geen verband houden met facturering of kostenpercentages) voor het object bekijken of bewerken.

Financiële machtigingen verlenen aan een object:

1. Ga naar een taak, project, of kwestie die u met anderen wilt delen.
1. Bij de naam van het voorwerp, klik **Aandeel**.

1. In **geef `<Object name>` toegang tot** gebiedsbegin het typen van de naam van een gebruiker, een team, een rol, een groep, of een bedrijf dat u het voorwerp met wilt delen.

   >[!TIP]
   >
   >U kunt een object alleen delen met actieve gebruikers, teams, rollen of bedrijven.

1. Klik op de vervolgkeuzelijst rechts van de gebruikersnaam en selecteer een van de volgende opties:

   * **Mening**
   * **draagt** bij
   * **leiden**

1. Klik in hetzelfde vervolgkeuzemenu op het pictogram Geavanceerde opties naast het machtigingsniveau en voer een van de volgende handelingen uit:

   * Voor om het even welk toestemmingsniveau, uitgezochte **het factureringspercentages van de Mening**, **de kostentarieven van de Mening**, en **de algemene financiering van de Mening** zoals nodig.
   * Voor **beheer** slechts toestemmingen, uitgezocht **het factureren tarieven**, **geeft kostentarieven** uit, en **geeft algemene financiering** zoals nodig uit.

1. Klik **sparen**.

## Financiële toestemming voor alle niveaus voor delen

In de volgende tabel wordt aangegeven welke financiële machtigingen gebruikers krijgen wanneer u hun weergavemachtigingen, Contribute- of beheermachtigingen voor objecten toekent:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th><strong> Acties </strong> </th> 
   <th><strong> leiden </strong> </th> 
   <th><strong> draagt </strong> bij </th> 
   <th><strong> Mening </strong> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>Factureringsrecords beheren</td> 
   <td>✓</td> 
   <td> <p>  </p> </td> 
   <td>  </td> 
  </tr> 
  <tr> 
   <td>Factureringssnelheden bewerken</td> 
   <td>✓</td> 
   <td></td> 
   <td>  </td> 
  </tr> 
  <tr> 
   <td>Kostentarieven bewerken</td> 
   <td>✓</td> 
   <td></td> 
   <td>  </td> 
  </tr>  
  <tr> 
   <td>Algemene financiën bewerken</td> 
   <td>✓</td> 
   <td></td> 
   <td>  </td> 
  </tr>
  <tr> 
   <td>Factureringssnelheden weergeven</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>  ✓</td> 
  </tr> 
  <tr> 
   <td>Kostentarieven weergeven</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>  ✓</td> 
  </tr>  
  <tr> 
   <td>Algemene financiën weergeven</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>  ✓</td> 
  </tr> 
  <tr> 
   <td>De informatie van de mening door Kosten in de hulpmiddelen van de Planning van het Middel</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>De middelen van de begroting in de hulpmiddelen van de Planning van Middelen*</td> 
   <td>✓</td> 
   <td>  </td> 
   <td>  </td> 
  </tr> 
  <tr> 
   <td>De middelen van de mening in de hulpmiddelen van de Planning van het Middel*</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td> <p>✓</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42; vereist de extra toegang van het Beheer van het Middel.

Voor informatie over de toegang van het Beheer van het Middel, zie [&#x200B; Toegang van de Verlening tot het Beheer van het Middel &#x200B;](../../administration-and-setup/add-users/configure-and-grant-access/grant-access-resource-management.md).

<!--
These rows removed from last table.

  <tr> 
   <td>Manage/ View Role Billing and Cost Rates</td> 
   <td>✓</td> 
   <td>  </td> 
   <td>  </td> 
  </tr> 
  <tr> 
   <td>Manage/ View User Billing and Cost Rates</td> 
   <td>✓</td> 
   <td>  </td> 
   <td>  </td> 
  </tr> 

-->
