---
product-area: documents;workfront-integrations
navigation-topic: adobe-workfront-for-experince-manager-asset-essentials
title: Inhoud en mappen koppelen met Content Advisor van Experience Manager Assets
description: Met Content Advisor kunt u inhoud of mappen vanuit Experience Manager Assets koppelen aan elk Adobe Workfront-object dat documenten ondersteunt. Content Advisor brengt intelligente, contextbewuste detectie rechtstreeks naar Workfront, zodat u snel relevante, goedgekeurde inhoud kunt vinden.
author: Courtney
feature: Digital Content and Documents, Workfront Integrations and Apps
exl-id: dbd19985-88b1-48ca-9cba-b7933ff2c191
source-git-commit: ab868314aef0924906ca69e82a10ece130484ba7
workflow-type: tm+mt
source-wordcount: '1226'
ht-degree: 0%

---

# Inhoud en mappen koppelen met Experience Manager Assets Content Advisor

Content Advisor brengt intelligente, contextbewuste detectie rechtstreeks naar Workfront, zodat u snel relevante, goedgekeurde inhoud kunt vinden op basis van context. Met functies zoals slimme suggesties, Dynamische media-uitvoeringen en gedetailleerde metagegevens over elementen kunt u inhoud efficiënt evalueren en opnieuw gebruiken zonder Workfront te verlaten. Zo kunt u de inhoud sneller maken en de consistentie van uw merk behouden.

Met Content Advisor kunt u inhoud en mappen van Experience Manager Assets naar Workfront koppelen. Als de inhoud eenmaal is gekoppeld, kunt u de inhoud in Workfront weergeven en beheren. Alle wijzigingen die in de inhoud in Experience Manager Assets zijn aangebracht, worden weerspiegeld in Workfront.

>[!IMPORTANT]
>
>Als uw organisatie weigert de GenAI Rider-overeenkomst te ondertekenen, kunt u nog steeds Content Advisor gebruiken om middelen en mappen in Experience Manager Assets te kiezen, maar hebt u geen toegang tot door AI aangedreven functies zoals AI Search, slimme suggesties of analyseringscampagnematerialen.

## Toegangsvereisten

+++ Breid uit om de toegangseisen voor de functionaliteit in dit artikel weer te geven.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-pakket</td> 
   <td> <p> Alle</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-licenties</td> 
   <td> 
   <p>Medewerker of hoger</p> 
   <p>Aanvraag of hoger</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Aanvullende producten</td> 
   <td>U moet Experience Manager as a Cloud Service of Assets Essentials hebben en u moet als gebruiker aan het product worden toegevoegd in de Admin Console.</td> 
  </tr> 
   <tr> 
    <td role="rowheader">Experience Manager-machtigingen</td> 
    <td>U moet schrijftoegang tot de map hebben.</td> 
   </tr>
  <tr> 
   <td role="rowheader">Configuraties op toegangsniveau</td> 
   <td> <p>Toegang tot documenten bewerken</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objectmachtigingen</td> 
   <td> <p>Toegang weergeven of hoger</p> </td> 
  </tr> 
 </tbody> 
</table>

Voor meer detail over de informatie in deze lijst, zie [&#x200B; vereisten van de Toegang in de documentatie van Workfront &#x200B;](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Vereisten

Voordat u begint:

* Uw Workfront-beheerder moet een Experience Manager-integratie configureren. Voor meer informatie, zie [&#x200B; de integratie van Experience Manager Assets as a Cloud Service &#x200B;](/help/quicksilver/administration-and-setup/configure-integrations/configure-aacs-integration.md) vormen.

* Als u de functie Slimme suggesties of Campagne Brief wilt gebruiken, moet u een GenAI Rider ondertekenen. Voor meer informatie, zie [&#x200B; Adviseur van de Inhoud van het Gebruik om tot inhoud van AEM in de toepassingen van Adobe &#x200B;](https://experienceleague.adobe.com/en/docs/experience-manager-cloud-service/content/assets/manage/content-advisor-adobe-applications#content-advisor-ai-search) toegang te hebben.



## Inhoud van Experience Manager Assets koppelen met Content Advisor

U kunt Content Advisor nu gebruiken om inhoud van Experience Manager Assets rechtstreeks in Workfront te koppelen. Content Advisor is niet beschikbaar voor Elementen.

Inhoud koppelen:

1. Ga naar het **gebied van Documenten** in Workfront waar u het document wilt toevoegen.
1. Selecteer **toevoegen Nieuw**, dan selecteren de integratie van Experience Manager uw beheerderopstelling.

   >[!NOTE]
   >
   >De Workfront-beheerder kan elke naam voor deze integratie kiezen, dus Experience Manager Assets wordt niet specifiek genoemd.

1. Met Content Advisor kunt u:


   <table style="table-layout:auto">
   <tbody>
      <tr>
         <td><strong> Onderzoek naar activa die AI Onderzoek gebruiken.</strong> Gebruik een door AI aangedreven zoekopdracht die betekenis en intentie achter query's begrijpt en die meerdere talen, typos en synoniemen ondersteunt.</td>
         <td>Voor meer informatie, zie <a href="https://experienceleague.adobe.com/en/docs/experience-manager-cloud-service/content/assets/manage/content-advisor-adobe-applications#content-advisor-ai-search"> AI Onderzoek naar slimmere activaontdekking </a>.</td>
      </tr>
      <tr>
         <td><strong> de slimme suggesties van de Mening die op context en intent worden gebaseerd.</strong> Ontdek elementen die u kunt uitlijnen op uw inhoud en gebruik daarbij contextgevoelige aanbevelingen van de Adobe-hosttoepassing.</td>
         <td>Voor meer informatie, zie <a href="https://experienceleague.adobe.com/en/docs/experience-manager-cloud-service/content/assets/manage/content-advisor-adobe-applications#smart-suggestions-content-advisor"> Slimme suggesties die op context en intent </a> worden gebaseerd.</td>
      </tr>
      <tr>
         <td><strong> upload een campagnemorandum om relevante activa te ontdekken.</strong> Upload een PDF-, DOCX- of TXT-campagnecorrecept, zodat Content Advisor dit kan analyseren en relevante elementen kan aanbevelen.</td>
         <td>Voor meer informatie, zie {de briefjes van 0} Campagne om relevante activa <a href="https://experienceleague.adobe.com/en/docs/experience-manager-cloud-service/content/assets/manage/content-advisor-adobe-applications#campaign-briefs-content-advisor"> te ontdekken.</a></td>
      </tr>
      <tr>
         <td><strong> Mening en selecteer Dynamische de activavertoningen van Media.</strong> Blader door voor kanalen geoptimaliseerde uitvoeringen, waaronder voorinstellingen voor afbeeldingen, slimme uitsnijdingen en opmaaktypen, en pas modifiers voor dynamische media toe om in real-time voorvertoningen van aanpassingen weer te geven.</td>
         <td>Voor meer informatie, zie <a href="https://experienceleague.adobe.com/en/docs/experience-manager-cloud-service/content/assets/manage/content-advisor-adobe-applications#dynamic-media-renditions-content-advisor"> Dynamische de activavertoningen van Media beschikbaar voor gebruik </a>.</td>
      </tr>
      <tr>
         <td><strong> past Dynamische bepalingen van Media op vertoningen toe.</strong> Voeg opties toe om elementuitvoeringen in real-time te transformeren en bekijk een voorvertoning van de resultaten voordat u een uitvoering voor de hosttoepassing selecteert.</td>
         <td>Voor meer informatie, zie <a href="https://experienceleague.adobe.com/en/docs/experience-manager-cloud-service/content/assets/manage/content-advisor-adobe-applications#dynamic-media-renditions-content-advisor"> Dynamische de activavertoningen van Media beschikbaar voor gebruik </a>.</td>
      </tr>
      <tr>
         <td><strong> ontdekt en doorblader de Fragments van de Inhoud.</strong> Zoeken via Content Fragments, live miniatuurvoorvertoningen bekijken, de status controleren (Concept, Gewijzigd of Gepubliceerd) en gedetailleerde eigenschappen, verwijzingen en variaties inspecteren.</td>
         <td>Voor meer informatie, zie <a href="https://experienceleague.adobe.com/en/docs/experience-manager-cloud-service/content/assets/manage/content-advisor-adobe-applications#content-fragments-discovery-content-advisor"> Ontdekking van de Fragmenten van de Inhoud </a>.</td>
      </tr>
      <tr>
         <td><strong> de activameta-gegevens van de Toegang.</strong> U kunt de eigenschappen van elementen, zoals titel, beschrijving, indeling, grootte en andere tabbladen met metagegevens (Product, Campagne, Tags), op dezelfde manier bekijken als de weergave Assets.</td>
         <td>Voor meer informatie, zie <a href="https://experienceleague.adobe.com/en/docs/experience-manager-cloud-service/content/assets/manage/content-advisor-adobe-applications#asset-metadata-content-advisor"> de activameta-gegevens van de Toegang verenigbaar met de mening van Assets </a>.</td>
      </tr>
      <tr>
         <td><strong> de activa van de Filter gebruikend vooraf bepaalde filters.</strong> Verfijn de resultaten van elementen met filters zoals Bestandstype, Bestandsindeling, Status van element, Bestandsgrootte, Afbeeldingsbreedte, Afbeeldingshoogte, Gewijzigde datum en Gemaakt op.</td>
         <td>Voor meer informatie, zie <a href="https://experienceleague.adobe.com/en/docs/experience-manager-cloud-service/content/assets/manage/content-advisor-adobe-applications#filters-content-advisor"> de filters van de Toegang verenigbaar met de mening van Assets </a>.</td>
      </tr>
      <tr>
         <td><strong> sparen en hergebruik onderzoeken.</strong> Maak opgeslagen zoekopdrachten door een zoekterm en filteropties op te geven en deze vervolgens te hergebruiken in Experience Manager Assets en andere Adobe-toepassingen.</td>
         <td>Voor meer informatie, zie <a href="https://experienceleague.adobe.com/en/docs/experience-manager-cloud-service/content/assets/manage/content-advisor-adobe-applications#saved-searches-content-advisor"> Toegang en hergebruik recente en bewaarde onderzoeken </a>.</td>
      </tr>
      <tr>
         <td><strong> Onderzoek naar activa over en binnen inzamelingen.</strong> Zoeken naar elementen of verzamelingen in alle verzamelingen, of de zoekopdracht beperken tot een bepaalde verzameling.</td>
         <td>Voor meer informatie, zie <a href="https://experienceleague.adobe.com/en/docs/experience-manager-cloud-service/content/assets/manage/content-advisor-adobe-applications#search-collections-content-advisor"> Onderzoek naar activa over en binnen inzamelingen </a>.</td>
      </tr>
   </tbody>
   </table>


### Een nieuwe versie van Experience Manager Assets koppelen met Content Advisor

U kunt nieuwe inhoud ophalen uit Experience Manager Assets of Elementen en deze toevoegen aan een bestaand element als een nieuwe versie. Als het document al is gekoppeld en een nieuwe versie wordt toegevoegd in Experience Manager Assets of Assets Essentials, wordt de nieuwe versie automatisch weergegeven in Workfront.

Een nieuwe versie koppelen:

1. Ga naar het **gebied van Documenten** in Workfront waar u het document wilt toevoegen.
1. Selecteer het element dat u wilt vervangen door een nieuwe versie. U kunt geen nieuwe versie van een middel in een verbonden omslag tot stand brengen.
1. Selecteer **Nieuwe** toevoegen > **Versie**, dan de integratie van Experience Manager uw beheerderopstelling selecteren.

   >[!NOTE]
   >
   >De Workfront-beheerder kan elke naam voor deze integratie kiezen, dus Experience Manager Assets wordt niet specifiek genoemd.

1. Selecteer de inhoud die u wilt koppelen:

   * Selecteer het tabblad Assets om te bladeren in elementen, mappen of verzamelingen in Experience Manager Assets of Elementen.

     ![&#x200B; adviseur van de Inhoud &#x200B;](assets/content-advisor-full.png)

   * Inhoudsfragmenten ondersteunen geen versies. Als u een inhoudsfragment selecteert, vervangt de nieuwe versie het bestaande inhoudsfragment in plaats van een nieuwe versie te maken.

1. Klik **Uitgezocht**.

## Een map van Experience Manager Assets koppelen met Content Advisor

Rechten om afzonderlijke elementen in een map weer te geven, zijn afhankelijk van Experience Manager Assets-machtigingen.

Een map koppelen:

1. Ga naar het **gebied van Documenten** in Workfront waar u de omslag wilt.
1. Selecteer **toevoegen Nieuw**, dan selecteren de integratie van Experience Manager uw beheerderopstelling.

   >[!NOTE]
   >
   >De Workfront-beheerder kan elke naam voor deze integratie kiezen, dus Experience Manager Assets wordt niet specifiek genoemd.

1. Klik **Assets** > **Dossiers &amp; Omslagen**.

1. Klik het **pictogram van de Filter**, dan in de **sectie van het Type van Activa**, kies **Omslagen**.

1. Selecteer de map die u wilt koppelen.

1. Klik **Uitgezocht**.

## Overwegingen

* De functionaliteit Content Advisor is niet beschikbaar voor objecten die gebruikmaken van Adobe Enterprise Storage. Als uw organisatie Adobe Enterprise Storage gebruikt, kunt u nog steeds middelen en mappen van Experience Manager Assets of Assets Essentials koppelen, maar hebt u geen toegang tot functies voor Content Advisor, zoals AI-zoekopdrachten, slimme suggesties of Dynamische media-uitvoeringen. Voor meer informatie, zie [&#x200B; Gebruik Adobe Experience Manager met de integratie Frame.io &#x200B;](/help/quicksilver/review-and-approve-work/native-integrations/frame-io/use-aem-with-frame.md).

* De functionaliteit van de Adviseur van de inhoud is niet beschikbaar voor de Hoofdzaak van Activa. Om activa en omslagen van de Hoofdzaak van Activa te verbinden, zie [&#x200B; activa en omslagen van de Verbinding van de Hoofdzaak van Experience Manager Assets &#x200B;](/help/quicksilver/documents/adobe-workfront-for-experience-manager-assets-essentials/link-to-aem-essentials.md).

* Metagegevensvelden worden eerst toegewezen wanneer u een element verzendt van Workfront naar Experience Manager Assets. Als uw Workfront-beheerder heeft ingesteld dat objectmetagegevenssynchronisatie is ingeschakeld, blijven de velden up-to-date als deze in een van beide toepassingen zijn gewijzigd.
