---
title: Workfront-objecten maken met Workfront Planning Record-automatisering
description: U kunt automatiseringen in de Planning van Workfront vormen die, wanneer geactiveerd, tot voorwerpen in Workfront leiden.
feature: Workfront Planning
role: User, Admin
author: Alina, Becky
recommendations: noDisplay, noCatalog
source-git-commit: bac3ed2a169e070b541192ab312d4fc1a1b467d1
workflow-type: tm+mt
source-wordcount: '386'
ht-degree: 0%

---


# Workfront-objecten maken met Workfront Planning Record-automatisering

U kunt automatiseringen in de Planning van Workfront vormen die, wanneer geactiveerd, tot voorwerpen in Workfront leiden.

U activeert de automatisering in verslagen. Het object in Workfront is verbonden met de planningsrecord waarin u de automatisering hebt geactiveerd.

U kunt bijvoorbeeld een automatisering maken die een Workfront-planningscampagne voert en een project maakt in Workfront om de voortgang van die campagne te volgen. Het project zou worden gekoppeld aan de planningscampagne van Workfront.

Voor meer informatie over verbonden verslagen, zie [ Verbonden verslagenoverzicht ](/help/quicksilver/planning/records/connected-records-overview.md).


## Automatisering configureren in Workfront-planning

U moet een automatisering in de Planning van Workfront vormen alvorens u het kunt gebruiken om voorwerpen van Workfront tot stand te brengen.

1. Klik **Meer** menu ![](assets/more-menu.png) en selecteer **Automaties**.

   De lijst met beschikbare automatiseringen wordt geopend.

1. Klik **creëren nieuwe automatisering** in de hoger-juiste hoek van het scherm.
1. Op het **gebied van de Tekst van de Knoop**, ga de tekst in die u op de knoop wilt verschijnen. Gebruikers klikken op deze knop wanneer ze de automatisering gebruiken om een Workfront-object te maken.
1. (Optioneel) Als u een pictogram aan de knop wilt toevoegen, selecteert u een pictogram uit de beschikbare opties.
1. Op **creeer een type van** gebied, selecteer het voorwerp dat u de automatisering wilt tot stand brengen.

   Beschikbare objecten zijn:

   * Project
   * Portfolio
   * Programma
   * Groep

1. Op **selecteer het gebied op het gebied van de projectnaam** te gebruiken, selecteer een verslaggebied. Het nieuwe project in Workfront heeft de inhoud van dit veld als naam.
1. Op **selecteer het gebied om het gecreeerde project terug** gebied te verbinden, selecteer een verslaggebied. Het nieuwe project in Workfront wordt in dit veld weergegeven wanneer u de record weergeeft in Workfront Planning.
1. Selecteer andere opties die beschikbaar zijn voor het type object dat u maakt.
1. Klik **creëren**

De automatisering wordt weergegeven in de lijst met automatiseringen en is beschikbaar voor gebruik in records.

## Een Workfront-planningsautomatisering gebruiken om een Workfront-object te maken

1. Open in Workfront Planning de pagina met recordtypen die de records bevat die u wilt gebruiken om Workfront-objecten te maken.
1. Selecteer een of meer records.
1. Klik op de automatiseringsknop in de rechterbenedenhoek van het scherm.

   In dit voorbeeld is dit de knop Project maken.

   ![ knoop van de Automatisering ](assets/automation-custom-button.png)

>[!NOTE]
>
>We raden u aan te controleren of het object is gemaakt en verbonden zoals u had verwacht.
