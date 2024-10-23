---
content-type: reference
product-area: reporting
navigation-topic: calculate-custom-data-reports
title: "Voorbeeld van berekend aangepast veld: geef de manager van de maker van een uitgave weer op het aangepaste formulier voor uitgave"
description: Met behulp van een berekend aangepast veld kunt u de naam van de beheerder van de maker van een uitgave weergeven op een aangepast formulier dat aan de uitgave is gekoppeld. Met dezelfde instructie kunt u vergelijkbare berekende velden maken voor projecten, problemen en andere objecten.
author: Nolan
feature: Reports and Dashboards
exl-id: f501ce1a-7a80-458b-9b30-2292426c9262
source-git-commit: 7697327455a7ffdc1a15bfa1676c3a0b091abd04
workflow-type: tm+mt
source-wordcount: '410'
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

U moet de volgende toegang hebben om de stappen in dit artikel uit te voeren:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p>Adobe Workfront-abonnement*</p> </td> 
   <td>Alle</td> 
  </tr> 
  <tr> 
   <td> <p>Adobe Workfront-licentie*</p> </td> 
   <td> <p>Plan </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>Configuraties op toegangsniveau*</td> 
   <td> <p>De administratieve toegang tot de vormen van de Douane <br> voor informatie over het verlenen van administratieve toegang van het toegangsniveau, zie <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md" class="MCXref xref"> gebruikers administratieve toegang van de Verlening tot bepaalde gebieden </a>.</p> <p>Opmerking: als u nog steeds geen toegang hebt, vraag dan aan de Workfront-beheerder of deze aanvullende beperkingen op uw toegangsniveau heeft ingesteld. Voor informatie over hoe een beheerder van Workfront uw toegangsniveau kan veranderen, zie <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref"> tot douanetoegangsniveaus </a> leiden of wijzigen.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p>Objectmachtigingen</p> </td> 
   <td> <p>Contribute heeft toegang tot het object waaraan het formulier is gekoppeld, en heeft toegang tot het aangepaste formulier bewerken</p> <p>Voor informatie bij het vragen van om extra toegang, zie <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref"> de toegang van het Verzoek tot voorwerpen </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42; om te weten te komen welk plan, vergunningstype, of toegang u hebt, contacteer uw beheerder van Workfront.

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
