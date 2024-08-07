---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: 'Groeperen: de weergavenaam in een groep bewerken'
description: U kunt de namen van groepen in lijsten en rapporten wijzigen in iets wat de gebruikers beter bekend is.
author: Nolan
feature: Reports and Dashboards
exl-id: 072d3c2b-9ede-4bb9-9a27-dc77ceb732c4
source-git-commit: 138181de2ad8257785773a5296bc5bcfc144a801
workflow-type: tm+mt
source-wordcount: '369'
ht-degree: 0%

---

# Groeperen: de weergavenaam in een groep bewerken

<!--Audited: 01/2024-->

U kunt de namen van groepen wijzigen in iets wat de gebruikers beter bekend is.

Bijvoorbeeld, wanneer u de standaardgroepering van de Naam van het Portfolio op een lijst van projecten toepast, verschijnt de naam van de groepering als *Portfolio: Naam:`<name of portfolio>`*.

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
   <td>

<p>Nieuw: </p>
   <ul>
   <li> <p>Medewerker om een groep te wijzigen </p></li>
   <li><p>Standaard voor het wijzigen van een rapport</p></li></ul>

<p> Huidige:</p>
   <ul>  
   <li><p>Verzoek om een groepering te wijzigen </p></li>
   <li><p>Plan om een rapport te wijzigen</p></li> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraties op toegangsniveau*</td> 
   <td> <p>Toegang tot rapporten, dashboards, kalenders bewerken om een rapport te wijzigen</p> <p>Toegang tot filters, weergaven en groepen bewerken om een groep te wijzigen</p> <p><b>OPMERKING</b>

Als u nog steeds geen toegang hebt, vraagt u de Workfront-beheerder of deze aanvullende beperkingen op uw toegangsniveau instelt. Voor informatie over hoe een beheerder van Workfront uw toegangsniveau kan wijzigen, zie <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref"> tot douanetoegangsniveaus </a> leiden of wijzigen.</p> </td>
</tr>  
  <tr> 
   <td role="rowheader">Objectmachtigingen</td> 
   <td> <p>Machtigingen beheren voor een rapport</p> <p>Voor informatie bij het vragen van om extra toegang, zie <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref"> de toegang van het Verzoek tot voorwerpen </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42; om te weten te komen welk plan, vergunningstype, of toegang u hebt, contacteer uw beheerder van Workfront.

## De weergavenaam in een groep bewerken

De weergavenaam wijzigen in een projectgroep:

1. Ga naar een lijst met projecten.
1. Van **het Groeperen** drop-down menu, uitgezochte **Nieuwe Groepering**.

1. Klik **toevoegen Groepering**, en beginnen &quot;Naam van het Portfolio&quot;in **eerst te typen door:** gebied, dan selecteer het wanneer het in de lijst toont.

1. Klik **Schakelaar aan de Wijze van de Tekst**.
1. Voer een van de volgende handelingen uit:

   * Voeg de volgende code aan de bestaande tekst beschikbaar in de **Groep uw doos van het Rapport** toe:


     `group.0.displayname=Your Value`


     In dit geval:

     `group.0.displayname=Portfolio`

   * Verwijder alle regels in de interface van de tekstmodus van de groep die het woord &quot;naam&quot; bevatten en voeg vervolgens de regel toe:

     `group.0.name=Your Value`

     In dit geval:

     `group.0.name=Portfolio`

     >[!TIP]
     >
     >U kunt ook de regels `group.0.name=` en `group.0.displayname=` leeg laten. In dat geval geeft de groepering de waarde weer waarop u groepeert.


     ![](assets/grouping-edited-name-no-name-350x162.png)

1. Klik **Gedaan**, dan **sparen Groepering**.

   De standaardnaam voor de groepering wordt gewijzigd op basis van de gegevens in de tekstmodus.
