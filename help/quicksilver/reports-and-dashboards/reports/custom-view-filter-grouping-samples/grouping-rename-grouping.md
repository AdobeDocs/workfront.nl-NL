---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: 'Groeperen: de weergavenaam in een groep bewerken'
description: U kunt de namen van groepen wijzigen in iets wat de gebruikers beter bekend is.
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: 072d3c2b-9ede-4bb9-9a27-dc77ceb732c4
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '323'
ht-degree: 0%

---

# Groeperen: de weergavenaam in een groep bewerken

U kunt de namen van groepen wijzigen in iets wat de gebruikers beter bekend is.

Als u bijvoorbeeld de standaardgroepering Naam Portfolio toepast op een lijst met projecten, wordt de naam van de groepering weergegeven als *Portfolio: Naam:`<name of portfolio>`*.

![](assets/grouping-unedited-name-350x167.png)

U kunt deze groepering wijzigen door in de tekstmodus een naam weer te geven die beter leesbaar is.

![](assets/grouping-edited-name-350x160.png)

## Toegangsvereisten

U moet de volgende toegang hebben om de stappen in dit artikel uit te voeren:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-abonnement*</td> 
   <td> <p>Alle</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-licentie*</td> 
   <td> <p>Plan </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraties op toegangsniveau*</td> 
   <td> <p>Toegang tot rapporten, dashboards, kalenders bewerken</p> <p>Toegang tot filters, weergaven, groepen bewerken</p> <p>Opmerking: Als u nog steeds geen toegang hebt, vraagt u de Workfront-beheerder of deze aanvullende beperkingen op uw toegangsniveau instelt. Voor informatie over hoe een beheerder van Workfront uw toegangsniveau kan wijzigen, zie <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Aangepaste toegangsniveaus maken of wijzigen</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objectmachtigingen</td> 
   <td> <p>Rechten voor een rapport beheren</p> <p>Voor informatie over het aanvragen van aanvullende toegang raadpleegt u <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Toegang tot objecten aanvragen </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Neem contact op met uw Workfront-beheerder om te weten te komen welk plan, licentietype of toegang u hebt.

## De weergavenaam in een groep bewerken

De weergavenaam wijzigen in een projectgroep:

1. Ga naar een lijst met projecten.
1. Van de **Groepering** vervolgkeuzelijst, selecteert u **Nieuwe groepering**.

1. Klikken **Groepering toevoegen** en typ &quot;naam Portfolio&quot; in het dialoogvenster **Eerst door:** en selecteert u deze wanneer deze in de lijst wordt weergegeven.

1. Klikken **Overschakelen naar tekstmodus**.
1. Gereed op een van de volgende manieren:

   * Voeg de volgende code toe aan de bestaande tekst beschikbaar in het dialoogvenster **Uw rapport groeperen** vak:

      ```
      group.0.displayname=Your
      ```

      ```
      Value
      ```

      In dit geval:

      ```
      group.0.displayname=Portfolio
      ```

   * Verwijder alle regels in de interface van de tekstmodus van de groep die het woord &quot;naam&quot; bevatten en voeg vervolgens de regel toe:

      ```
      group.0.name=Your Value
      ```

      In dit geval:

      ```
      group.0.name=Portfolio
      ```

      U kunt ook de

      ```
      group.0.name
      ```

      regel leeg. In dat geval wordt in de groep de naam weergegeven van de waarde waarop u groepeert.

      ![](assets/grouping-edited-name-no-name-350x162.png)

1. Klikken **Gereed** vervolgens **Groepering opslaan**.
