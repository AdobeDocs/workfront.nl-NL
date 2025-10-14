---
content-type: overview;how-to-procedural
product-area: projects
navigation-topic: financials
title: Prestatie-index (CSI) voor kostenplanning berekenen
description: De prestatie-index van het kostenschema (CSI) is een automatische berekening waarbij de kostenprestatie-index (CPI) en de prestatie-index (SPI) van het schema worden gecombineerd tot één algemene maatstaf die de kosten en het tijdschema in evenwicht brengt.
author: Lisa
feature: Work Management
exl-id: 38a8c5e0-b812-499d-8fe7-a71ddccb3aad
source-git-commit: abf5f21281b05dedfecbe71c6ffbf54ee69e2460
workflow-type: tm+mt
source-wordcount: '331'
ht-degree: 0%

---

# Prestatie-index (CSI) voor kostenplanning berekenen

<!-- Audited: 6/2025 -->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: Linked to the product. Do not change link.) </p>
-->

## Overzicht van de prestatie-index voor kostenplanning (CSI)

De prestatie-index van het kostenschema (CSI) is een automatische berekening waarbij de kostenprestatie-index (CPI) en de prestatie-index (SPI) van het schema worden gecombineerd tot één algemene maatstaf die de kosten en het tijdschema in evenwicht brengt. Door deze waarden samen te vermenigvuldigen, kan één enkele metrisch een langdurig programma bij een lager budget of vice versa verklaren. De managers van het project kunnen dit gebruiken om algemene project of taakgezondheid te bepalen wanneer de kosten worden opgeofferd om planning midden-project te drijven.

>[!TIP]
>
>Adobe Workfront berekent CSI voor zowel taken als projecten, maar niet kwesties.

U kunt van de informatie profiteren die door dit metrisch wordt verstrekt slechts als de volgende scenario&#39;s in uw organisatie bestaan:

* Uw gebruikers registreren tijd voor het werk zij voltooien. Dit berekent CSI gebaseerd op Uren.
* Uw gebruikers of baanrollen hebben Kosten per Uur verbonden aan hen. Dit berekent CSI op basis van kosten.

## Hoe Workfront de Performance Index (CSI) van het Kostenschema berekent

Workfront berekent de Kostenprestatie-index (CSI) van een project of taak aan de hand van de volgende formule:

`CSI = CPI x SPI`

Voor informatie over CPI, zie het artikel [&#x200B; Berekent de Index van de Prestaties van Kosten (CPI) &#x200B;](../../../manage-work/projects/project-finances/calculate-cpi.md).

Voor informatie over SPI, zie het artikel [&#x200B; de Index van de Prestaties van het Programma berekenen (SPI) &#x200B;](../../../manage-work/projects/project-finances/calculate-spi.md).

CSI heeft de volgende drie mogelijke waarden:

* 1 = Volgt het algemene plan
* \>1 = Combinatie van begrotingsprogramma
* &lt;1 = combinatie van begrotingsschema voor overschrijden

![&#x200B; CSI &#x200B;](assets/csi-highlighted.png)

## Zoek de Performance Index (CSI) voor kostenplanning

>[!CAUTION]
>
>U moet toegang tot de Gegevens van de Mening Financiële in uw Niveau van de Toegang en toestemmingen hebben om het project of de taak te bekijken om de waarde CSI van een project of een taak te zien.

U kunt CSI vinden in de volgende gebieden van Workfront:

* Financieringsgebied in de sectie Projectdetails.
* Het gebied van de financiën in de sectie van de Details van de Taak.
* Een project- of taakweergave.
* Een project- of taakrapport.
