---
content-type: reference
product-area: reporting;projects;user-management
navigation-topic: custom-view-filter-and-grouping-samples
title: '''Groeperen: Projectsponsor voor uren"'
description: Deze uurgroepering organiseert uren door de sponsor van het project waar de uren worden geregistreerd. De standaardinterface van de rapportbouwer voor uurgroepen verstrekt geen afbeelding aan het gebied van de Sponsor van het Project. U moet de interface Tekstmodus gebruiken om dit veld te openen.
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: 6b35b0ef-18b7-4121-ae39-d7957d76c04b
source-git-commit: 661f925b4e485069122ef4278b2914d206387974
workflow-type: tm+mt
source-wordcount: '295'
ht-degree: 0%

---

# Groeperen: Projectsponsor voor uren

Deze uurgroepering organiseert uren door de sponsor van het project waar de uren worden geregistreerd. De standaardinterface van de rapportbouwer voor uurgroepen verstrekt geen afbeelding aan het gebied van de Sponsor van het Project. U moet de interface Tekstmodus gebruiken om dit veld te openen.

![hour_report_grouped_by_sponsor.png](assets/hour-report-grouped-by-sponsor-350x39.png)

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
   <td> <p>Verzoek om een groepering te wijzigen </p>
   <p>Plan om een rapport te wijzigen</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraties op toegangsniveau*</td> 
   <td> <p>Toegang tot rapporten, dashboards, kalenders bewerken om een rapport te wijzigen</p> <p>Toegang tot filters, weergaven en groepen bewerken om een groep te wijzigen</p> <p><b>OPMERKING</b>

Als u nog steeds geen toegang hebt, vraagt u de Workfront-beheerder of deze aanvullende beperkingen op uw toegangsniveau instelt. Voor informatie over hoe een beheerder van Workfront uw toegangsniveau kan wijzigen, zie <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Aangepaste toegangsniveaus maken of wijzigen</a>.</p> </td>
</tr>  
  <tr> 
   <td role="rowheader">Objectmachtigingen</td> 
   <td> <p>Rechten voor een rapport beheren</p> <p>Voor informatie over het aanvragen van aanvullende toegang raadpleegt u <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Toegang tot objecten aanvragen </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Neem contact op met uw Workfront-beheerder om te weten te komen welk plan, licentietype of toegang u hebt.

## Uren groeperen op projectsponsor

Deze groep toepassen:

1. Ga naar een lijst met uren.
1. Van de **Groepering** vervolgkeuzelijst, selecteert u **Nieuwe groepering**.

1. Klikken **Overschakelen naar tekstmodus**.
1. De tekst in het dialoogvenster verwijderen **Uw rapport groeperen** gebied.

1. Vervang de tekst door de volgende code:

   <pre>group.0.linkedname=project:sponsor:name<br>group.0.name=<br>group.0.valueField=project:sponsor:name<br>groep.0.valueFormat=HTML<br>textmode=true<br></pre>

1. Klikken **Groepering opslaan**.
