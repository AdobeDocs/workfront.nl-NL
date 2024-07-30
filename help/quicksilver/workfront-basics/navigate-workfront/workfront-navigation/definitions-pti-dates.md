---
content-type: reference
navigation-topic: workfront-navigation
title: Overzicht van het Project, de Taak, en de data van de Uitgave in  [!DNL Workfront]
description: Dit artikel verstrekt definities aan de gemeenschappelijkste data verbonden aan projecten, taken, en kwesties in  [!DNL Adobe Workfront].
feature: Get Started with Workfront
author: Alina
exl-id: 3808200f-a573-4c39-8965-b254f69c893c
source-git-commit: 6f1f669f7e2235637864a92a40aadbfb19b4310b
workflow-type: tm+mt
source-wordcount: '2070'
ht-degree: 0%

---

# Overzicht van de project-, taak- en uitgiftedatums in [!DNL Workfront]

<!-- Audited: 05/2024 -->

<!--consider expanding on this article with ALL dates for PTIs - Hand off dates, Approval Dates, etc-->

<!-- there are dates below that need definition - ask Product-->

Dit artikel bevat definities voor de meest gebruikte datums voor projecten, taken en problemen in [!DNL Adobe Workfront] . De afbeeldingen die hier worden weergegeven, zijn voorbeelden van plaatsen waar de datums in Workfront worden weergegeven en zijn niet uitputtend. Er zijn andere gebieden die de datums weergeven. Alle datums zijn ook zichtbaar in project-, taak- en uitgifterapporten en lijsten.

Zie de volgende artikelen voor informatie over rapporten en lijsten:

* [Aan de slag met lijsten in  [!DNL Adobe Workfront]](../../../workfront-basics/navigate-workfront/use-lists/view-items-in-a-list.md)
* [Aan de slag met rapporten](../../../reports-and-dashboards/reports/reporting/get-started-reports-workfront.md)

Voor meer informatie over project, taak, en geven gebieden uit, zie [ Verklarende woordenlijst van  [!DNL Adobe Workfront]  terminologie ](../../../workfront-basics/navigate-workfront/workfront-navigation/workfront-terminology-glossary.md).


## [!UICONTROL Actual Start Date]

De [!UICONTROL Actual Start Date] is de datum waarop een gebruiker begint te werken aan een project, taak of uitgave. [!UICONTROL Actual Start Date] is leeg wanneer het project, de taak, of de kwestie wordt gecreeerd.

U kunt handmatig aangeven wanneer het werk aan een taak of een uitgave is begonnen, of de code [!UICONTROL Actual Start Date] wordt automatisch ingevuld wanneer de taak of de status van de uitgave verandert van [!UICONTROL New] in [!UICONTROL In Progress] of [!UICONTROL Complete] . De [!UICONTROL Actual Start Date] van een project valt samen met de datum waarop de eerste taak van het project wordt gestart.

>[!TIP]
>
>De [!UICONTROL Actual Start Date] komt mogelijk niet overeen met een [!UICONTROL Planned Start Date] van een project, taak of uitgave omdat de gebruiker later of eerder kan beginnen met werken dan de geplande datum.

Voor meer informatie, zie [ Overzicht van het project [!UICONTROL Actual Start Date]](../../../manage-work/projects/planning-a-project/project-actual-start-date.md).

>[!NOTE]
>
>De [!UICONTROL Must Start On] -taak of de Vaste datumbeperkingen hebben invloed op de [!UICONTROL Planned Start Date] -status van een taak, niet op de [!UICONTROL Actual Start Date] -taak. Hiermee werkt u [!UICONTROL Planned Start Date] bij naar een datum die u opgeeft. [!UICONTROL Actual Start Date] wordt onafhankelijk van [!UICONTROL Planned Start Date] bijgewerkt, zoals hierboven beschreven.

![](assets/actual-start-date-on-edit-task-highlighted-nwe-350x251.png)

![](assets/actual-start-date-on-task-details-highlighted-nwe-350x191.png)

## [!UICONTROL Actual Completion Date]

De [!UICONTROL Actual Completion Date] is de datum waarop een gebruiker een project, taak of uitgave voltooit. [!UICONTROL Actual Completion Date] is leeg wanneer het project, de taak, of de kwestie wordt gecreeerd.

U kunt handmatig aangeven wanneer een taak of een probleem is voltooid. [!UICONTROL Actual Completion Date] wordt automatisch ingevuld wanneer een van de volgende gebeurtenissen plaatsvindt:

* De project-, taak- of uitgiftestatus verandert in [!UICONTROL Complete] , [!UICONTROL Closed] of [!UICONTROL Resolved] .
* De taak of het projectpercentage voltooid is 100%.

[!UICONTROL Actual Completion Date] van een project valt samen met de datum waarop u de laatste taak van het project hebt voltooid.

>[!TIP]
>
>De [!UICONTROL Actual Completion Date] komt mogelijk niet overeen met de [!UICONTROL Planned Completion Date] .

Voor meer informatie, zie [ Overzicht van het project [!UICONTROL Actual Completion Date]](../../../manage-work/projects/planning-a-project/project-actual-completion-date.md).

![](assets/actual-completion-date-task-details-highlighted-nwe-350x189.png)

## Voltooiingsdatum goedkeuringspad

De datum van de Voltooiing van de Weg van de Goedkeuring is de datum toen de goedkeuring van een project, een taak, of een kwestie werd verleend en de Status van het punt werd veranderd.

De datum van de Voltooiing van de Weg van de Goedkeuring is zichtbaar in project, taak, en geeft lijsten en rapporten uit.

## Begindatum goedkeuringspad

De Datum van het Begin van de Weg van de Goedkeuring is de datum toen het project, de taak, of de Uitgiftestatus in &quot;In afwachting van goedkeuring&quot;werd veranderd en het verzoek van de projectgoedkeuring werd verzonden naar de fiatteurs.

De Datum van het Begin van de Weg van de Goedkeuring is zichtbaar in project, taak, en geeft lijsten en rapporten uit.

<!--## Auto Closure Date -->

## Datum van geplande voltooiing

Dit is een verouderd gebied voor projecten. Alle informatie die in dit veld in een lijst of rapport wordt weergegeven, is gerelateerd aan een functie die door Workfront is verwijderd. Dit veld kan niet worden bijgewerkt.

Het gebied is zichtbaar in projectrapporten en lijsten.

## Begindatum van begroting

Dit is een verouderd gebied voor projecten. Alle informatie die in dit veld wordt weergegeven, is gerelateerd aan een functie die door Workfront is verwijderd. Dit veld kan niet worden bijgewerkt.

Het gebied is zichtbaar in projectrapporten en lijsten.

## [!UICONTROL Commit Date]

[!UICONTROL Commit Date] is de datum waardoor een gebruiker die aan een taak of een kwestie wordt toegewezen de taak of de kwestie verbindt te voltooien. Dit is anders dan de [!UICONTROL Planned Completion Date] , omdat het een realistischere schatting is van de voltooiingsdatum die alleen wordt gegeven door de gebruiker die verantwoordelijk is voor het werk. Zie [[!UICONTROL Commit Date] overview ](../../../manage-work/projects/updating-work-in-a-project/overview-of-commit-dates.md) voor meer informatie.

>[!NOTE]
>
>Het wijzigen van [!UICONTROL Commit Date] heeft invloed op de [!UICONTROL Projected Completion Date] maar niet op de [!UICONTROL Planned Completion Date] van een taak of een probleem. De projectmanager kan de wijzigingen die een toegewezen persoon aanbrengt in [!UICONTROL Commit Date] gebruiken om de [!UICONTROL Planned Completion Date] van een taak of een uitgave bij te werken.

<!--## Completion Pending Date-->

## Restrictiedatum

Als u een Restrictie van de Taak gebruikt die aan een specifieke datum gebonden is, dan wordt die specifieke datum de Datum van de Restrictie van de taak.

De volgende taakbeperkingen werken het gebied van de Datum van de Beperking bij:

* Moet beginnen op
* Moet worden voltooid op
* Niet later starten dan
* Niet eerder starten dan

>[!TIP]
>
>Een taak met een beperking van Vaste datums heeft geen Restrictiedatum.
>

De datum van de Beperking is zichtbaar in een taaklijst of een rapport.

## Invoerdatum van geconverteerde uitgave

De datum waarop de uitgave die in het project of de taak werd omgezet werd gecreeerd.

De Omgezette Datum van de Ingang van de Uitgave is zichtbaar in project en taaklijsten en rapporten.

## Vervaldatum

De datum waarop een taak of een kwestie moet worden voltooid. De vervaldatum van een taak of uitgifte is dezelfde datum als de geplande afsluitende datum.

De taak en het Eind van de uitgave zijn zichtbaar in taak en geeft lijsten en rapporten uit.

Voor informatie, zie de [ Geplande sectie van de Datum van de Voltooiing ](#planned-completion-date) in dit artikel.

## Verwacht op

De datum waarop het project moet worden voltooid. De vervaldatum van een project is dezelfde datum als de geplande uitvoeringsdatum van het project.

De op datum verouderde projectdatum is zichtbaar in projectlijsten en rapporten.

Voor informatie, zie de [ Geplande sectie van de Datum van de Voltooiing ](#planned-completion-date) in dit artikel.

## [!UICONTROL Entry Date]

De [!UICONTROL Entry Date] is de datum waarop een project, taak of uitgave is gemaakt in [!DNL Workfront] .

De instructie [!UICONTROL Entry Date] heeft geen invloed op de tijdlijn van projecten, taken of problemen, maar is wel belangrijk voor het bijhouden en rapporteren van gegevens. [!DNL Workfront] genereert automatisch [!UICONTROL Entry Date] wanneer het object wordt gemaakt en u kunt het niet handmatig bewerken.

![](assets/entry-date-in-task-details-highlighted-nwe.png)

## Geschatte vervaldatum

De geplande einddatum van de taak en het project geeft een realistischere datum aan waarop het project of de taak moet worden voltooid.

De geschatte data zijn meer in overeenstemming met de realiteit van het project en de taak, aangezien ze rekening houden met wat van invloed is op de daadwerkelijke voltooiing van het project of de taak. De geschatte vervaldata zijn vergelijkbaar met de verwachte sluitingsdata.

Voor meer informatie, zie [ Overzicht van Geprojecteerde en Geschatte Data ](/help/quicksilver/manage-work/tasks/task-information/differentiate-projected-estimated-dates.md).

Het project en de taak Geschatte Vervaldata zijn zichtbaar in project en taaklijsten en rapporten.

## Geschatte begindatum

De taak en het project Geschatte Datum van het Begin tonen een realistischere datum van wanneer het project of de taak kon beginnen.

De geschatte data zijn meer in overeenstemming met de realiteit van het project en de taak, aangezien ze rekening houden met wat van invloed is op de daadwerkelijke start van het project of de taak. De geschatte begindatums zijn vergelijkbaar met de verwachte begindatums.

Voor meer informatie, zie [ Overzicht van Geprojecteerde en Geschatte Data ](/help/quicksilver/manage-work/tasks/task-information/differentiate-projected-estimated-dates.md).

Het project en de taak Geschatte Datums van het Begin zijn zichtbaar in project en taaklijsten en rapporten.

<!--## Exchange Rate Date-->

## Vaste einddatum

De projectaanvrager of eigenaar identificeert de vaste einddatum van een project wanneer het bedrijfscase wordt voltooid. Het is de datum waarop zij aanbevelen dat het project moet worden voltooid.

Dit is een handmatige schatting en er wordt geen rekening gehouden met de werkelijke voortgang van de taken van het project.

De Vaste Datum van het Eind van een project is zichtbaar in de Van Bedrijfs het Geval sectie van het project evenals in projectlijsten en rapporten.

![](assets/fixed-end-date-business-case-highlight.png)

## Vaste begindatum

De projectaanvrager of eigenaar identificeert de Vaste Begindatum van een project wanneer de bedrijfscase wordt voltooid. Het is de datum waarop zij aanbevelen het project te starten.

Dit is een handmatige schatting en er wordt geen rekening gehouden met de werkelijke voortgang van de taken van het project.

De Vaste Datum van het Begin van een project is zichtbaar in de Van Bedrijfs het Geval sectie van het project evenals in projectlijsten en rapporten.

![](assets/fixed-start-date-business-case-highlight.png)

## Handoff-datum

De datum waarop een taak beschikbaar wordt voor het werk. Dit betekent dat alle beperkingen, goedkeuringen en afhankelijkheden zijn voltooid en dat gebruikers aan de taak kunnen beginnen te werken.

De afhandelingsdatum is een berekening en kan niet handmatig worden ingesteld.

Voor meer informatie over de Datum van de Aflevering, zie [ Overzicht van de Datum van de Aflevering van de Taak ](/help/quicksilver/manage-work/tasks/task-information/handoff-task-date.md).

De Handoff Datum van een taak is zichtbaar in taaklijsten en rapporten.

## Datum laatste financiële update

De datum waarop de financiële informatie over een project is bijgewerkt. Dit omvat het bijwerken van financiële gebieden in de sectie Financiën of de sectie Bedrijfs-case van het project.

De laatste Datum van de Update van de Financiën is zichtbaar in projectlijsten en rapporten.

## Datum laatste update

De datum waarop het project, de taak of de uitgave voor het laatst is bijgewerkt. Een update wordt beschouwd als elke wijziging die een project, taak of uitgave activeert die moet worden opgeslagen. Dit omvat wijzigingen in status, toestand, tijdlijn, financiën of andere gebieden.

De laatste Datum van de Update is zichtbaar in project, taak, en uitgiftenlijsten en rapporten.

## [!UICONTROL Hour Entry Date]

Wanneer u tijd voor projecten, taken, en kwesties registreert om erop te wijzen hoeveel daadwerkelijke tijd (in uren) u het werken aan het project, de taak, of de kwestie doorbrengt, wordt de tijd u het logboek [!UICONTROL Actual Hours] van het project, de taak, of de kwestie.

De datum waarvoor u de tijd registreert is het [!UICONTROL Hour Entry Date] gebied op de uuringang.

De Datum van de Ingang van het Uur is zichtbaar in uurlijsten en rapporten.

>[!TIP]
>
>De waarde [!UICONTROL Entry Date] van een uur is anders dan de waarde [!UICONTROL Entry Date] van een ander Workfront-object. Dit is namelijk niet de datum waarop het uurlog is gemaakt, maar de datum waarop de uren moeten worden gekoppeld.
>
>U kunt bijvoorbeeld uren voor een taak op 5 september vastleggen, maar de uren koppelen aan 1 september. De ingangsdatum van het uur is 1 september.

Voor informatie over hoe te om tijd in Workfront te registreren, zie [ tijd van het Logboek ](../../../timesheets/create-and-manage-timesheets/log-time.md).

>[!TIP]
>
>Wij adviseren registrerentijd op het werken taken en kwesties, eerder dan oudertaken of projecten. De tijd die op de het werk taken wordt geregistreerd rolt omhoog aan de oudertaken en het project als [!UICONTROL Actual Hours] voor de oudertaken en het project. De tijd die op kwesties wordt geregistreerd rolt omhoog aan het project als [!UICONTROL Actual Hours] voor het project.

## [!UICONTROL Planned Completion Date]

De [!UICONTROL Planned Completion Date] - of [!UICONTROL Due On] -datum is de datum waarop een project, taak of uitgave moet worden voltooid.

Afhankelijk van de instructie [!UICONTROL Task Constraint] kunt u de [!UICONTROL Planned Completion Date] van een taak mogelijk niet bewerken. Afhankelijk van [!UICONTROL Schedule Mode] van het project, kunt u [!UICONTROL Planned Completion Date] van een project misschien niet uitgeven.

[!UICONTROL Planned Completion Date] wordt in bepaalde gebieden van [!DNL Workfront] weergegeven als de datum Verouderd.

Raadpleeg de volgende artikelen voor meer informatie:

* [Overzicht van de taak [!UICONTROL Planned Completion Date]](../../../manage-work/tasks/task-information/task-planned-completion-date.md)
* [Het project instellen [!UICONTROL Planned Completion Date]](../../../manage-work/projects/planning-a-project/project-planned-completion-date.md)
* [Overzicht van het probleem [!UICONTROL Planned Completion Date]](../../../manage-work/issues/issue-information/issue-planned-completion-date.md)

![](assets/project-header-planned-completion-date-highlighted-nwe-350x34.png)

![](assets/planned-completion-date-in-task-list-highlighted-nwe-350x183.png)


## Geplande datumuitlijning

Dit is een automatische indicator dat Workfront projecten, taken, en kwesties toewijst om te tonen wanneer een punt met betrekking tot zijn Geplande Datum van de Voltooiing zal worden voltooid.

Hieronder vindt u mogelijke waarden voor de indicator voor het uitlijnen van de geplande datum:

* Wordt uitgevoerd op de geplande einddatum
* Wordt uitgevoerd vóór de geplande einddatum
* Wordt uitgevoerd na de geplande einddatum

De geplande datumuitlijning is zichtbaar in project-, taak- en uitgiftenlijsten en -rapporten.

## [!UICONTROL Planned Start Date]

De [!UICONTROL Planned Start Date] is de datum waarop een project, taak of uitgave moet worden gestart.

Afhankelijk van de instructie [!UICONTROL Task Constraint] kunt u de [!UICONTROL Planned Start Date] van een taak mogelijk niet bewerken. Afhankelijk van [!UICONTROL Schedule Mode] van het project, kunt u [!UICONTROL Planned Start Date] van een project misschien niet uitgeven.

Voor meer informatie, zie [ Overzicht van het project [!UICONTROL Planned Start Date]](../../../manage-work/projects/planning-a-project/project-planned-start-date.md).

![](assets/planned-start-date-on-edit-task-highlighted-nwe.png)

![](assets/planned-start-date-in-task-list-highlighted-nwe-350x167.png)

## [!UICONTROL Projected Completion Date]

[!UICONTROL Projected Completion Date] is een real-time, berekende indicator van wanneer het project, de taak, of de kwestie zullen worden voltooid. Wanneer het project, de taak of de uitgave is gemarkeerd als Voltooid, verandert [!UICONTROL Projected Completion Date] in de datum van [!UICONTROL Actual Completion Date] .

Als alles vloeiend en volgens plan verloopt, moet de [!UICONTROL Projected Completion date] overeenkomen met de [!UICONTROL Planned Completion Date] . Anders kan de [!UICONTROL Projected Completion Date] anders worden dan de [!UICONTROL Planned Completion Date] vanwege vertragingen bij de voorgaande taken.

Voor meer informatie, zie [ Overzicht van [!UICONTROL Projected Completion Date] voor projecten, taken, en kwesties ](../../../manage-work/projects/planning-a-project/project-projected-completion-date.md).

![](assets/projected-completion-date-in-task-details-highlighted-nwe-350x187.png)

## [!UICONTROL Projected Start Date]

[!UICONTROL Projected Start Date] is een datum in real time van wanneer het project, de taak, of de kwestie begint en rekening houdt met alle vertragingen. Dit is een nauwkeurigere Begindatum voor het project, de taak of het probleem dan de [!UICONTROL Planned Start Date] . In [!UICONTROL Planned Start Date] wordt geen rekening gehouden met vertragingen of datums uit het verleden.

Wanneer u een project de eerste keer plant, zijn de [!UICONTROL Planned Start Date] en [!UICONTROL Projected Start Date] van de taken en van het project identiek. Aangezien vertragingen kunnen optreden of taken eerder kunnen worden voltooid, kan [!UICONTROL Projected Start Date] anders worden dan [!UICONTROL Planned Start Date] .

Voor een taak kan een [!UICONTROL Projected Start Date] ook afwijken van de [!UICONTROL Planned Start Date] wanneer een van de voorgangers achter het schema wordt uitgevoerd.

>[!TIP]
>
>U kunt de [!UICONTROL Projected Start Date] van een probleem alleen in een lijst of rapport bekijken.

Voor meer informatie, zie [ Overzicht van het project [!UICONTROL Projected Start Date]](../../../manage-work/projects/planning-a-project/project-projected-start-date.md).

![](assets/projected-start-date-in-task-details-highlighted-nwe-350x188.png)

<!--## Rejection Date-->

## Datum Slack

Taken kunnen soms worden gestart en laat worden voltooid zonder dat dit gevolgen heeft voor de Voltooiingsdatum van het project.

De datum van de Slack toont de nauwkeurige datum wanneer een taak de Datum van de Voltooiing van het project beslist zou kunnen beïnvloeden.

Voor informatie over de Datum van de Slack van een taak, zie [ Overzicht van de Datum van de Slack van de Taak ](/help/quicksilver/manage-work/tasks/task-information/task-slack-date.md).

De Datums van de Slack van de taak zijn zichtbaar in taaklijsten en rapporten.

## Starten bij

De datum waarop het project van start gaat. De begindatum van een project is dezelfde datum als de geplande begindatum van het project.

Dit gebied is zichtbaar in projectlijsten en rapporten.

Voor informatie, zie de [ Geplande 1} sectie van de Datum van het Begin {in dit artikel.](#planned-start-date)



