---
product-area: reporting
navigation-topic: text-mode-reporting
title: Instructies OR maken in tekstmodusfilters
description: U kunt meerdere instructies opnemen wanneer u een filter maakt in lijsten en rapporten.
author: Nolan
feature: Reports and Dashboards
exl-id: be145e22-d66c-4a74-af0e-8bb0598b4d67
source-git-commit: af4a82ad11b57c7a7457d5d7ee74ee18494a1dc0
workflow-type: tm+mt
source-wordcount: '503'
ht-degree: 0%

---

# Instructies OR maken in tekstmodusfilters

U kunt meerdere instructies opnemen wanneer u een filter maakt in lijsten en rapporten.

Zie de volgende artikelen voor informatie over het maken van filters:

* [&#x200B; Overzicht van Filters &#x200B;](/help/quicksilver/reports-and-dashboards/reports/reporting-elements/filters-overview.md)
* [Een filter bewerken in de tekstmodus](/help/quicksilver/reports-and-dashboards/reports/text-mode/edit-text-mode-in-filter.md)

## Operatoren voor het filter Tekstmodus

Voor informatie over de filterexploitanten van Adobe Workfront in de standaardfilterinterface, zie [&#x200B; Overzicht van Filters &#x200B;](/help/quicksilver/reports-and-dashboards/reports/reporting-elements/filters-overview.md).

Workfront heeft 2 filteroperatoren die elke filterinstructie verbinden:

* **EN**: Wanneer u zich bij 2 filterverklaring door EN exploitant aansluit geeft u aan dat u beide filterverklaringen wilt tezelfdertijd worden ontmoet.

  Standaard worden de instructies in een filter samengevoegd met de operator AND.

  Wanneer het bouwen van EN filter in de interface van de tekstwijze, te hoeven u niet de exploitant AND te gebruiken. Dat wordt aangenomen.

  **Voorbeeld:** om voor taken te filtreren die een Geplande Datum van de Voltooiing van Vandaag hebben en een Percentage voltooide lager dan 100% gebruik de volgende code van de tekstwijze:

  ```
  plannedCompletionDate=$$TODAY
  plannedCompletionDate_Mod=eq 
  percentComplete=100 percent
  Complete_Mod=lt
  ```

* **OF**: Wanneer u zich bij 2 filterverklaringen door OF exploitant aansluit geeft u aan dat u één van beide verklaring wilt worden ontmoet.

  >[!TIP]
  >
  >Wanneer het veranderen van uw EN verklaringen in OF verklaringen, zou het aantal punten in uw rapport moeten stijgen.

  Wanneer het bouw van OF filter gebruikend de interface van de tekstwijze, moet u de exploitant OR gebruiken.

  **Voorbeeld:** om voor taken te filtreren die een Geplande Datum van de Voltooiing van Vandaag of een Percentage Voltooien hebben lager dan 100% gebruik de volgende code van de tekstwijze:

  ```
  plannedCompletionDate=$$TODAY
  plannedCompletionDate_Mod=eq
  OR:1:percentComplete=100
  OR:1:percentComplete_Mod=lt
  ```

## Syntaxis tekstmodus voor OR-filters

De syntaxis van de tekstmodus voor een OR-filter moet het volgende bevatten:

* De operator OR gevolgd door een dubbele punt, een getal en een andere dubbele punt aan het begin van elke filterlijn die naar het object in de instructie OR verwijst. Dit omvat de lijn die verwijzingen het filtergebied of attribuut en de lijn die verwijzingen de filterbepaling.

  Volg dit patroon wanneer het bouwen van een OF filter:

  ```
  <field name in camel case>=<value>
  <field name in camel case>_Mod=<modifier value>
  OR:1:<field name in camel case>=<value>
  OR:1:<field name in camel case>_Mod=<modifier value>
  ```

  >[!TIP]
  >
  >De operator OR is hoofdlettergevoelig en altijd hoofdletters.

  U kunt veelvoudige OF verklaringen in een filter hebben. In dit geval ontvangt elke instructie OR een getal in de volgorde waarin de instructies moeten worden toegepast.

  **Voorbeeld:** om voor taken te filtreren die een Geplande Datum van de Voltooiing van vandaag of een Percentage hebben voltooit lager dan 100% OF een Status van Nieuw gebruik de volgende code van de tekstwijze:

  ```
  plannedCompletionDate=$$TODAY
  plannedCompletionDate_Mod=eq
  OR:1:status=NEW
  OR:1:status_Mod=in
  OR:2:percentComplete=100
  OR:2:percentComplete_Mod=lt
  ```

* De naam van de velden of de kenmerken waarnaar u in een filter verwijst, moet in kameelletters worden geschreven. Voor informatie over camel geval, zie [&#x200B; overzicht van de wijzesyntaxis van de Tekst &#x200B;](../../../reports-and-dashboards/reports/text-mode/text-mode-syntax-overview.md).
* Wanneer u naar aangepaste velden in een OR-filter verwijst, moet u de volgende code invoegen: tussen de syntaxis van de OR-modifier en de naam van het aangepaste veld. U moet de naam van het aangepaste veld spellen zoals deze wordt weergegeven in de Workfront-interface.

  **Voorbeeld:** om voor taken te filtreren die een Status van Nieuw OF een Percentage Volledige lager dan 100% OF een douanegebied genoemd &quot;het Type van Rekening&quot;met een waarde van &quot;Gelijk&quot;hebben, gebruik de volgende code van de tekstwijze:

  ```
  status=NEW
  status_Mod=in
  OR:1:percentComplete=100
  OR:1:percentComplete_Mod=lt
  OR:2:DE:Account Type=Capital
  OR:2:DE:Account Type_Mod=in
  ```
