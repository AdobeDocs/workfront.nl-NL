---
product-area: documents;workfront-integrations
navigation-topic: adobe-workfront-for-experince-manager-asset-essentials
title: Een document verzenden naar Experience Manager Assets of Elementen
description: U kunt documenten van Workfront naar Experience Manager Assets of Assets Essentials verzenden. Documenten die van Workfront naar Assets Essentials zijn geüpload en verzonden, tellen nog steeds mee voor de totale opslag van documenten. Assets gekoppeld van Assets Essentials telt niet mee voor algemene opslag.
author: Courtney
feature: Digital Content and Documents, Workfront Integrations and Apps
exl-id: 7942e77b-9466-4dff-9737-97b17647ac48
source-git-commit: 85a2f154b3b561cdf53c68d50e66b8945f9f9823
workflow-type: tm+mt
source-wordcount: '919'
ht-degree: 0%

---

# Een document verzenden naar Experience Manager Assets of Elementen

U kunt documenten van Workfront naar Experience Manager Assets of Assets Essentials verzenden. Documenten die van Workfront naar Assets Essentials zijn geüpload en verzonden, tellen nog steeds mee voor de totale opslag van documenten. Assets gekoppeld van Assets Essentials telt niet mee voor algemene opslag.

Assets die naar Experience Manager door deze integratie wordt verzonden heeft een groottegrens van **5 GB**.

In het milieu van de Voorproef, heeft Assets die naar Experience Manager door deze integratie wordt verzonden een groottegrens van **30 GB**.

Metagegevensvelden worden eerst toegewezen wanneer u een element verzendt van Workfront naar Experience Manager Assets of Elementen. Eventuele metagegevens die zijn geconfigureerd om toe te wijzen voor bovenliggende objecten, worden ook verzonden. Voor meer informatie bij het vormen meta-gegevensafbeelding, zie [ de integratie van Experience Manager Assets as a Cloud Service ](/help/quicksilver/administration-and-setup/configure-integrations/configure-aacs-integration.md) vormen of [ vormen de integratie van de Hoofdzaak van Experience Manager Assets ](/help/quicksilver/documents/adobe-workfront-for-experience-manager-assets-essentials/setup-asset-essentials.md).

>[!INFO]
>
>**Voorbeeld** wanneer u eerst een activa verzendt in bijlage aan een taak, de kaarten van taakmeta-gegevens aan Experience Manager Assets of de Hoofdzaak van Activa evenals om het even welke in kaart gebrachte meta-gegevens van oudervoorwerpen zoals een project, een portefeuille, en een programma.

## Toegangsvereisten

+++ Breid uit om de toegangseisen voor de functionaliteit in dit artikel weer te geven.

U moet de volgende toegang hebben om de stappen in dit artikel te voltooien:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><a href="https://www.workfront.com/plans" target="_blank"> plan van Adobe Workfront </a>*</td> 
   <td> <p> Alle</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><a href="../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref"> overzicht van de Vergunningen van de Vererfenis </a>*</td> 
   <td> <p>Aanvraag of hoger</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Product</td> 
   <td>U moet Experience Manager as a Cloud Service of Assets Essentials hebben en u moet als gebruiker aan het product worden toegevoegd in de Admin Console.
</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraties op toegangsniveau*</td> 
   <td> <p>Toegang tot documenten bewerken</p> <p>Opmerking: als u nog steeds geen toegang hebt, vraag dan aan de Workfront-beheerder of deze aanvullende beperkingen op uw toegangsniveau heeft ingesteld. Voor informatie over hoe een beheerder van Workfront uw toegangsniveau kan wijzigen, zie <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref"> tot douanetoegangsniveaus </a> leiden of wijzigen.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objectmachtigingen</td> 
   <td> <p>Toegang of hoger weergeven op documenten</p> <p>Voor informatie bij het vragen van om extra toegang, zie <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref"> de toegang van het Verzoek tot voorwerpen </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42; om te weten te komen welk plan, vergunningstype, of toegang u hebt, contacteer uw beheerder van Workfront.

+++

## Vereisten

Voordat u begint,

* Uw Workfront-beheerder moet een Experience Manager-integratie configureren. Voor meer informatie, zie [ de integratie van Experience Manager Assets as a Cloud Service ](/help/quicksilver/administration-and-setup/configure-integrations/configure-aacs-integration.md) vormen of [ vormen de integratie van de Hoofdzaak van Experience Manager Assets ](/help/quicksilver/documents/adobe-workfront-for-experience-manager-assets-essentials/setup-asset-essentials.md).


## Een document verzenden vanuit Workfront

Wanneer een gebruiker een document van Workfront naar Experience Manager Assets of Assets Essentials verzendt, worden de toegewezen metagegevens over het document overgedragen. Nadat het document is verzonden, worden wijzigingen die zijn aangebracht in de metagegevens van het document in Workfront, niet doorgevoerd in Assets of Assets Essentials. Als een toegewezen veld in Workfront wordt gewijzigd, moet u een nieuwe versie van het document met de bijgewerkte metagegevens verzenden naar Assets of Assets Essentials. Aan opstelling of geef meta-gegevens uit, zie [ de integratie van Experience Manager Assets as a Cloud Service ](/help/quicksilver/administration-and-setup/configure-integrations/configure-aacs-integration.md) of [ vormen de integratie van de Hoofdzaak van Experience Manager Assets ](../../documents/adobe-workfront-for-experience-manager-assets-essentials/setup-asset-essentials.md).

Een document verzenden:

1. Ga naar het **gebied van Documenten** in Workfront, en selecteer het document u wilt verzenden.
1. Klik **verzenden naar**, dan kies de integratie van Experience Manager uw beheerderopstelling.

   >[!NOTE]
   >
   >De Workfront-beheerder kan een willekeurige naam voor deze integratie kiezen, dus Assets of Assets Essentials wordt niet specifiek vermeld.

   ![ verzendt naar ](assets/copy-of-send-to-in-toolbar-350x149.png)

1. Kies waar u de activa wilt gaan, dan klik **Uitgezochte Omslag**.
1. Wanneer u uw gewenste bestemming vindt, klik **sparen**.

## Nieuwe versie verzenden

U kunt een nieuwe versie toevoegen aan een document dat u eerder naar Workfront hebt geüpload. Voor meer informatie, zie [ een nieuwe versie van een document ](../../documents/managing-documents/upload-new-document-version.md) uploaden. Nadat de meest recente versie is geüpload, kunt u deze naar Elementen verzenden. Als een toegewezen veld in Workfront is gewijzigd, werkt de nieuwe versie de metagegevens in Elementen bij wanneer deze worden verzonden.

>[!IMPORTANT]
>
>Voordat u een nieuwe versie naar Workfront uploadt, raden we u aan de naam van het bestand te wijzigen. Als u een nieuwe versie uploadt met precies dezelfde bestandsnaam als een vorige versie, kan alleen de meest recente versie worden gedownload van Workfront. Alle versies kunnen ongeacht de bestandsnaam worden gedownload van Experience Manager Assets of Assets Essentials.

De meest recente versie verzenden:

1. Ga naar het **gebied van Documenten** in Workfront, en bepaal de plaats van het document.
1. Selecteer **verzenden naar**, dan kies de integratie van Experience Manager uw beheerderopstelling.

   >[!NOTE]
   >
   >De Workfront-beheerder kan een willekeurige naam voor deze integratie kiezen, dus Assets of Assets Essentials wordt niet specifiek genoemd.

   ![ verzendt naar ](assets/copy-of-send-to-in-toolbar-350x149.png)

1. Klik **sparen**. De nieuwe versie slaat op dezelfde locatie op als de vorige versie.

## Een document naar een gekoppelde map in Experience Manager Assets verplaatsen

>[!NOTE]
>
>Deze functionaliteit is alleen beschikbaar voor Experience Manager Assets as a Cloud Service. Deze is niet beschikbaar voor Experience Manager Assets Essentials.

U kunt een document naar een gekoppelde map in Experience Manager Assets verplaatsen als zowel het document als de gekoppelde map zich in dezelfde documentlijst bevinden (zoals het documentgebied van een project).

1. Zoek het document dat u wilt verplaatsen.
1. Sleep het document naar de gekoppelde Experience Manager Assets-map waarnaar u het wilt verplaatsen.

De documentopties zijn niet beschikbaar wanneer het document wordt verplaatst. Nadat het document naar Experience Manager Assets is verplaatst, is het niet meer zichtbaar in de documentlijst in Workfront.

>[!NOTE]
>
> Handelingen of bewerkingen die u tijdens het verplaatsen in het document aanbrengt, worden niet in het document in Experience Manager Assets weergegeven en gaan daarom verloren.

