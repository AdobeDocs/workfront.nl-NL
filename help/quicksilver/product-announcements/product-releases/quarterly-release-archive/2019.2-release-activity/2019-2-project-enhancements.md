---
content-type: release-notes
navigation-topic: 2019-2-release-activity
title: 2019.2 Projectverbeteringen
description: Op deze pagina worden alle projectverbeteringen beschreven die zijn opgenomen in de release van 2019.2. De functionaliteit zal naar verwachting in de week van 20 mei 2019 beschikbaar zijn in de productieomgeving.
author: Luke
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: 76292f90-af1a-4740-9b8e-b02a6303625c
source-git-commit: f1e463c90641f9221228e335b583cab72762b3bd
workflow-type: tm+mt
source-wordcount: '731'
ht-degree: 0%

---

# 2019.2 Projectverbeteringen

Op deze pagina worden alle projectverbeteringen beschreven die zijn opgenomen in de release van 2019.2. De functionaliteit zal naar verwachting in de week van 20 mei 2019 beschikbaar zijn in de productieomgeving.

Voor een lijst van alle veranderingen die in 2019.2 worden aangebracht, zie [ 2019.2 Overzicht van de Activiteit van de Versie ](../../../../product-announcements/product-releases/quarterly-release-archive/2019.2-release-activity/2019-2-release-activity-overview.md).

## Groepen sneller zoeken bij het aanpassen van statussen

Het vervolgkeuzemenu op het tabblad Statussen in het gedeelte Instellen is nu een hoofdmenu. Op deze manier kunt u snel elke groep in het systeem zoeken en zoeken, zodat statussen gemakkelijker kunnen worden aangepast.

Eerder werd in de vervolgkeuzelijst een beperkt aantal groepen weergegeven. Als de groep u wilde niet tonen, moest u aan Opstelling > Groepen navigeren en de specifieke groep vinden om de status van de groep aan te passen.

Voor meer informatie, zie [ een status ](../../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-or-edit-a-status.md) creëren of uitgeven.

## Standaard aangepaste Forms- en goedkeuringsprocessen koppelen aan taken

U kunt standaarddouaneformulieren en goedkeuringsprocessen nu vormen om aan taken vast te maken wanneer u taken aan een project toevoegt. U kunt de standaardmontages op het projectniveau vormen.

Voor informatie over het vormen van standaarddouaneformulieren en goedkeuringsprocessen voor taken op het projectniveau, zie de &quot;sectie van Taken&quot;in [ projecten ](../../../../manage-work/projects/manage-projects/edit-projects.md) artikel uitgeven.

## De gehele rij van een bovenliggende taak in Vet weergeven in een takenlijst

In een takenlijst, wordt de rij die een oudertaak bevat getoond in vette letters. Deze verandering is zichtbaar wanneer de lijst door de structuur van de Onderverdeling van het Werk of door het Aantal van de Taak in stijgende orde wordt gesorteerd.

## Wijzigingen in taaklijsten omkeren

Met de nieuwe knop Automatisch opslaan in de takenlijst kunt u opgeven of de aangebrachte wijzigingen automatisch moeten worden opgeslagen of dat u de effecten wilt zien die de wijzigingen hebben aangebracht voordat u ze opslaat. Deze instelling is van toepassing op zowel de takenlijst als het Gantt-diagram.

Vóór deze verbetering, werden alle veranderingen altijd automatisch bewaard.

Voor informatie over het uitgeven van taken in een taaklijst, zie [ taken ](../../../../manage-work/tasks/manage-tasks/edit-tasks.md) uitgeven.

Voor informatie over het uitgeven van taken in de grafiek van Gantt, zie [ informatie van de Update in de Grafiek van Gantt van de taaklijst ](../../../../manage-work/gantt-chart/use-the-gantt-chart/update-info-task-list-gantt.md).

## Nieuwe standaardwaarden kolombreedte in nieuwe lijsten

Workfront past nu automatisch de breedte van de kolommen aan op basis van de informatie over de notatie van de waarde in elke kolom. Kolommen met een getal zijn bijvoorbeeld breder dan de kolommen met het veld Beschrijving.

Vóór deze verbetering, werden de kolombreedten in het nieuwe project en de taakmeningen geplaatst aan 100 pixel, tenzij anders gespecificeerd.

Voor informatie over kolombreedten, zie [ kolombreedte en orde wijzigen ](../../../../reports-and-dashboards/reports/reporting-elements/modify-column-width-order.md).

## Ongebruikte objecten deactiveren

>[!NOTE]
>
>Deze functie is tijdens de voorvertoningsperiode van 2019.2 rechtstreeks in de productieomgeving uitgebracht.

Als u objecten hebt die niet meer worden gebruikt, kunt u deze deactiveren en verbergen in lijsten om te voorkomen dat gebruikers deze aan andere objecten koppelen.

Wanneer u nu een van de onderstaande objecten bewerkt, kunt u aangeven of deze actief moeten zijn. Objecten die zijn ingesteld op Actief, worden weergegeven in vervolgkeuzemenu&#39;s en keuzelijsten die kunnen worden gekoppeld aan andere objecten. Objecten die niet op Actief zijn ingesteld, zijn niet zichtbaar in vervolgkeuzemenu&#39;s en keuzelijsten die aan andere objecten moeten worden gekoppeld.

* Goedkeuringsprocessen
* Bedrijven
* Aangepaste Forms
* Mijlpaden
* Portfolio&#39;s
* Programma&#39;s
* Sjablonen

Alles wat u deactiveert en dat momenteel wordt gebruikt, functioneert nog steeds zoals het altijd is, en wordt niet verwijderd of geblokkeerd.

>[!IMPORTANT]
>
>Wanneer u deze objecten maakt via de Workfront API, is de standaardwaarde voor de parameter &quot;isActive&quot; true. Dit is een nieuw veld voor alle objecten en u kunt dit veld niet bewerken vóór versie 11 van de API. Dit veld bestond eerder voor Portfolio, behalve dat de standaardwaarde false was. De standaardwaarde wordt gewijzigd in true, te beginnen met versie 11 van de API.

## De Begrotende Kosten van het Gepland Werk (BCWS) en Geëxporteerde (BCWP) van de vertoning in Mening

U kunt de Gefabriceerde Kosten van Gepland Werk (BCWS) en de Gefabriceerde Kosten van het Gepresteerde Werk (BCWP) in project en taakmeningen nu tonen.

Hoewel deze maatstaven voor projectprestaties al eerder in financiële berekeningen in Workfront werden gebruikt, waren ze vóór deze verbetering niet zichtbaar in het systeem.

Voor informatie over het berekenen van BCWS, zie [ Berekende Gefabriceerde Kosten van Gepland Werk (BCWS) ](../../../../manage-work/projects/project-finances/calculate-bcws.md).

Voor informatie over het berekenen van BCWP, zie [ Begrotende Kosten van het Geprezen Werk berekenen (BCWP) ](../../../../manage-work/projects/project-finances/calculate-bcwp.md).

