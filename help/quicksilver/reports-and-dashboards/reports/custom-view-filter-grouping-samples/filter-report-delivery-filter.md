---
content-type: reference
product-area: reporting
navigation-topic: custom-view-filter-and-grouping-samples
title: 'Filter: weergaverapporten die zijn gepland voor levering'
description: Dit rapportfilter geeft alle rapporten weer die automatisch worden geleverd in Adobe Workfront. U kunt deze instelling het beste gebruiken in de standaardweergave.
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: 7b937384-80c9-4bc7-94be-5573cf86b35b
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '210'
ht-degree: 0%

---

# Filter: weergaverapporten die zijn gepland voor levering

Dit rapportfilter geeft alle rapporten weer die automatisch worden geleverd in Adobe Workfront. U kunt deze instelling het beste gebruiken in de standaardweergave.

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

## Rapportfilter

Dit filter toepassen:

1. Ga naar een lijst met rapporten.
1. Van de **Filter** vervolgkeuzelijst, selecteert u **Nieuw filter**.

1. Klikken **Overschakelen naar tekstmodus**.
1. In de **Filterregels instellen voor uw rapport** gebied, kopieert en plakt de volgende code:

   ```
   scheduledReportID=0<br>scheduledReportID_Mod=notnull
   ```

1. Klikken **Filter opslaan**.
