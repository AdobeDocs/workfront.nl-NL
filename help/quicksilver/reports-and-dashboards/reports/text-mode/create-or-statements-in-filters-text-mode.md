---
product-area: reporting
navigation-topic: text-mode-reporting
title: Instructies "OR" maken in tekstmodusfilters
description: U kunt meerdere instructies opnemen wanneer u een filter maakt in lijsten en rapporten.
author: Nolan
feature: Reports and Dashboards
exl-id: be145e22-d66c-4a74-af0e-8bb0598b4d67
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '566'
ht-degree: 0%

---

# Instructies &quot;OR&quot; maken in tekstmodusfilters

U kunt meerdere instructies opnemen wanneer u een filter maakt in lijsten en rapporten.

Zie de volgende artikelen voor informatie over het maken van filters:

* [Overzicht van filters in Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md)
* [Een filter bewerken in de tekstmodus](../../../reports-and-dashboards/reports/text-mode/edit-text-mode-in-filter.md)

## Operatoren voor het filter Tekstmodus

Voor informatie over Adobe Workfront-filteroperatoren in de standaardfilterinterface raadpleegt u [Overzicht van filters in Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md).

Workfront heeft 2 filteroperatoren die elke filterinstructie verbinden:

* **EN**: Wanneer u zich bij 2 filterverklaring door de exploitant van AND aansluit, wijst u erop dat u beide filterverklaringen wilt tezelfdertijd ontmoeten.

   Standaard worden de instructies in een filter samengevoegd met de operator AND.

   Wanneer het bouwen van EN filter in de interface van de tekstwijze, te hoeven u niet de exploitant AND te gebruiken. Dat wordt aangenomen.

   **Voorbeeld:** Als u wilt filteren voor taken met een geplande Voltooiingsdatum van vandaag en een percentage voltooid van minder dan 100%, gebruikt u de volgende code voor de tekstmodus:

   <pre>scheduledCompletionDate=$$TODAY</pre><pre>scheduledCompletionDate_Mod=eq</pre><pre>percentComplete=100</pre><pre>percentComplete_Mod=lt</pre>

* **OF**: Wanneer u 2 filterinstructies door de operator OR samenvoegt, geeft u aan dat aan een van beide instructies moet worden voldaan.

   >[!TIP]
   >
   >Wanneer het veranderen van uw EN verklaringen in OF verklaringen, zou het aantal punten in uw rapport moeten stijgen.

   Wanneer het bouw van OF filter gebruikend de interface van de tekstwijze, moet u de exploitant OR gebruiken.

   **Voorbeeld:** Als u wilt filteren voor taken met een geplande voltooiingsdatum van vandaag of een percentage voltooid dat lager is dan 100%, gebruikt u de volgende code voor de tekstmodus:

   <pre>scheduledCompletionDate=$$TODAY</pre><pre>scheduledCompletionDate_Mod=eq</pre><pre>OF:1:percentComplete=100</pre><pre>OF:1:percentComplete_Mod=lt</pre>

## Syntaxis tekstmodus voor OR-filters

De syntaxis van de tekstmodus voor een OR-filter moet het volgende bevatten:

* De operator OR gevolgd door een dubbele punt, een getal en een andere dubbele punt aan het begin van elke filterlijn die naar het object in de instructie OR verwijst. Dit omvat de lijn die verwijzingen het filtergebied of attribuut en de lijn die verwijzingen de filterbepaling.

   Volg dit patroon wanneer het bouwen van een OF filter:

   <pre><field name in camel case>=<value></pre><pre><field name in camel case>_Mod=<modifier value></pre><pre>OF:1:<field name in camel case>=<value></pre><pre>OF:1:<field name in camel case>_Mod=<modifier value></pre>

   >[!TIP]
   >
   >De operator OR is hoofdlettergevoelig en altijd hoofdletters.

   U kunt veelvoudige OF verklaringen in een filter hebben. In dit geval ontvangt elke instructie OR een getal in de volgorde waarin de instructies moeten worden toegepast.

   **Voorbeeld:**  Als u wilt filteren voor taken met een geplande voltooiingsdatum van vandaag OF een gepland percentage van 100% voltooid OF een status van Nieuw, gebruikt u de volgende code voor de tekstmodus:

   <pre>scheduledCompletionDate=$$TODAY</pre><pre>scheduledCompletionDate_Mod=eq</pre><pre>OF:1:status=NEW</pre><pre>OF:1:status_Mod=in</pre><pre>OF:2:percentComplete=100</pre><pre>OF:2:percentComplete_Mod=lt</pre>

* De naam van de velden of de kenmerken waarnaar u in een filter verwijst, moet in kameelletters worden geschreven. Voor informatie over kamelendoosjes raadpleegt u [Overzicht van syntaxis in tekstmodus](../../../reports-and-dashboards/reports/text-mode/text-mode-syntax-overview.md).
* Wanneer u naar aangepaste velden in een OF-filter verwijst, moet u DE invoegen: tussen de syntaxis van de optie OR en de naam van het aangepaste veld. U moet de naam van het aangepaste veld spellen zoals deze wordt weergegeven in de Workfront-interface.

   **Voorbeeld:** Als u wilt filteren op taken met de status Nieuw OF Percentage voltooid lager dan 100% OF met een aangepast veld genaamd Accounttype met de waarde Gelijk, gebruikt u de volgende code voor de tekstmodus:

   <pre>status=NEW</pre><pre>status_Mod=in</pre><pre>OF:1:percentComplete=100</pre><pre>OF:1:percentComplete_Mod=lt</pre><pre>OF:2:DE:Accounttype=Capital</pre><pre>OF:2:DE:Accounttype_Mod=in</pre>
