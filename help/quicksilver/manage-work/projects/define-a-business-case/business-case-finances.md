---
content-type: overview
navigation-topic: business-case-and-scorecards
title: Overzicht van de financiële vakgebieden Bedrijfscase
description: Het subtabblad Bedrijfscase bevat financiële velden voor het project. Om sommige financiële gebieden waarde te hebben, moeten de overeenkomstige gebieden van het BedrijfsGeval worden voltooid.
author: Becky
feature: Work Management
exl-id: d420fc3e-e98d-47a0-a456-b2df17d72f34
source-git-commit: dbc4404501e20b3f1905a5eebd13734a65db27ae
workflow-type: tm+mt
source-wordcount: '745'
ht-degree: 0%

---

# Overzicht van de financiële vakgebieden Bedrijfscase

Het subtabblad Bedrijfscase bevat financiële velden voor het project. Om sommige financiële gebieden waarde te hebben, moeten de overeenkomstige gebieden van het BedrijfsGeval worden voltooid.

De volgende financiële gebieden van het project tonen in het BedrijfsGeval:

<table border="1" cellspacing="15" cellpadding="1"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th scope="col">Naam van veld</th> 
   <th scope="col">Beschrijving</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>Uitgelijnd </td> 
   <td> <p>Toont de groepering van het project volgens zijn scorecard. Een hoog percentagewaarde wijst erop dat het project goed-gericht met het doel en de doelstellingen van de organisatie is. <br> voor meer informatie over het gebruiken van scorecards, zie <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/create-scorecard.md" class="MCXref xref"> een scorecard </a> creëren.</p> <p>Dit gebied toont in het Van Bedrijfs Geval Summiere gebied. </p> </td> 
  </tr> 
  <tr> 
   <td>Geraamde kosten</td> 
   <td> <p>De totale kosten die naar schatting aan het project zullen worden gekoppeld wanneer het project wordt gestart.</p> <p>De begrote kosten voor het project worden berekend aan de hand van de volgende formule:<br></p> <p><code>Budgeted Cost = Budgeted Expense Cost + Budgeted Labor Cost </code> <br> </p> <p>Adobe Workfront gebruikt de begrote uren uren van de Planner van het Middel om de begrote arbeidskosten te berekenen.<br> voor meer informatie over het berekenen van Beoogde Kosten, zie <a href="../../../manage-work/projects/project-finances/budgeted-cost.md" class="MCXref xref"> Beoogde Kosten </a> berekenen. </p> <p>Dit gebied toont in het Van Bedrijfs Geval Summiere gebied.</p> </td> 
  </tr> 
  <tr> 
   <td>begrote kosten</td> 
   <td> <p>De begrote kosten van alle uitgaven voor het project. </p> <p>Dit wordt berekend aan de hand van de volgende formule:</p> <p><code>Budgeted Expense Cost = SUM(Planned Amount of Expenses on the project) </code></p> <p>Voor meer informatie over het berekenen van uitgaven, zie <a href="../../../manage-work/projects/project-finances/manage-project-expenses.md" class="MCXref xref"> projectuitgaven beheren </a>.</p> <p>Dit veld wordt weergegeven in het gebied Uitgaven.</p> </td> 
  </tr> 
  <tr> 
   <td>begrote arbeidskosten</td> 
   <td> <p>De kosten verbonden aan de middelen die worden toegewezen om het werk aan het project te voltooien.</p> <p>De begrote loonkosten voor het project worden berekend aan de hand van de volgende formule:<br></p> <p><code>Budgeted Labor Cost = SUM(Estimated/ Budgeted hours for each job role on the project * Cost per Hour rate of each job role on the project) </code><br></p> <p>Workfront gebruikt de begrote uren uren van de Planner van het Middel om de begrote arbeidskosten te berekenen.<br> voor meer informatie over het berekenen van de Begrotende Kosten van de Arbeid, zie <a href="../../../manage-work/projects/project-finances/budgeted-labor-cost.md" class="MCXref xref"> Begonnen Arbeidskosten en Begrotingspunten voor projecten </a> begrijpen.</p> <p>Dit gebied toont op het gebied van de Begroting van het Middel van het BedrijfsGeval. </p> </td> 
  </tr> 
  <tr> 
   <td>Voorziene uitgaven</td> 
   <td> <p>Dit is hetzelfde als de begrote kosten. </p> <p>Opmerking: De geplande kosten van de uitgaven verschillen van de geplande kosten voor het project. De geraamde kosten worden berekend op basis van het geplande bedrag van de kosten van het project, terwijl de geplande kosten worden berekend op basis van de geplande uren van het project. </p> <p>Dit veld wordt voor elke uitgave weergegeven in het gebied Uitgaven.</p> </td> 
  </tr> 
  <tr> 
   <td>Nettowaarde</td> 
   <td> <p>Dit is de totale verwachte waarde van het project na berekening van het voordeel en verwijdering van de kosten.</p> <p>De nettowaarde voor het project wordt berekend aan de hand van de volgende formule:<br></p> <p><code>Net Value = Planned Benefit - Budgeted Cost - Potential Risk</code>. <br></p> <p>Voor meer informatie over het berekenen van Netto Waarde, zie <a href="../../../manage-work/projects/project-finances/calculate-net-value.md" class="MCXref xref"> Netto Waarde berekenen </a>.<br></p> <p>Dit gebied toont in het Van Bedrijfs Geval Summiere gebied.</p> </td> 
  </tr> 
  <tr> 
   <td>Gepland voordeel</td> 
   <td>Een handmatige schatting van het geldelijke voordeel voor uw organisatie wanneer dit project wordt voltooid. Het kan om het even welk bedrag van munt zijn en het is specifiek voor u en aan elk project u beheert. Het geplande voordeel kan geen negatieve waarde hebben. Dit gebied toont in het Van Bedrijfs Geval Summiere gebied en het kan op het gebied van Info van het Project van het BedrijfsGeval worden uitgegeven. </td> 
  </tr> 
  <tr> 
   <td>Potentiële kosten van risico's</td> 
   <td> <p>Dit zijn de potentiële kosten van alle risico's voor het project. </p> <p>Dit wordt berekend aan de hand van de volgende formule:</p> <p><code>Potential Risk = SUM(Potential Cost * Probability of Risk) </code></p> <p>Voor meer informatie over risico's op het project, zie <a href="../../../manage-work/projects/define-a-business-case/create-edit-risks-on-projects.md" class="MCXref xref"> risico's op projecten </a> creëren en uitgeven.</p> <p>Dit gebied toont in het Van Bedrijfs Geval Summiere gebied.</p> </td> 
  </tr> 
  <tr> 
   <td>Potentieel risico</td> 
   <td> <p>In de Samenvatting van de Bedrijfs- Gevallen, is dit het bedrag van de kosten van alle risico's als zij zouden moeten voorkomen, gebaseerd op hun waarschijnlijkheid. Bijvoorbeeld, als een Risico een Potentiële Kosten van $100 heeft en een Mogelijke van het voorkomen van van 10%, is het Potentiële Risico $10. Het potentiële risico in de Samenvatting van de Bedrijfs- Gevallen wordt berekend door de volgende formule:</p> <p><code>Potential Risk = SUM(Risk Potential Cost x Probability)</code> voor alle risico's. </p> </td> 
  </tr> 
  <tr> 
   <td>Kosten risicobeperking</td> 
   <td> <p>De kosten van het mitigatieplan voor de risico's die u schat zouden op het project kunnen voorkomen.<br> voor meer informatie over risico's op het project, zie <a href="../../../manage-work/projects/define-a-business-case/create-edit-risks-on-projects.md" class="MCXref xref"> risico's op projecten </a> creëren en uitgeven.</p> <p>Dit gebied toont op het gebied van Risks voor elk risico dat op het project wordt gespecificeerd.</p> </td> 
  </tr> 
  <tr> 
   <td>Potentiële kosten voor één risico</td> 
   <td> <p>De geschatte financiële kosten wanneer de voor het project gedefinieerde risico's daadwerkelijk zouden optreden, ongeacht de waarschijnlijkheid ervan. </p> <p>Dit is een manueel bijgewerkt gebied dat over elk risico op het gebied van Risks van het BedrijfsGeval toont. </p> </td> 
  </tr> 
  <tr> 
   <td>Risico's totale potentiële kosten</td> 
   <td> <p>Dit is de totale geschatte financiële kosten van alle risico's die bij het project zijn vastgesteld wanneer zij daadwerkelijk hebben plaatsgevonden. </p> <p>Dit wordt berekend aan de hand van de volgende formule:</p> <p><code>Risks Total Potential Cost = SUM(Potential Cost of all risks on the project) </code></p> <p>Het wordt weergegeven als een valutanummer naast de titel van het gebied Risks van de Business Case.</p> </td> 
  </tr> 
 </tbody> 
</table>
