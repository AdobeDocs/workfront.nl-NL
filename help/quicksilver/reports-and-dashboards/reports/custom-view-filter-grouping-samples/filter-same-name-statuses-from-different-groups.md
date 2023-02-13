---
content-type: reference
product-area: reporting
navigation-topic: custom-view-filter-and-grouping-samples
title: 'Filter: items weergeven op basis van dezelfde naam wanneer de statussen zijn gekoppeld aan verschillende groepen'
description: U kunt een taakstatus hebben die aan Groep A wordt toegewezen genoemd Nieuwe Status met de 3-letterige sleutel NST. U kunt een andere taakstatus hebben die aan Groep B ook wordt toegewezen genoemd Nieuwe Status met de 3-letterige sleutel NES. Hoewel de namen voor de twee statussen identiek kunnen zijn, is de 3-letterige code altijd uniek. Zie Een groepsstatus maken of bewerken voor meer informatie over groepsstatussen.
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: 8ddcd8b1-44a9-4341-80c7-76ba70d2953b
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '471'
ht-degree: 0%

---

# Filter: items weergeven op basis van status met dezelfde naam wanneer de statussen aan verschillende groepen zijn gekoppeld

U kunt een taakstatus hebben die aan Groep A wordt toegewezen *Nieuwe status* met de 3-lettertoets *NST*. U kunt een andere taakstatus hebben die aan Groep B ook wordt toegewezen genoemd *Nieuwe status* met de 3-lettertoets *NES.* Hoewel de namen voor de twee statussen identiek kunnen zijn, is de 3-letterige code altijd uniek.\
Voor meer informatie over groepsstatussen raadpleegt u [Een groepsstatus maken of bewerken](../../../administration-and-setup/manage-groups/manage-group-statuses/create-or-edit-a-group-status.md).

Met de filterbuilder kunt u zich niet identificeren tussen de twee statussen met dezelfde naam. U moet Tekstmodus gebruiken om onderscheid te maken tussen de twee statussen.

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

## Items weergeven met dezelfde naam als statussen wanneer de statussen zijn gekoppeld aan verschillende groepen

1. Ga naar het filter u voor een lijst van taken wilt aanpassen, bijvoorbeeld.\
   Dit werkt ook voor projecten en kwesties.
1. Klikken **Filterregel toevoegen** voor de **Status** veld van het object in uw lijst.\
   In een taakrapport voegt u bijvoorbeeld **Status gelijk aan nieuwe status**, als u alleen taken wilt weergeven die de status **Nieuwe status**.

   >[!TIP]
   >
   >U hebt slechts één optie voor een status met de naam Nieuwe status.

1. Klikken **Overschakelen naar tekstmodus**.\
   De volgende code moet worden weergegeven:

   <pre xml:space="preserve">status=NST<br>status_Mod=in </pre>

   >[!NOTE]
   >
   >Hier wordt slechts één status weergegeven. Op de statusregel wordt een van de 3-letterige toetsen voor een van de statussen weergegeven.

1. Voeg de volgende twee coderegels toe om de status toe te voegen die ontbreekt in het filter:

   <pre>OF:1:status=NES<br>OF:1:status_Mod=in</pre>

1. Klikken **Gereed** vervolgens **Filter opslaan**.

   In de lijst worden beide taken weergegeven met de status &quot;Nieuwe status&quot; in groep A en met de status &quot;Nieuwe status&quot; in groep B.
