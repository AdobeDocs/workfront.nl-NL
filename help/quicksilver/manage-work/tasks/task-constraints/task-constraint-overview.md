---
content-type: overview
product-area: projects
navigation-topic: task-constraints
title: Overzicht van taakbeperking
description: De beperkingen van de taak bepalen wanneer een taak op een project zou moeten beginnen en eindigen.
author: Alina
feature: Work Management
exl-id: 91b0844b-95a3-4d18-9fdb-a907dd42e1bf
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '418'
ht-degree: 0%

---

# Overzicht van taakbeperking

De beperkingen van de taak bepalen wanneer een taak op een project zou moeten beginnen en eindigen.

## Overzicht van taakbeperkingen

Terwijl u uw projectplan maakt, neemt u beslissingen over de volgorde en het tijdkader van uw taken voor het project. Taken kunnen onafhankelijk van elke taakvolgorde functioneren, maar dit kan van invloed zijn op de projecttijdlijn. De Beperkingen van de taak staan een projectmanager toe om te plannen wanneer bepaalde taken op een project kunnen beginnen of voltooien.

Afhankelijk van de beperking die u gebruikt, moet u mogelijk een geplande begindatum, een geplande einddatum of beide opgeven voor de taak.

Restrictietypen waarvoor gedefinieerde datums zijn vereist, beïnvloeden de voorgaande relaties.

>[!TIP]
>
>U kunt overwegen een type beperking te gebruiken waarvoor geen specifieke datums zijn vereist als u een eerdere relatie tussen taken gebruikt.

In de volgende tabel worden elke restrictie en de afkorting ervan weergegeven. Afkortingen worden gebruikt in taaklijsten en bij het maken van Kick-Start-importbestanden. Klik op de gekoppelde titel van elke taakbeperking voor meer informatie over dat type beperking.

<table border="1" cellspacing="15" cellpadding="1"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th> <p><strong>Restrictienaam</strong> </p> </th> 
   <th> <p><strong>Afkorting</strong> </p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td scope="col"> <p><a href="../../../manage-work/tasks/task-constraints/as-soon-as-possible.md" class="MCXref xref">Overzicht van taakbeperking: Zo snel mogelijk</a> </p> </td> 
   <td scope="col"> <p>ASAP</p> </td> 
  </tr> 
  <tr> 
   <td scope="col"> <p><a href="../../../manage-work/tasks/task-constraints/as-late-as-possible.md" class="MCXref xref">Overzicht van taakbeperking: Zo laat mogelijk </a> </p> </td> 
   <td scope="col"> <p>ALAP</p> </td> 
  </tr> 
  <tr> 
   <td scope="col"> <p><a href="../../../manage-work/tasks/task-constraints/earliest-available-time.md" class="MCXref xref">Overzicht van taakbeperking: Vroegst beschikbare tijd</a> </p> </td> 
   <td scope="col"> <p>EAT</p> </td> 
  </tr> 
  <tr> 
   <td scope="col"> <p><a href="../../../manage-work/tasks/task-constraints/latest-available-time.md" class="MCXref xref">Overzicht van taakbeperking: Laatste beschikbare tijd</a> </p> </td> 
   <td scope="col"> <p>LAT</p> </td> 
  </tr> 
  <tr> 
   <td scope="col"> <p><a href="../../../manage-work/tasks/task-constraints/start-no-earlier-than.md" class="MCXref xref">Overzicht van taakbeperking: Niet eerder starten dan</a> </p> </td> 
   <td scope="col"> <p>SNET</p> </td> 
  </tr> 
  <tr> 
   <td scope="col"> <p><a href="../../../manage-work/tasks/task-constraints/start-no-later-than.md" class="MCXref xref">Overzicht van taakbeperking: Niet later starten dan</a> </p> </td> 
   <td scope="col"> <p>SNLT</p> </td> 
  </tr> 
  <tr> 
   <td scope="col"> <p><a href="../../../manage-work/tasks/task-constraints/finish-no-earlier-than.md" class="MCXref xref">Overzicht van taakbeperking: Niet eerder voltooien dan</a> </p> </td> 
   <td scope="col"> <p>FNET</p> </td> 
  </tr> 
  <tr> 
   <td scope="col"> <p><a href="../../../manage-work/tasks/task-constraints/finish-no-later-than.md" class="MCXref xref">Overzicht van taakbeperking: Niet later voltooien dan</a> </p> </td> 
   <td scope="col"> <p>FNLT</p> </td> 
  </tr> 
  <tr> 
   <td> <p><a href="../../../manage-work/tasks/task-constraints/must-start-on.md" class="MCXref xref">Overzicht van taakbeperking: Moet beginnen op</a> </p> </td> 
   <td scope="col"> <p>MSO</p> </td> 
  </tr> 
  <tr> 
   <td> <p><a href="../../../manage-work/tasks/task-constraints/must-finish-on.md" class="MCXref xref">Overzicht van taakbeperking: Moet worden voltooid op</a> </p> </td> 
   <td scope="col"> <p>MFO</p> </td> 
  </tr> 
  <tr> 
   <td> <p><a href="../../../manage-work/tasks/task-constraints/fixed-dates.md" class="MCXref xref">Overzicht van taakbeperking: Vaste datums</a> </p> </td> 
   <td> <p>FIXT</p> </td> 
  </tr> 
 </tbody> 
</table>

## Overzicht van standaardbeperkingen

Wanneer u nieuwe taken maakt, wordt automatisch een taakbeperking geselecteerd door Workfront.

Workfront gebruikt twee variabelen om te beslissen welke de Beperking van de Taak door gebrek voor een nieuwe taak wordt geselecteerd:

* De **Projectschema van** veld op het project.

   Voor informatie over het Programma van het Project van gebied, zie [Projecten bewerken](../../../manage-work/projects/manage-projects/edit-projects.md).

* De **Begindatum** door uw Workfront of groepsbeheerder ingestelde voorkeur in het dialoogvenster **Taken en problemen** gebied van **Instellen**.

   Voor informatie over de Voorkeur van Taken &amp; van Kwesties, zie de &quot;Nieuwe sectie van de Standaardinstellingen van de Taak&quot;in [Taak- en probleemvoorkeuren voor het hele systeem configureren](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md).

De volgende lijst toont de standaardBeperking van de Taak wanneer het kiezen van verschillende variabelen voor uw project en uw nieuwe taken:

| Projectschema van | Begindatum taak | Standaardtaakbeperking |
|---|---|---|
| Begindatum | Gebaseerd op de geplande projectdatum | Zo snel mogelijk |
| Begindatum | Vandaag | Niet eerder starten dan |
| Voltooiingsdatum | Gebaseerd op de geplande projectdatum | Zo laat mogelijk |
| Voltooiingsdatum | Vandaag | Niet later starten dan |
