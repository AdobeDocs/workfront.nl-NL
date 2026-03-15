---
content-type: reference
product-area: reporting
navigation-topic: calculate-custom-data-reports
title: 'Voorbeeld van berekende aangepaste velden: geef de manager van de maker van een uitgave weer voor het aangepaste formulier voor de uitgave'
description: Met behulp van een berekend aangepast veld kunt u de naam van de manager van de maker van een uitgave weergeven op een aangepast formulier dat is gekoppeld aan de uitgave. Met dezelfde instructie kunt u vergelijkbare berekende velden voor projecten, uitgaven en andere objecten maken.
author: Courtney
feature: Reports and Dashboards
exl-id: f501ce1a-7a80-458b-9b30-2292426c9262
source-git-commit: 4261febe4af8628508083fa18e4767e3fd3e1136
workflow-type: tm+mt
source-wordcount: '334'
ht-degree: 0%

---

# Voorbeeld van berekende aangepaste velden: geef de manager van de maker van een uitgave weer voor het aangepaste formulier voor de uitgave

Met behulp van een berekend aangepast veld kunt u de naam van de manager van de maker van een uitgave weergeven op een aangepast formulier dat is gekoppeld aan de uitgave. Met dezelfde instructie kunt u vergelijkbare berekende velden maken voor projecten, problemen en andere objecten.

<!--outdated link: 
>[!TIP]
>
>For information about additional custom text mode examples from other customers, follow the [Text Mode Reporting](https://one.workfront.com/s/topic/0TO0z000000cdHmGAI/text-mode-reporting?tabset-21363=3) topic on our Community site.
-->

## Toegangsvereisten

+++ Vouw uit om de toegangsvereisten voor de functionaliteit in dit artikel weer te geven.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p>Adobe Workfront-pakket</p> </td> 
   <td><p>Alle</p></td> 
  </tr> 
  <tr> 
   <td> <p>Adobe Workfront-licentie</p> </td> 
   <td>
      <p>Standard</p>
      <p>Plan</p></td>
  </tr> 
  <tr> 
   <td><p>Configuraties op toegangsniveau</p></td> 
   <td> <p>Administratieve toegang tot aangepaste formulieren</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Objectmachtigingen</p> </td> 
   <td> <p>Contribute opent het object waaraan het formulier is gekoppeld met toegang tot het aangepaste formulier bewerken</p></td> 
  </tr> 
 </tbody> 
</table>

Voor informatie, zie [&#x200B; vereisten van de Toegang in de documentatie van Workfront &#x200B;](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## De manager van de maker van een uitgave weergeven op het aangepaste formulier voor de uitgave

In de volgende stappen wordt aangegeven hoe u een berekend veld kunt maken voor een formulier dat is aangepast aan de uitgave, waarin u de naam kunt vastleggen van de manager van de gebruiker die de uitgave heeft gemaakt. Het proces is identiek wanneer u de naam wilt vastleggen van de manager van een gebruiker die bijvoorbeeld een taak, project of portfolio heeft gemaakt.

1. Maak een formulier dat is aangepast aan de uitgave en voeg er een berekend veld aan toe.

   Zie de volgende artikelen voor informatie over het maken van een aangepast formulier en het toevoegen van berekende velden aan dit formulier:

   * [Een aangepast formulier maken](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md)
   * [Berekende velden toevoegen aan een formulier](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/add-a-calculated-field.md)

1. Kopieer en kleef de volgende code van de tekstwijze in het **gebied van de Berekening** van de douanevorm:

   ```
   {owner}.{manager}.{name}
   ```

   >[!TIP]
   >
   >Berekeningen van aangepaste velden zijn hoofdlettergevoelig.

1. Klik **Gedaan**, dan **sparen + Sluiten**.

   De manager van de gebruiker die de uitgave heeft gemaakt, wordt in het berekende veld weergegeven wanneer het formulier dat het veld bevat, aan een uitgave is gekoppeld.
