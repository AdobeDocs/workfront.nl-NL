---
product-area: templates
navigation-topic: templates-navigation-topic
title: Overzicht van start- en voltooiingsdagen in een sjabloon
description: U kunt projectmalplaatjes gebruiken om de meeste herhaalbare processen, informatie, en montages te vangen verbonden aan de projecten in uw organisatie. Hoewel projecten specifieke start- en voltooiingsdatums hebben, hebben sjablonen algemene start- en voltooiingsdagen als indicatie voor de plaats waar deze data op het project zullen vallen, op basis van de algemene tijdslijn van het project.
author: Alina
feature: Work Management
exl-id: caa0e7b1-37c3-4973-92ce-cc93df4e4186
source-git-commit: dbc4404501e20b3f1905a5eebd13734a65db27ae
workflow-type: tm+mt
source-wordcount: '714'
ht-degree: 0%

---

# Overzicht van start- en voltooiingsdagen in een sjabloon

U kunt projectmalplaatjes gebruiken om de meeste herhaalbare processen, informatie, en montages te vangen verbonden aan de projecten in uw organisatie. Hoewel projecten specifieke start- en voltooiingsdatums hebben, hebben sjablonen algemene start- en voltooiingsdagen als indicatie voor de plaats waar deze data op het project zullen vallen, op basis van de algemene tijdslijn van het project.

**Voorbeeld:** als de Datum van het Begin van een project 1 April is en u een taak wilt beginnen op 3 April (twee dagen na het begin van het project), zou de overeenkomstige taak op het malplaatje dat tot het project leidt op Dag 2 van het malplaatje moeten beginnen, waar de eerste dag van het malplaatje als Dag 0 wordt beschouwd.

## Begindag

Houd rekening met het volgende wanneer u werkt met sjablonen en sjabloontaken:

* Door gebrek, hebben de malplaatjes een Dag van het Begin van 0 en de malplaatjetaken en het malplaatje toont een Dag van het Begin van 0. De Begindag van de sjabloontaken kan veranderen, maar dit verandert de Begindag van de sjabloon niet.
* De begindag van een sjabloontaak geeft het aantal werkdagen weer dat Workfront toevoegt aan de geplande begindatum van de taak wanneer een project wordt gemaakt op basis van de sjabloon. U kunt bijvoorbeeld een sjabloon hebben met slechts één taak en de Begindag van de sjabloontaak is 4. De begindag van de sjabloon is nog steeds 0. Wanneer u een project van dit malplaatje creeert waar de Wijze van het Programma van het project de Datum van het Begin is, en de Geplande Datum van het Begin van het project 1 November, 2019 is, voegt de nieuw-gecreeerde taak 4 dagen aan deze datum toe en plaatst zijn Geplande Waarde van de Datum van het Begin aan 5 November 2019.

Hier volgen enkele acties die de Begindag van de sjabloontaken kunnen wijzigen:

* Werk de Duur van de taken van het voorgangersmalplaatje bij
* De taakbeperkingen bijwerken

  Wanneer het gebruiken van op datum-gebaseerde Beperkingen van de Taak, kunt u de Dag van het Begin van de malplaatjetaken manueel bijwerken. Sommige voorbeelden van op datum-gebaseerde Taakbeperkingen zijn Vaste Data, Begin niet vroeger dan, Begin niet later dan, moet beginnen op.

* Voorgangers voor sjabloontaken bijwerken

## Voltooiingsdag

De voltooiingsdag van de sjabloon is de dag waarop de laatste sjabloontaak is voltooid. Door gebrek, tonen alle malplaatjetaken en het malplaatje een Dag van de Voltooiing van 1, omdat Workfront veronderstelt dat om het even welke malplaatjetaak een Duur van 1 Dag heeft. De Voltooiingsdag van de malplaatjetaken kan veranderen en dit verandert ook de Dag van de Voltooiing van het malplaatje. De Voltooiingsdag van het malplaatje wordt de Geplande VoltooiingsDatum van het toekomstige project en de VoltooiingsDagen van de malplaatjetaken worden de Geplande AfsluitingsData van de toekomstige projecttaken.

Hier volgen enkele acties die de Voltooiingsdag van de sjabloontaken kunnen wijzigen:

* De duur van de sjabloontaken bijwerken
* De taakbeperkingen bijwerken

  Wanneer het gebruiken van op datum-gebaseerde Beperkingen van de Taak, kunt u de Dag van de Voltooiing van de malplaatjetaken manueel bijwerken. Sommige voorbeelden van op datum-gebaseerde taakbeperkingen zijn Vaste DATA, beëindigen niet vroeger dan, beëindigen niet later dan, moet beëindigen op.

* Voorgangers voor sjabloontaken bijwerken

## Werken met sjablonen die zijn gepland na voltooiing

U kunt een sjabloon plannen vanaf Voltooiingsdag. Voor meer informatie, zie [ projectmalplaatjes ](../../../manage-work/projects/create-and-manage-templates/edit-templates.md) uitgeven.

Denk aan het volgende wanneer u werkt met sjablonen die vanaf de Voltooiingsdatum zijn gepland:

* Als u de Begindag wijzigt, wordt de taakbeperking ingesteld op Aan.
* Als u de voltooiingsdag wijzigt, wordt de taakbeperking ingesteld op Op.
* Wanneer het malplaatje van de Dag van de Voltooiing gepland is, wordt de Dag van de Beperking van de Taak berekend vanaf de Dag van de Voltooiing.

  **Voorbeeld:** de duur van uw malplaatje is 285 dagen, en u hebt een malplaatjetaak met duur 60 dagen. Als u de Taakbeperking instelt op Moet beginnen op en Beperkingsdag op 120, hebt u een Begindag van 165 (285 - 120) en Voltooiingsdag van 225 (165 + 60). Dus als je de Begindag bewerkt, wordt deze geïnterpreteerd als Restrictiedag.
