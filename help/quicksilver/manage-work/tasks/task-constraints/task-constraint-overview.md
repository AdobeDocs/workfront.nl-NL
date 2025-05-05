---
content-type: overview
product-area: projects
navigation-topic: task-constraints
title: Overzicht van taakbeperking
description: De beperkingen van de taak bepalen wanneer een taak op een project zou moeten beginnen en eindigen.
author: Alina
feature: Work Management
exl-id: 91b0844b-95a3-4d18-9fdb-a907dd42e1bf
source-git-commit: 91d757513792604677d6285baafa795629b4506d
workflow-type: tm+mt
source-wordcount: '691'
ht-degree: 0%

---

# Overzicht van taakbeperking

<!-- Audited: 12/2023 -->

De beperkingen van de taak bepalen wanneer een taak op een project zou moeten beginnen en eindigen.

## Overzicht van taakbeperkingen

Terwijl u uw projectplan maakt, neemt u beslissingen over de volgorde en het tijdkader van uw taken voor het project. Taken kunnen onafhankelijk van elke taakvolgorde functioneren, maar dit kan van invloed zijn op de projecttijdlijn. De Beperkingen van de taak staan een projectmanager toe om te plannen wanneer bepaalde taken op een project kunnen beginnen of voltooien.

Afhankelijk van de beperking die u gebruikt, moet u mogelijk een geplande begindatum, een geplande einddatum of beide opgeven voor de taak.

Restrictietypen waarvoor gedefinieerde datums zijn vereist, beïnvloeden de voorgaande relaties.

>[!TIP]
>
>U kunt overwegen een type beperking te gebruiken waarvoor geen specifieke datums zijn vereist als u voorgaande relaties tussen taken gebruikt.

In de volgende tabel worden elke restrictie en de afkorting daarvan weergegeven. Afkortingen worden gebruikt in taaklijsten en bij het maken van Kick-Start-importbestanden. Klik op de gekoppelde titel van elke taakbeperking voor meer informatie over dat type beperking.

<table border="1" cellspacing="15" cellpadding="1"> 
 <col> 
 <col> 
 <col>
 <thead> 
  <tr> 
   <th> <p><strong> Naam van de Beperking </strong> </p> </th> 
   <th> <p><strong> Afkorting </strong> </p> </th> 
   <th> <p><strong> Beschrijving </strong> </p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td scope="col"> <p><a href="../../../manage-work/tasks/task-constraints/as-soon-as-possible.md" class="MCXref xref"> overzicht van de Restrictie van de Taak: Zo spoedig mogelijk </a> </p> </td> 
   <td scope="col"> <p>ASAP</p> </td>
   <td scope="col"> <p>Plaatst de begintijd van de taak zo dicht mogelijk bij het begin van het project.</p> 
   <p>Het is de standaardbeperking als het project een Wijze van het Programma van de Datum van het Begin gebruikt en als de systeemstandaardbegindatum voor een nieuwe taak aan Gebaseerd op het Geplande Datum van het Project wordt geplaatst. </p>
   </td> 
  </tr> 
  <tr> 
   <td scope="col"> <p><a href="../../../manage-work/tasks/task-constraints/as-late-as-possible.md" class="MCXref xref"> Overzicht van taakbeperking: zo laat mogelijk </a> </p> </td> 
   <td scope="col"> <p>ALAP</p> </td> 
   <td scope="col"> <p>Hiermee plaatst u de voltooiingstijd van de taak zo dicht mogelijk bij het einde van het project.</p> 
   <p>Dit is de standaardbeperking wanneer de wijze van het projectprogramma van de Datum van de Voltooiing is en het systeem of groepgebrek voor de Datum van het Begin van een taak wordt geplaatst aan Gebaseerd op de Geplande Datum van het Project. </p>
   </td> 
  </tr> 
  <tr> 
   <td scope="col"> <p><a href="../../../manage-work/tasks/task-constraints/earliest-available-time.md" class="MCXref xref"> Overzicht van de Beperking van de Taak: De vroegste Beschikbare Tijd </a> </p> </td> 
   <td scope="col"> <p>EAT</p> </td> 
 <td scope="col"> <p>Plan een taak om bij de vroegste beschikbare tijd te beginnen na het overwegen van om het even welke voorgangersverhoudingen.</p> </td>
  </tr> 
  <tr> 
   <td scope="col"> <p><a href="../../../manage-work/tasks/task-constraints/latest-available-time.md" class="MCXref xref"> Overzicht van de Beperking van de Taak: De nieuwste Beschikbare Tijd </a> </p> </td> 
   <td scope="col"> <p>LAT</p> </td> 
   <td scope="col"> <p>Plan een taak om bij de recentste beschikbare tijd te beginnen na het overwegen van voorganger-opvolgerrelaties in het project.</p> </td>
  </tr> 
  <tr> 
   <td scope="col"> <p><a href="../../../manage-work/tasks/task-constraints/start-no-earlier-than.md" class="MCXref xref"> Overzicht van de Beperking van de Taak: Begin Geen vroeger dan </a> </p> </td> 
   <td scope="col"> <p>SNET</p> </td> 
   <td scope="col"> <p>Hiermee plant u een taak die moet worden gestart na de opgegeven datum.</p> 
   <p>Dit is de standaardbeperking als de Wijze van het projectprogramma van de Datum van het Begin is en als het systeem of de groep standaardDatum van het Begin voor een nieuwe taak aan Vandaag wordt geplaatst.   </td> 
  </tr> 
  <tr> 
   <td scope="col"> <p><a href="../../../manage-work/tasks/task-constraints/start-no-later-than.md" class="MCXref xref"> overzicht van de Restrictie van de Taak: Begin niet later dan </a> </p> </td> 
   <td scope="col"> <p>SNLT</p> </td> 
   <td scope="col"> <p>Hiermee plant u een taak die moet worden gestart vóór de datum die u opgeeft.</p> 
   <p>Dit is de standaardbeperking als de Wijze van het projectprogramma van de Datum van de Voltooiing is en als het systeem of groepsgebrek voor de Datum van het Begin van een taak aan Vandaag wordt geplaatst. 
   </td> 
  </tr> 
  <tr> 
   <td scope="col"> <p><a href="../../../manage-work/tasks/task-constraints/finish-no-earlier-than.md" class="MCXref xref"> overzicht van de Beperking van de Taak: Eindig geen vroeger dan </a> </p> </td> 
   <td scope="col"> <p>FNET</p> </td>
   <td scope="col"> <p>Hiermee wordt een taak gepland die na de opgegeven datum moet worden voltooid.</p> </td> 
  </tr> 
  <tr> 
   <td scope="col"> <p><a href="../../../manage-work/tasks/task-constraints/finish-no-later-than.md" class="MCXref xref"> overzicht van de Beperking van de Taak: Einde niet later dan </a> </p> </td> 
   <td scope="col"> <p>FNLT</p> </td> 
   <td scope="col"> <p>Hiermee wordt een taak gepland die moet worden voltooid vóór de datum die u opgeeft.</p> </td> 
  </tr> 
  <tr> 
   <td> <p><a href="../../../manage-work/tasks/task-constraints/must-start-on.md" class="MCXref xref"> overzicht van de Restrictie van de Taak: Moet </a> beginnen </p> </td> 
   <td scope="col"> <p>MSO</p> </td> 
   <td scope="col"> <p>Hiermee wordt een taak gepland die precies op een bepaalde datum moet beginnen.</p> </td> 
  </tr> 
  <tr> 
   <td> <p><a href="../../../manage-work/tasks/task-constraints/must-finish-on.md" class="MCXref xref"> overzicht van de Beperking van de Taak: Moet </a> beëindigen </p> </td> 
   <td scope="col"> <p>MFO</p> </td> 
   <td scope="col"> <p>Hiermee plant u een taak die op een bepaalde datum moet eindigen.</p> </td>
  </tr> 
  <tr> 
   <td> <p><a href="../../../manage-work/tasks/task-constraints/fixed-dates.md" class="MCXref xref"> overzicht van de Restrictie van de Taak: Vaste Daten </a> </p> </td> 
   <td> <p>FIXT</p> </td> 
   <td> <p>Hiermee wordt een taak gepland die op specifieke datums moet beginnen en eindigen.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Overzicht van standaardbeperkingen

Wanneer u nieuwe taken maakt, wordt automatisch een taakbeperking geselecteerd door Workfront.

Workfront gebruikt twee variabelen om te beslissen welke Restrictie van de Taak door gebrek voor een nieuwe taak wordt geselecteerd:

* Het **Programma van het Project van** gebied op het project.

  Voor informatie over het Programma van het Project van gebied, zie [ projecten ](../../../manage-work/projects/manage-projects/edit-projects.md) uitgeven.

* De **voorkeur van de Datum van het 0&rbrace; Begin &lbrace;die door uw Workfront of groepsbeheerder in het** wordt gevormd Taken &amp; van Kwesties **gebied van** Opstelling **.**

  Voor informatie over de Voorkeur van Taken &amp; van Kwesties, zie de [ Nieuwe sectie van de Taak Standaardwaarden ](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md#new-task-defaults) in [ de taak van het hele systeem vormen en voorkeur van de uitgave ](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md).

De volgende lijst toont de standaardBeperking van de Taak wanneer het kiezen van verschillende variabelen voor uw project en uw nieuwe taken:

| Projectschema van | Begindatum taak | Standaardtaakbeperking |
|---|---|---|
| Begindatum | Gebaseerd op de geplande projectdatum | Zo snel mogelijk |
| Begindatum | Vandaag | Niet eerder starten dan |
| Voltooiingsdatum | Gebaseerd op de geplande projectdatum | Zo laat mogelijk |
| Voltooiingsdatum | Vandaag | Niet later starten dan |
