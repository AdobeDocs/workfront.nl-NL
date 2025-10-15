---
content-type: reference
product-area: reporting
navigation-topic: custom-view-filter-and-grouping-samples
title: 'Filter: Items weergeven op basis van dezelfde naam wanneer de statussen aan verschillende groepen zijn gekoppeld'
description: U kunt een taakstatus hebben die aan Groep A wordt toegewezen genoemd Nieuwe Status met de 3-letterige sleutel NST. U kunt een andere taakstatus hebben die aan Groep B ook wordt toegewezen genoemd Nieuwe Status met de 3-letterige sleutel NES. Hoewel de namen voor de twee statussen identiek kunnen zijn, is de 3-letterige code altijd uniek. Zie Een groepsstatus maken of bewerken voor meer informatie over groepsstatussen.
author: Nolan
feature: Reports and Dashboards
exl-id: 8ddcd8b1-44a9-4341-80c7-76ba70d2953b
source-git-commit: aa8275f252dd51f5a14d7aa931423aa4afb4ba8f
workflow-type: tm+mt
source-wordcount: '472'
ht-degree: 0%

---

# Filter: items weergeven op basis van dezelfde naam wanneer de statussen zijn gekoppeld aan verschillende groepen

<!--Audited: 10/2024-->

U kunt een taakstatus hebben die aan Groep A wordt toegewezen genoemd *Nieuwe Status* met de 3 brief sleutel *NST*. U kunt een andere taakstatus hebben die aan Groep B ook wordt toegewezen genoemd *Nieuwe Status* met 3 brief sleutel *NES.* Hoewel de namen voor de twee statussen identiek kunnen zijn, is de 3-letterige code altijd uniek.

Voor meer informatie over groepsstatussen, zie [ tot stand brengen of een groepsstatus ](../../../administration-and-setup/manage-groups/manage-group-statuses/create-or-edit-a-group-status.md) uitgeven.

Met de filterbuilder kunt u zich niet identificeren tussen de twee statussen met dezelfde naam. U moet de Tekstmodus in een aangepast filter gebruiken om onderscheid te maken tussen de twee statussen.

## Toegangsvereisten

+++ Breid uit om de toegangseisen voor de functionaliteit in dit artikel weer te geven. 

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-pakket</td> 
   <td> <p>Alle</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-licentie</td> 
   <td> 
   <p>Medewerker of verzoek om een filter te wijzigen </p>
   <p>Standaard of Plan om een rapport te wijzigen</p>
  </tr> 
  <tr> 
   <td role="rowheader">Configuraties op toegangsniveau</td> 
   <td> <p>Toegang tot rapporten, dashboards, kalenders bewerken om een rapport te wijzigen</p> <p>Toegang tot filters, weergaven en groepen bewerken om een filter te wijzigen</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objectmachtigingen</td> 
   <td> <p>Machtigingen beheren voor een rapport</p>  </td> 
  </tr> 
 </tbody> 
</table>

Voor meer detail over de informatie in deze lijst, zie [ vereisten van de Toegang in de documentatie van Workfront ](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Items weergeven met dezelfde naam als statussen wanneer de statussen zijn gekoppeld aan verschillende groepen

1. Ga naar de **drop-down van de Filter** voor de filter die u voor een lijst van taken, bijvoorbeeld wilt aanpassen.\
   Dit werkt ook voor projecten en kwesties.
1. Klik **Nieuwe filter**.
1. Selecteer Taak > Status in het eerste keuzemenu linksboven.
1. Selecteer **evenaart** voor de bepaling, dan selecteer één van de statussen u wilt rapporteren.

   Bijvoorbeeld, in een taakrapport, voeg **Status gelijk aan Nieuwe Status** toe, als u slechts taken wilt tonen die in een status van **Nieuwe Status** zijn.

   >[!TIP]
   >
   >U hebt slechts één optie voor een status met de naam Nieuwe status.

1. Klik **Wijze van de Tekst**.\
   De volgende code moet worden weergegeven in de beschikbare ruimte:

   <pre>OF :1: status=NST <br> OF :1: status_Mod=in </pre>

   >[!NOTE]
   >
   >Hier wordt slechts één status weergegeven. Op de statusregel wordt een van de 3-letterige toetsen voor een van de statussen weergegeven.

1. Voeg de volgende twee coderegels toe om de status toe te voegen die ontbreekt in het filter:

   <pre>OF :2: status=NES <br> OF :2: status_Mod=in</pre>

1. Klik **toepassen**, dan **sparen als nieuw**.

   In de lijst worden beide taken weergegeven met de status &quot;Nieuwe status&quot; in groep A en met de status &quot;Nieuwe status&quot; in groep B.
