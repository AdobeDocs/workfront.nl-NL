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
exl-id: fe213fe7-5bb8-479c-926b-761cbdd7ba4e
source-git-commit: f65fbe7ceab19cee75aa0346c389907707c47c8b
workflow-type: tm+mt
source-wordcount: '396'
ht-degree: 0%

---

# Een pakket voor milieubescherming installeren

>[!NOTE]
>
>Als u een pakket wilt installeren, moet u zijn aangemeld bij de omgeving waarin u het pakket wilt installeren. Dit is de omgeving waarin u objecten kopieert **tot**.

1. Ga naar de omgeving waarin u het pakket wilt installeren.
1. Klik op de knop **[!UICONTROL Main Menu]** pictogram ![Hoofdmenu](/help/_includes/assets/main-menu-icon.png) in de rechterbovenhoek van Adobe Workfront of (indien beschikbaar) op de knop **[!UICONTROL Main Menu]** pictogram ![Hoofdmenu](/help/_includes/assets/main-menu-icon-left-nav.png) in de linkerbovenhoek klikt u op **[!UICONTROL Setup]** ![Pictogram Instellen](/help/_includes/assets/gear-icon-setup.png).
1. Selecteren **Systeem** in de linkernavigatie selecteert u vervolgens **Milieubevordering**.
1. Selecteer het pakket in de weergegeven lijst.
1. Voor elk voorwerp dat een botsing heeft, selecteer hoe te om de botsing op te lossen.

   Als u een botsing wilt oplossen, klikt u op de vervolgkeuzepijl naast het objecttype en selecteert u de actie die u wilt uitvoeren.

   Zie voor meer informatie [Botsingdetectie](#collisions) in dit artikel
1. Als u het pakket in de nieuwe omgeving wilt implementeren, klikt u op **Implementeren** rechtsboven in het scherm.

## Botsingdetectie

Er treden botsingen op wanneer een object dat deel uitmaakt van het installatiepakket, al in de doelomgeving bestaat. Wanneer dit voorkomt, kunt u selecteren hoe te om de botsing op te lossen. De botsingen worden opgelost op het objecten niveau.

U kunt botsingen bekijken door op dropdown naast elk objecten type te klikken. De botsingen worden getoond in de kolom van de Botsing.

Om een botsing op te lossen, selecteer een actie in de kolom van de Actie van de Plaatsing, of gebruik de standaardactie die reeds wordt getoond.

* **Maken met nieuwe naam**: Maak een nieuw object in de doelomgeving. Als het object bestaat in de doelomgeving, kunt u een nieuw object met een nieuwe naam maken. Als het niet bestaat in de doelomgeving, kunt u het object maken met een nieuwe naam of met de naam die het object in het pakket heeft.
* **Bestaande gebruiken**: Het object in het pakket is niet geïnstalleerd en het object dat al in de doelomgeving bestond, blijft ongewijzigd.
* **Overschrijven**: Het object in het pakket vervangt het bestaande object in de doelomgeving.
<!--
* Do not use: The object in the package is not installed in the target environment. If you select Do not use, an error message will appear detailing how this choice will affect other objects or fields.
-->

Standaardwaarden zijn `Create new` als het object niet bestaat in de doelomgeving, en `Use existing` als het object wel bestaat in de doelomgeving. U kunt terugkeren naar de standaardtoewijzing door op **Standaardtoewijzing herstellen**.



<!--
## Collisions

A collision occurs when <!--???--.

In Workfront, a potential collision is marked with a blue dot. You can select 

You can select whether to show all package contents, or collisions only.

## Comparison tool

-->
