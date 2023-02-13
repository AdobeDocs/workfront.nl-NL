---
content-type: reference
product-area: reporting;user-management
navigation-topic: custom-view-filter-and-grouping-samples
title: '''Weergave: documentrapport met koppeling naar bewijs"'
description: '''Weergave: documentrapport met koppeling naar bewijs"'
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: a38c5e86-9789-41ca-a832-2ee5eb0a570b
source-git-commit: 40c7142574c3491b7bdf8799c287db1c3f7e9e8c
workflow-type: tm+mt
source-wordcount: '339'
ht-degree: 0%

---

# Weergave: documentrapport met koppeling naar bewijs

In deze documentweergave kunt u een koppeling invoegen naar een proefdruk van de huidige versie van het document.

![](assets/view-document-with-proof-link-350x92.png)

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

## Een documentrapport weergeven met koppeling naar een proefdruk

Deze weergave toepassen:

1. Ga naar een lijst met documenten.
1. Van de **Weergave** vervolgkeuzelijst, selecteert u **Nieuwe weergave**.

1. Klikken **Kolom toevoegen**.
1. Klikken **Overschakelen naar tekstmodus**.
1. Houd de cursor boven het gebied van de tekstmodus en klik op **Klik om tekst te bewerken**.
1. Verwijder de tekst die u vindt in het dialoogvenster **Tekstmodus** en vervang deze door de volgende code:

   ```
   displayname=Proof Link
   
   shortview=true
   
   textmode=true
   
   valueexpression=CONCAT("https://Your domain.my.workfront.com/document/",{currentVersion}.{ID},"/proof/",{currentVersion}.{proofID},"/view")
   
   valueformat=HTML
   ```

   >[!TIP]
   >
   >Vervang &quot;Uw domein&quot; door uw Workfront-domein. Als de Workfront-URL van uw bedrijf bijvoorbeeld *Company.my.workfront.com*, uw domein is &quot;Bedrijf.&quot;

1. Klikken **Opslaan** vervolgens **Weergave opslaan**.
1. Typ een naam voor de weergave en klik vervolgens op **Weergave opslaan**.
1. (Optioneel) Als u alleen documenten met proefdrukken wilt weergeven, voegt u een filter toe door het volgende te doen:

   1. Klik op de knop **Filter** vervolgkeuzemenu en vervolgens op **Nieuw filter**.
   1. Klikken **Filterregel toevoegen** en typ Proefeigenaar en selecteer vervolgens **ID eigenaar van proefexemplaar** wanneer deze in de lijst wordt weergegeven.
   1. Selecteren **Is niet leeg** voor de filteroptie.
   1. Klikken **Filter opslaan**, typt u de naam van het filter en klikt u op **Filter opslaan**.

1. Klik op de koppeling in de kolom Proefkoppeling voor toegang tot de proefdruk van de laatste versie van het document.
