---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: '''Weergave: de naam van bovenliggende taken weergeven als kapitalen'
description: U kunt deze kolom aan een taakmening toevoegen om de naam van de oudertaken in alle hoofdletters te tonen.
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: bb489920-6b17-4689-b432-b0c28bcb5d10
source-git-commit: 661f925b4e485069122ef4278b2914d206387974
workflow-type: tm+mt
source-wordcount: '300'
ht-degree: 0%

---

# Weergave: de naam van bovenliggende taken weergeven als kapitalen

U kunt deze kolom aan een taakmening toevoegen om de naam van de oudertaken in alle hoofdletters te tonen.

![](assets/column-task-with-all-caps-parent-350x112.png)

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
   <td> <p>Verzoek om filters, weergaven en groepen te wijzigen </p>
   <p>Plan om rapporten te wijzigen</p>
    </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraties op toegangsniveau*</td> 
   <td> <p>Toegang tot rapporten, dashboards, kalenders bewerken om een rapport te wijzigen</p> <p>Toegang tot filters, weergaven en groepen bewerken om afzonderlijke weergaven te wijzigen</p> <p><b>OPMERKING</b>

Als u nog steeds geen toegang hebt, vraagt u de Workfront-beheerder of deze aanvullende beperkingen op uw toegangsniveau instelt. Voor informatie over hoe een beheerder van Workfront uw toegangsniveau kan wijzigen, zie <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Aangepaste toegangsniveaus maken of wijzigen</a>.</p> </td>
</tr> 
  <tr> 
   <td role="rowheader">Objectmachtigingen</td> 
   <td> <p>Rechten voor een rapport beheren</p> <p>Voor informatie over het aanvragen van aanvullende toegang raadpleegt u <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Toegang tot objecten aanvragen </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Neem contact op met uw Workfront-beheerder om te weten te komen welk plan, licentietype of toegang u hebt.

## Naam van bovenliggende taken weergeven als kapitalen

Deze kolom bouwen in een taakmening:

1. Ga naar een takenlijst.
1. Van de **Weergave** vervolgkeuzelijst, selecteert u **Weergave aanpassen**.\
   of\
   Van de **Weergave** vervolgkeuzelijst, selecteert u **Nieuwe weergave**.

1. In de **Kolomvoorvertoning** klikt u op de kop van de kolom die de naam van de taak in de lijst weergeeft.
1. Klikken **Overschakelen naar tekstmodus**.
1. Plaats de muis boven het gebied in de tekstmodus en klik op **Klik om tekst te bewerken**.
1. Verwijder de tekst die u vindt in het dialoogvenster **Tekstmodus** en vervang deze door de volgende code: <pre>descriptionKey=name<br>displayname=Task Name<br>textmode=true<br>valueexpression=IF({numberOfChildren}>&quot;0&quot;,UPPER({name}),{name})<br>valueformat=HTML<br>width=150<br></pre>

1. Klikken **Weergave opslaan**.
