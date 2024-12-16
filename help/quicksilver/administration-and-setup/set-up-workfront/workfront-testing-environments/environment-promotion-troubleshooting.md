---
user-type: administrator
content-type: overview;how-to-procedural
product-area: system-administration
navigation-topic: workfront-testing-environments
title: Problemen met milieubescherming oplossen
description: Veelvoorkomende problemen met de bevordering van het milieu oplossen.
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: 830dd573-d954-4ba2-a1d3-d1645b3fbac8
source-git-commit: c3c9a423bd60b26b2605a1b52bd706c9bc6acdec
workflow-type: tm+mt
source-wordcount: '328'
ht-degree: 0%

---

# Problemen met milieubescherming oplossen

In dit artikel wordt beschreven hoe u de bevordering van omgevingen kunt oplossen.

## Probleem: Milieubevorderingspakket is aan het stagneren of mislukt

Probeer het volgende als uw pakket voor milieubescherming stagneert of mislukt:

* Als een pakketinstallatie na 10-15 minuten stagneert, of als een pakketinstallatie mislukt, dient u het bestaande pakket opnieuw samen te stellen of een nieuw pakket te maken.

* Als een pakketinstallatie mislukt, kan er een probleem zijn met een of meer objecten. Controleer de foutberichten die het object identificeren en die het probleem kunnen helpen identificeren. Nadat u het probleem met het object hebt opgelost, stelt u het pakket opnieuw samen en probeert u de installatie opnieuw uit.

* Als u nog steeds problemen ondervindt met een installatie, probeert u de installatie te repliceren in een andere doelomgeving. Zo dicht mogelijk bij de oorspronkelijke installatie houden, met inbegrip van objecten en geselecteerde installatiehandelingen.

* We raden u aan de inhoud van het pakket altijd te controleren nadat het pakket is samengesteld om te bevestigen dat het de objecten bevat die u verwacht.


## Probleem: aangepast formulier kan niet worden bevorderd

Dit kan gebeuren omdat het aangepaste formulier een berekend veld bevat. Als een berekend veld verwijst naar een veld waarnaar niet wordt verwezen in een aangepast formulier, wordt een pakket met dit formulier niet bevorderd en ziet de gebruiker mogelijk het volgende bericht:

&quot;De volgende velden zijn ongeldig: Ongeldige aangepaste uitdrukking ongeldige uitdrukking: ongeldige aangepaste uitdrukking.&quot;

Deze kwestie kan zich voordoen wanneer het van verwijzingen voorzien van een bestaand gebied dat niet aan om het even welke douaneformulieren in het doelmilieu, of met een pas gecreeerd gebied in bijlage is.

Voer een van de volgende handelingen uit om dit probleem op te lossen:

* Maak een pakket met een aangepast projecttype dat het veld waarnaar wordt verwezen bevat. Na de bevordering van dit pakket aan het doelmilieu, promoot het oorspronkelijk voorgenomen pakket dat het berekende gebied bevat.
* Maak handmatig het veld waarnaar wordt verwezen in de doelomgeving en koppel dit aan een aangepast projecttype. Nadat dit wordt gedaan, zal het gebied worden erkend, en u kunt het pakket bevorderen zonder de fout te ontmoeten.
