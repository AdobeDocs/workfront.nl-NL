---
content-type: reference
product-area: reporting
navigation-topic: calculate-custom-data-reports
title: 'Voorbeeld van berekend aangepast veld: geef de manager van de maker van een uitgave weer op het aangepaste formulier voor uitgave'
description: Met behulp van een berekend aangepast veld kunt u de naam van de beheerder van de maker van een uitgave weergeven op een aangepast formulier dat aan de uitgave is gekoppeld. Met dezelfde instructie kunt u vergelijkbare berekende velden maken voor projecten, problemen en andere objecten.
author: Jenny
feature: Reports and Dashboards
exl-id: f501ce1a-7a80-458b-9b30-2292426c9262
source-git-commit: a1ead6d0c1c85bfbe6d7302506743db8d8b3e205
workflow-type: tm+mt
source-wordcount: '334'
ht-degree: 0%

---

# Voorbeeld van berekend aangepast veld: geef de manager van de maker van een uitgave weer op het aangepaste formulier voor uitgave

Met behulp van een berekend aangepast veld kunt u de naam van de beheerder van de maker van een uitgave weergeven op een aangepast formulier dat aan de uitgave is gekoppeld. Met dezelfde instructie kunt u vergelijkbare berekende velden maken voor projecten, problemen en andere objecten.

<!--outdated link: 
>[!TIP]
>
>For information about additional custom text mode examples from other customers, follow the [Text Mode Reporting](https://one.workfront.com/s/topic/0TO0z000000cdHmGAI/text-mode-reporting?tabset-21363=3) topic on our Community site.
-->

## Toegangsvereisten

+++ Breid uit om de toegangseisen voor de functionaliteit in dit artikel weer te geven.

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

Voor informatie, zie [ vereisten van de Toegang in de documentatie van Workfront ](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## De manager van de maker van een uitgave weergeven op het aangepaste formulier voor uitgave

In de volgende stappen wordt aangegeven hoe u een berekend veld kunt maken voor een aangepaste uitgave waarin u de naam kunt vastleggen van de manager van de gebruiker die de uitgave heeft gemaakt. Het proces is identiek wanneer u de naam van de manager van een gebruiker wilt vangen die een taak, een project, een portefeuille creeerde, bijvoorbeeld.

1. Maak een aangepast formulier voor uitgave en voeg er een berekend veld aan toe.

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

   De manager van de gebruiker die de kwestie creeerde toont op het berekende gebied wanneer de vorm die het gebied bevat aan een kwestie in bijlage is.
