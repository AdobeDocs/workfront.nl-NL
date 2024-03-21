---
user-type: administrator
content-type: how-to-procedural
product-area: system-administration
navigation-topic: workfront-testing-environments
title: Een pakket voor milieubescherming installeren
description: Het milieu bevorderend vermogen is bedoeld om de capaciteit te verstrekken om op configuratie betrekking hebbende voorwerpen van één milieu aan een andere te bewegen. Leer hoe u een milieupromotiepakket in een doelomgeving installeert.
author: Becky
feature: System Setup and Administration
role: Admin
hide: true
hidefromtoc: true
recommendations: noDisplay, noCatalog
source-git-commit: 610469811a937fde70a938af829b156e69cca391
workflow-type: tm+mt
source-wordcount: '352'
ht-degree: 0%

---

# Een pakket voor milieubescherming installeren


1. Ga naar de omgeving waarin u het pakket wilt installeren. Dit is de omgeving waarin u objecten kopieert **tot**.
1. Klik op de knop **[!UICONTROL Main Menu]** pictogram ![Hoofdmenu](/help/_includes/assets/main-menu-icon.png) in de rechterbovenhoek van Adobe Workfront of (indien beschikbaar) op de knop **[!UICONTROL Main Menu]** pictogram ![Hoofdmenu](/help/_includes/assets/main-menu-icon-left-nav.png) in de linkerbovenhoek klikt u op **[!UICONTROL Setup]** ![Pictogram Instellen](/help/_includes/assets/gear-icon-setup.png).
1. Selecteren **Systeem** in de linkernavigatie selecteert u vervolgens **Milieubevordering**.
1. Selecteer het pakket in de weergegeven lijst.
1. Klik op **Installeren** rechtsboven in het scherm.
1. Wijs elk object in het pakket toe aan het corresponderende object in de doelomgeving.

   Zie voor meer informatie [Toewijzing](#mapping) in dit artikel


## Toewijzing

Elk objecttype wordt weergegeven in de linkernavigatie en op een kaart. De kaart geeft objecten van dat type weer en geeft aan of deze objecten in de doelomgeving aanwezig zijn. U kunt bepalen hoe deze objecten naar de doelomgeving worden verplaatst.

* Nieuw maken: maak een nieuw object in de doelomgeving. Als het object bestaat in de doelomgeving, kunt u een nieuw object met een nieuwe naam maken. Als het niet bestaat in de doelomgeving, kunt u het object maken met een nieuwe naam of met de naam die het object in het pakket heeft.
* Bestaande gebruiken: het object in het pakket is niet geïnstalleerd en het object dat al in de doelomgeving bestond, blijft ongewijzigd.
* Overschrijven: (momenteel niet beschikbaar) Het object in het pakket vervangt het bestaande object in de doelomgeving.
* Niet gebruiken: het object in het pakket is niet geïnstalleerd in de doelomgeving. Als u Niet gebruiken selecteert, wordt een foutbericht weergegeven waarin wordt aangegeven hoe deze keuze van invloed is op andere objecten of velden.

Standaardwaarden zijn `Create new` als het object niet bestaat in de doelomgeving, en `Use existing` als het object wel bestaat in de doelomgeving. U kunt terugkeren naar de standaardtoewijzing door op **Standaardtoewijzing herstellen**.



<!--
## Collisions

A collision occurs when <!--???--.

In Workfront, a potential collision is marked with a blue dot. You can select 

You can select whether to show all package contents, or collisions only.

## Comparison tool

-->
