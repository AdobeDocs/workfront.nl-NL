---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: 'Weergave: de inhoud van een kolom verbergen'
description: U kunt informatie in de kolom van een mening willen verbergen. U kunt dit doen door de tekstwijze van de kolom te wijzigen.
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: f4c3e1ca-d750-4f8b-835c-254c20ad72b3
source-git-commit: 661f925b4e485069122ef4278b2914d206387974
workflow-type: tm+mt
source-wordcount: '419'
ht-degree: 0%

---

# Weergave: de inhoud van een kolom verbergen

U kunt informatie in de kolom van een mening willen verbergen. U kunt dit doen door de tekstwijze van de kolom te wijzigen.

>[!TIP]
>
>* U kunt verborgen kolommen gebruiken om te sorteren op een bepaald object dat u niet wilt weergeven in de weergave.\
   >  U kunt bijvoorbeeld sorteren op Taaknummer in een taakweergave en de gegevens van Taaknummer verbergen in de weergave. In dit geval helpt het object waarnaar in de kolom wordt verwezen, de weergave te sorteren, maar wordt de informatie van dat object niet weergegeven in de weergave.
>* Als u een kolom verbergt, ziet u dat de informatie in de kolom verborgen is, maar dat de kolom nog steeds in de weergave voorkomt.
>


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
   <td> <p>Verzoek om een weergave te wijzigen </p>
   <p>Plan om een rapport te wijzigen</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraties op toegangsniveau*</td> 
   <td> <p>Toegang tot rapporten, dashboards, kalenders bewerken om een rapport te wijzigen</p> <p>Toegang tot filters, weergaven en groepen bewerken om een weergave te wijzigen</p> <p><b>OPMERKING</b>

Als u nog steeds geen toegang hebt, vraagt u de Workfront-beheerder of deze aanvullende beperkingen op uw toegangsniveau instelt. Voor informatie over hoe een beheerder van Workfront uw toegangsniveau kan wijzigen, zie <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Aangepaste toegangsniveaus maken of wijzigen</a>.</p> </td>
</tr> 
  <tr> 
   <td role="rowheader">Objectmachtigingen</td> 
   <td> <p>Rechten voor een rapport beheren</p> <p>Voor informatie over het aanvragen van aanvullende toegang raadpleegt u <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Toegang tot objecten aanvragen </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Neem contact op met uw Workfront-beheerder om te weten te komen welk plan, licentietype of toegang u hebt.

## Voorbeeld: U kunt de kolom Taaknummer in een taakweergave sorteren en verbergen:

1. Ga naar een takenlijst.
1. Van de **Weergave** vervolgkeuzelijst, klikt u op **Nieuwe weergave**.

1. Klikken **Kolom toevoegen** en begint &quot;Taaknummer&quot; te typen in het dialoogvenster **Tonen in deze kolom** selecteert u het veld wanneer het in de lijst wordt weergegeven.

1. Klikken **Overschakelen naar tekstmodus**.
1. Houd de cursor boven het gebied van de tekstmodus en klik op **Klik om tekst te bewerken**.
1. Verwijder de tekst die u vindt in het dialoogvenster **Tekstmodus** en vervang deze door de volgende code:

   <pre><strong>displayname=</strong>linkedname=direct<br>querysort=taskNumber<br>sortOrder=1<br>sortType=asc<br>textmode=true<br><strong>value=</strong>valueformat=int<br><strong>width=0</strong></pre>De belangrijkste wijzigingen in deze code waardoor de kolom verborgen wordt, zijn:

   ```
   displayname
   ```

   deze regel moet leeg zijn.

   ```
   valuefield
   ```

   Deze is vervangen door *value* en moet leeg zijn.

   ```
   width
   ```

   : Afhankelijk van het veld moet dit de waarde *0* of *1*.

1. Klikken **Opslaan** vervolgens **Weergave opslaan**.
