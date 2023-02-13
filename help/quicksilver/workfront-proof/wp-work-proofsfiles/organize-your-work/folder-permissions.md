---
content-type: reference
product-previous: workfront-proof
product-area: documents
navigation-topic: organize-your-work-workfront-proof
title: Mapmachtigingen begrijpen in [!DNL Workfront Proof]
description: Als iemand gemachtigd is om een item in een map te zien, kan hij of zij ook de map zelf zien. Ze kunnen echter alleen de items in de map zien die expliciet met hen zijn gedeeld.
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: 96162fe8-eef9-40f4-bc94-02911b970f02
source-git-commit: 41ab1312d2ccb8b8271bc851a35e31e9ff18c16b
workflow-type: tm+mt
source-wordcount: '561'
ht-degree: 0%

---

# Mapmachtigingen begrijpen in [!DNL Workfront Proof]

>[!IMPORTANT]
>
>Dit artikel verwijst naar functionaliteit in het standalone product [!DNL Workfront Proof]. Voor informatie over proefdrukken binnen [!DNL Adobe Workfront], zie [Proofing](../../../review-and-approve-work/proofing/proofing.md).

Als iemand gemachtigd is om een item in een map te zien, kan hij of zij ook de map zelf zien. Ze kunnen echter alleen de items in de map zien die expliciet met hen zijn gedeeld.

## Openbare mappen

Als een map openbaar is, kunnen gebruikers in de account (met uitzondering van gebruikers van Waarnemers en Licht) de mapnaam zien in de linkerzijbalk.

Uw machtigingsprofiel heeft ook invloed op de rechten die u hebt op openbare mappen:

| **Profiel/Handeling** | **Alle items in map weergeven** | **Zie items die expliciet met hen worden gedeeld** | **Items toevoegen** | **Items verwijderen** | **Submappen toevoegen** | **Submappen verwijderen** | **Mapdetails bewerken** |
|---|---|---|---|---|---|---|---|
| **Maker** | Ja | Ja | Ja | Ja | Ja | Ja | Ja |
| **Factureringsbeheerder** | Ja | Ja | Ja | Ja | Ja | Ja | Ja |
| **Beheerder** | Ja | Ja | Ja | Ja | Ja | Ja | Ja |
| **Supervisor** | Ja | Ja | Ja | Ja | Ja | Ja | Ja |
| **Manager** | Nee | Ja | Ja | Nee | Ja | Nee | Ja |
| **Waarnemer** | Nee | Ja | Nee | Nee | Nee | Nee | Nee |

{style=&quot;table-layout:auto&quot;}

Als een manager eigenaar is van de openbare map, kan hij of zij de hoofdmap en alle submappen verwijderen.

Zie voor meer informatie [Profielen met proefmachtigingen in [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/account-settings/proof-perm-profiles-in-wp.md).

## Persoonlijke mappen

Als een omslag privé is, zullen andere gebruikers in de zelfde rekening niet de naam van de omslag in linkerzijbalk kunnen zien tenzij de omslag of de punten in de omslag uitdrukkelijk met hen zijn gedeeld of zij een profiel van Supervisor, beheerder, of de Beheerder van de Facturering hebben:

| **Profiel/Handeling** | **Alle items in map weergeven** | **Zie items die expliciet met hen worden gedeeld** | **Items toevoegen** | **Items verwijderen** | **Submappen toevoegen** | **Submappen verwijderen** | **Mapdetails bewerken** |
|---|---|---|---|---|---|---|---|
| **Maker** | Ja | Ja | Ja | Ja | Ja | Ja | Ja |
| **Factureringsbeheerder** | Ja | Ja | Ja | Ja | Ja | Ja | Ja |
| **Beheerder** | Ja | Ja | Ja | Ja | Ja | Ja | Ja |
| **Supervisor** | Ja | Ja | Ja | Ja | Ja | Ja | Ja |
| **Manager** | Nee | Ja | Nee | Nee | Nee | Nee | Nee |
| **Waarnemer** | Nee | Ja | Nee | Nee | Nee | Nee | Nee |

{style=&quot;table-layout:auto&quot;}

Als u bijvoorbeeld wilt dat uw projectmanager en hun teams alleen specifieke mappen zien, kan de projectbeheerder een privémap instellen en de map vervolgens delen met specifieke gebruikers.

Wanneer u een persoonlijke map deelt, kunt u bepalen of u managers in staat wilt stellen om mapitems te maken, te bewerken en te verwijderen.

U kunt dit voor elke persoon afzonderlijk instellen op de pagina Nieuwe map en het wijzigen in het dialoogvenster [!UICONTROL Shared with] van de pagina met mapdetails. Zie voor meer informatie [Mappen maken in [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/organize-your-work/create-folders.md) en [Mappen en de inhoud ervan beheren in [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/organize-your-work/manage-folders-and-contents.md).

Als een privémap wordt gedeeld met een server of waarnemer, hebben deze gebruikers alleen-lezen toegang tot alle items in de map. Zie voor meer informatie [Profielen met proefmachtigingen in [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/account-settings/proof-perm-profiles-in-wp.md) en [Mappen delen in [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/organize-your-work/share-folders.md).

>[!NOTE]
>
>* Als een bovenliggende map een privémap is, zijn alle submappen ook privé. U kunt geen openbare submap onder een persoonlijke bovenliggende map hebben. U kunt echter wel een persoonlijke submap hebben onder een openbare bovenliggende map.
>* De maker en eigenaar van de map hebben altijd toegang tot de map en kunnen deze niet verwijderen.
>* Alleen de maker en eigenaar van de persoonlijke map kunnen de map verwijderen.


