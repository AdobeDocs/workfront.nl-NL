---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: workfront-fusion-2-0
title: Verbindingsmetagegevens in Adobe Workfront Fusion
description: De Adobe Workfront Fusion-documentatie is verplaatst naar een nieuwe locatie. Dit artikel is vervangen, maar bevat een koppeling naar het nieuwe artikel dat deze functionaliteit behandelt.
author: Becky
feature: Workfront Fusion
exl-id: af260c63-3385-4d5c-abc2-d5c23175be40
source-git-commit: 2d6af8b4988bd9aab7381daa79dec79e41408c45
workflow-type: tm+mt
source-wordcount: '338'
ht-degree: 0%

---

# Verbindingsmetagegevens in Adobe Workfront Fusion

>[!IMPORTANT]
>
>De Adobe Workfront Fusion-documentatie is verplaatst naar een nieuwe locatie.
>
>De informatie in dit artikel is nu te vinden in het artikel:
>
>* [ meta-gegevens van de Verbinding ](https://experienceleague.adobe.com/docs/workfront-fusion/using/references/connections/connection-metadata.html)
>
>Werk eventuele bladwijzers bij.
>
>Dit artikel wordt niet meer bijgewerkt en wordt in de nabije toekomst verwijderd.

>[!NOTE]
>
>[!DNL Adobe Workfront Fusion] vereist een [!DNL Adobe Workfront Fusion] licentie naast een [!DNL Adobe Workfront] licentie.

Niet alle verbindingen zijn het zelfde. Het begrip van de verschillen tussen verbindingen is zeer belangrijk voor het kennen van hun bedrijfscontext. Fusion gebruikt metagegevens om belangrijke kenmerken van een verbinding te identificeren.

Verbindingsmetagegevens kunnen worden ingesteld wanneer u een nieuwe verbinding maakt. Deze kenmerken bevinden zich in hetzelfde dialoogvenster dat wordt gebruikt voor het instellen van een verbinding:

![ meta-gegevens van de Verbinding ](assets/connection-metadata-setup.png)

Fusiegebruikers kunnen verbindingen weergeven en bewerken vanuit het gebied Verbindingen.

![ meta-gegevens van de Verbinding in het gebied van Verbindingen ](assets/connections-area-metadata.png)

## Omgevingstype

Fusieverbindingen kunnen zowel door productie- als niet-productiesystemen worden gebruikt. Kennis van het verschil is erg belangrijk voor de bescherming van productieomgevingen. Het omgevingstype wordt, net als andere verbindingsmetagegevens, alleen ter informatie gebruikt. Gebruikers zijn nog steeds verantwoordelijk voor het nauwkeurig instellen van dit kenmerk.

## Type verificatie

De verbindingen van de fusie kunnen voor zowel de dienstrekeningen als persoonlijke rekeningen worden gebruikt. De rekeningen van de dienst worden gebruikt voor authentificatie wanneer een scenario als Fusie automatiseert. Persoonlijke accounts zijn op een specifieke persoon gebaseerde verificatie. Welk authentificatietype wordt gebruikt hangt van de vereisten van het scenario af. Persoonlijke accounts moeten worden gebruikt voor geautomatiseerde gebruikersacties. Bijvoorbeeld, als een scenario van de Fusie goedkeuring door een specifieke persoon automatiseert, dan zou het authentificatietype voor die persoon moeten zijn. Anders fungeert Fusion als Fusion en moet het type &quot;Servicerekening&quot; zijn.

Merk op dat het type, net als andere verbindingsmetagegevens, alleen ter informatie wordt gebruikt. Gebruikers zijn nog steeds verantwoordelijk voor het handmatig instellen van dit kenmerk.

Voor meer informatie over authentificatietypen, te zien gelieve [ Authentificatie ](https://developer.adobe.com/developer-console/docs/guides/authentication/) in de gids van de Authentificatie van de Adobe.
