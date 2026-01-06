---
product-area: projects
navigation-topic: update-work-items-and-view-updates
title: Alle updates in een notitierapport weergeven
description: Als u alle updates wilt zien die een van de gebruikers voor een object heeft ingevoerd, kunt u een notitierapport maken waarin alle updates worden weergegeven.
author: Alina
feature: Get Started with Workfront
exl-id: fa5b91e4-b88c-42f0-860c-6864105b4652
source-git-commit: dbc4404501e20b3f1905a5eebd13734a65db27ae
workflow-type: tm+mt
source-wordcount: '373'
ht-degree: 0%

---

# Alle updates in een notitierapport weergeven

<!-- Audited: 10/2025 -->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: Alina: ***This is a report and it is in the Getting Started/ Updates section because I think it makes more sense to be in this area, where people want to view updates. - added this to this section from Reporting on 7/3/2018 ) </p>
-->

In het gedeelte Updates van een object wordt standaard maximaal 200 updates weergegeven. Als u alle updates wilt zien die een van de gebruikers voor een object heeft ingevoerd, kunt u een notitierapport maken waarin alle updates worden weergegeven.

>[!NOTE]
>
>U kunt een rapport bouwen om updates op voorwerpen in Voorproef met het de ingangsrapport van het Dagboek te bekijken. Voor meer informatie, zie [ Rapport over het gebied van Updates met een rapport van de Ingang van het Dagboek ](../../reports-and-dashboards/reports/creating-and-managing-reports/create-journal-entry-report.md).

## Toegangsvereisten

+++ Breid uit om de toegangseisen voor de functionaliteit in dit artikel weer te geven.

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-pakket</td> 
   <td> <p>Alle</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-licentie</td> 
   <td> <p>Standard</p>
   <p>Plan</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraties op toegangsniveau</td> 
   <td> <p>Bewerk de toegang met de mogelijkheid om het volgende te maken:</p> 
    <ul> 
     <li> <p>Rapporten, dashboards en Kalenders</p> </li> 
     <li> <p>Filters, Weergaven en Groepen</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objectmachtigingen</td> 
   <td> <p>De toestemmingen van de mening op de voorwerpen in het rapport</p>
   </td> 
  </tr> 
 </tbody> 
</table>

Voor informatie, zie [ vereisten van de Toegang in de documentatie van Workfront ](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

<!--Old:
<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan</td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license</td> 
   <td> <p>New: Standard </p>
   <p>Current: Plan</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations</td> 
   <td> <p>Edit access to:</p> 
    <ul> 
     <li> <p>Create Reports, Dashboards, and Calendars</p> </li> 
     <li> <p>Create Filters, Views, and Groupings</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>View</p>
    <p>Note: If you do not have View permission or higher to an object, information for that object doesn't display in the report.</p>  </td> 
  </tr> 
 </tbody> 
</table>-->

## Een notitierapport maken

Het maken van een rapport voor Notities voor elk object is identiek, ongeacht het object.

Bijvoorbeeld, om een rapport van de Nota voor alle nota&#39;s op een project tot stand te brengen:

{{step1-to-reports}}

1. In de upper-left hoek van de pagina, klik **Nieuw Rapport**, dan uitgezochte **Nota**.

1. (Facultatief) klik **(Kolommen) Mening**, dan **voeg Kolom** toe om de **Naam** van het **Project** in de mening van het rapport toe te voegen.

1. (Facultatief) als u op veelvoudige projecten tezelfdertijd rapporteert, klik **Groepen**, dan **voeg Groepering** aan groep door de **Naam** van het **Project** toe. Dit zorgt ervoor dat de nota&#39;s door hun respectieve projecten worden gegroepeerd, die het rapport gemakkelijker maken te lezen.

1. (Facultatief) klik **Filters**, dan **voeg een Regel van de Filter** toe.
1. Voeg een filter voor **Nota** toe > **de Tekst van de Nota** > **is niet leeg**.

   ![](assets/note-note-text-not-blank-filter.png)

   >[!TIP]
   >
   >   Als een projectgebied werd bijgewerkt maar geen nota werd toegevoegd op het tijdstip van de update, **de Tekst van de Nota** van de updatevertoningen als **(Geen tekst die aan update wordt toegevoegd)**.


1. (Facultatief) voeg een andere filter voor **Project** toe > **Naam** > **evenaart aan** en voegt één of verscheidene projectnamen toe waarvoor u nota&#39;s wilt bekijken.
1. Klik **sparen + Sluiten**. Alle updates ingegaan op het project door alle gebruikers met toestemmingen om het project te bekijken worden getoond in het rapport.
