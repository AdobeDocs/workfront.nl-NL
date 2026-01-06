---
product-area: projects
navigation-topic: manage-projects
title: Microsoft-projectvelden toewijzen aan Adobe Workfront-projecten
description: Projecten in Adobe Workfront en Microsoft Project zijn meestal compatibel. Dit artikel beschrijft hoe de gemeenschappelijkste projectgebieden van de twee toepassingen aan elkaar in kaart brengen.
author: Alina
feature: Work Management
exl-id: 381eb6ad-8084-406b-90f9-44460b58a04c
source-git-commit: dbc4404501e20b3f1905a5eebd13734a65db27ae
workflow-type: tm+mt
source-wordcount: '396'
ht-degree: 0%

---

# Microsoft-projectvelden toewijzen aan Adobe Workfront-projecten

Projecten in Adobe Workfront en Microsoft Project zijn meestal compatibel. Met de twee toepassingen kunt u het volgende doen:

* Projecten exporteren uit Microsoft Project en deze importeren in Workfront
* Exporteer projecten uit Workfront en importeer ze naar Microsoft Project.

Voor meer informatie over het invoeren van projecten van het Project van Microsoft in Workfront, zie [&#x200B; een project van het Project van Microsoft invoeren &#x200B;](../../../manage-work/projects/create-projects/import-project-from-ms-project.md).

Voor meer informatie over het uitvoeren van een project van Workfront om het in het Project van Microsoft in te voeren, zie [&#x200B; Uitvoer een project aan het Project van Microsoft &#x200B;](../../../manage-work/projects/manage-projects/export-project-to-ms-project.md).

Bij het uitvoeren van dergelijke invoer van gegevens, is het belangrijk om te begrijpen hoe de informatie van één toepassing aan andere vertaalt. Meestal zult u enkele handmatige wijzigingen in het project moeten aanbrengen nadat u het importeren hebt voltooid.

## Overzicht van veldtoewijzing

>[!NOTE]
>
>De geplande data komen niet altijd overeen tussen beide systemen. Verschillen tussen Workfront en Microsoft Project zijn te wijten aan schema en verschillen in systeemvoorkeuren. Deze datumverschillen kunnen ook resulteren in verschillen in inspanning, duur, en volledig percentage.

| **het Gebied van het Project van Microsoft** | **het Gebied van Workfront** |
|---|---|
| Projecttitel | Projectnaam |
| Begin- en einddatum | Geplande begin- en einddatum |
| Taaknaam | Taaknaam |
| Taakduur | Taak geplande duur |
| Taakwerk | Taak geplande uren |
| Taak % voltooid | Taak % voltooid (op basis van de duur van de taak) |
| Taakwerk % voltooid | Taak % voltooid (op basis van de geplande uren van de taak) |
| Gepland begin en einde | Geplande begin- en einddatum |
| Werkelijk starten en voltooien | Werkelijke begin- en einddatum |
| Bronnaam | Taaktoewijzing |
| Toewijzingseenheden | Percentage toewijzing toewijzing |
| Taaknotitie | Taakbeschrijving |
| Voorganger | Voorganger |

## Overzicht van gegevens die niet zijn opgenomen

Er zijn een aantal projectvelden die niet worden geïmporteerd in of geëxporteerd uit Workfront.

Deze velden omvatten onder meer, maar zijn niet beperkt tot:

* Documentbijlagen
* Aangepaste velden (op het project- of taakniveau)
* Workfront-notities
* Problemen
* Negatieve vertraging in taken met een eerdere relatie voor Start/Voltooien (taken worden zonder vertraging geïmporteerd)
* Toewijzingen
* Taakbeperkingen

  >[!NOTE]
  >
  >Omdat de Beperkingen niet tussen het Project van Microsoft en Workfront in kaart brengen, zorg ervoor dat er voorgangersverhoudingen tussen de taken zijn. Anders is het mogelijk dat de geplande begin- en einddatum van de taken in het geïmporteerde project niet nauwkeurig zijn.
