---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: connector
navigation-topic: apps-and-their-modules
title: Microsoft Dynamics 365 Financierings- en operationele modules
description: In een  [!DNL Adobe Workfront Fusion]  scenario, kunt u werkschema's automatiseren die de Financiën en Verrichtingen van Microsoft Dynamics 365 gebruiken, evenals het met veelvoudige derdetoepassingen en de diensten verbinden.
author: Becky
feature: Workfront Fusion
source-git-commit: 130437dd44db5db2a94914fb0e42fd35a7c14291
workflow-type: tm+mt
source-wordcount: '917'
ht-degree: 0%

---

# [!DNL Microsoft Dynamics 365 Finance and Operations modules]

In een [!DNL Adobe Workfront Fusion] -scenario kunt u workflows automatiseren die [!DNL Microsoft Dynamics 365] gebruiken en deze koppelen aan meerdere toepassingen en services van derden.

>[!NOTE]
>
>De [!DNL Microsoft Dynamics 365 Finance and Operations] -connector biedt geen ondersteuning voor [!DNL Dynamics 365] .
>
>Zie [[!DNL Microsoft Dynamics 365 modules]](/help/quicksilver/workfront-fusion/apps-and-their-modules/microsoft-dynamics-365-modules.md) voor Microsoft Dynamics 365-modules.

Als u instructies bij het creëren van een scenario nodig hebt, zie [ een scenario in  [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/create-a-scenario.md) creëren.

Voor informatie over modules, zie [ Modules in  [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/modules.md).

## Verbinding maken

Een verbinding maken voor uw Microsoft Dynamics 365-modules Financiën en Operations:

1. In om het even welke Microsoft Dynamics 365 de module van Financiën en van Verrichtingen, klik **[!UICONTROL Add]** naast het vakje van de Verbinding.

1. Vul de volgende velden in:

   <table style="table-layout:auto"> 
      <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column1">
      </col>
      <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column2">
      </col>
      <tbody>
        <tr>
        <td role="rowheader">[!UICONTROL Connection type]</td>
        <td>
          <p>Selecteer of u een standaardverbinding van de Financiën en van Verrichtingen van de Dynamiek, of een verbinding creeert gebruikend een vergunningscode.</p>
        </td>
        </tr>
        <tr>
        <td role="rowheader">[!UICONTROL Connection name]</td>
        <td>
          <p>Voer een naam in voor deze verbinding.</p>
        </td>
        </tr>
        <tr>
        <td role="rowheader">[!UICONTROL Client ID]</td>
        <td>Ga uw Dynamische Financiën en Verrichtingen in [!UICONTROL Client ID].</td>
        </tr>
        <tr>
        <td role="rowheader">[!UICONTROL Client Secret]</td>
        <td>Ga uw Dynamische Financiën en Verrichtingen in [!UICONTROL Client Secret]. </td>
        </tr>
        <tr>
        <td role="rowheader">[!UICONTROL Tenant ID]</td>
        <td>Ga uw Identiteitskaart van de Financiën van de Dynamica en van de Aannemer van Verrichtingen in.</td>
        </tr>
        <tr>
        <td role="rowheader">Bron</td>
        <td>Ga URL van uw Rekening van de Financiën en van Verrichtingen van de Dynamica (zonder https:// in)</td>
        </tr>
      </tbody>
    </table>

1. Klik op **[!UICONTROL Continue]** om de verbinding op te slaan en terug te keren naar de module.



## Microsoft Dynamics 365 Financierings- en operationele modules en hun gebieden

>[!IMPORTANT]
>
>De gegevensentiteiten die beschikbaar zijn via de F&amp;O API van Dynamics 365 kunnen per instantie variëren. Als u niet zeker weet welke entiteiten beschikbaar zijn via de API, is het nuttig om door de entiteiten in uw instantie te kijken gebruikend het &quot;gegevens&quot;eindpunt. Het &quot;gegevens&quot;eindpunt in Dynamiek 365 Financiën en Verrichtingen is de wortel URL voor de toegang tot van de diensten OData. Dit eindpunt staat u toe om met diverse gegevensentiteiten in wisselwerking te staan die door het systeem worden blootgesteld gebruikend standaard protocollen OData.
>
>U kunt deze entiteiten ophalen met de aangepaste API-aanroepmodule.
>
><!--For more information -->



### Entiteitsitem maken

Deze actiemodule leidt tot een nieuw entiteitspost in Microsoft Dynamics 365 Financiën en Verrichtingen.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
    <td>[!UICONTROL Connection]</td>
    <td> <p>Voor instructies over het verbinden van Microsoft Dynamics 365 Financiën en Verrichtingen met [!DNL Workfront Fusion], zie <a href="#create-a-connection" class="MCXref xref"> een verbinding </a> in dit artikel creëren.</p> </td> 
  </tr> 
  <tr> 
    <td>[!UICONTROL Entity]</td>
     <td>Ga of kaart het de entiteitstype van de Financiën en van Verrichtingen van de Dynamiek in dat u wilt creëren.</td> 
  </tr> 
  <tr> 
    <td>[!UICONTROL Body]</td>
     <td> <p>Ga of kaart een lichaam JSON in dat de gegevens bevat die u in het nieuwe entiteitpunt wilt omvatten.</p> </td> 
  </tr> 
 </tbody> 
</table>



### Entiteitsitem verwijderen

Deze actiemodule schrapt een entiteitpunt van de Financiën en Verrichtingen van de Dynamiek. Het item wordt aangegeven door de velden Primaire sleutel.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
    <td>[!UICONTROL Connection]</td>
    <td> <p>Voor instructies over het verbinden van Microsoft Dynamics 365 Financiën en Verrichtingen met [!DNL Workfront Fusion], zie <a href="#create-a-connection" class="MCXref xref"> een verbinding </a> in dit artikel creëren.</p> </td> 
  </tr> 
  <tr> 
    <td>[!UICONTROL Entity]</td>
     <td>Ga of kaart het de entiteitstype van de Financiën en van Verrichtingen van de Dynamiek in dat u wilt schrappen.</td> 
  </tr> 
  <tr> 
    <td>[!UICONTROL Primary key fields]</td>
     <td> In de velden Primaire sleutel wordt het item geïdentificeerd. Voor elk primair zeer belangrijk gebied dat u wilt verstrekken, klik <b> toevoegen punt </b> en ga of kaart de unieke sleutel en de waarde in die dat punt identificeren. </td> 
  </tr> 
 </tbody> 
</table>

### Een aangepaste API-aanroep maken

Deze actiemodule maakt een douanevraag aan de de Financiën en API van Verrichtingen van de Dynamiek.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
    <td> <p>Voor instructies over het verbinden van Microsoft Dynamics 365 Financiën en Verrichtingen met [!DNL Workfront Fusion], zie <a href="#create-a-connection" class="MCXref xref"> een verbinding </a> in dit artikel creëren.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">URL</td> 
   <td> <p>Ga een weg met betrekking tot uw de Financiën en van Verrichtingen URL van de Dynamiek in.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Method]</td> 
   <td> <p>Selecteer de HTTP- verzoekmethode u de API vraag moet vormen. Zie <a href="../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref" data-mc-variable-override=""> HTTP-aanvraagmethoden in [!DNL Adobe Workfront Fusion]</a> voor meer informatie.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Headers]</td> 
   <td> <p>Voeg de kopteksten van het verzoek toe in de vorm van een standaard JSON-object. Dit bepaalt het inhoudstype van het verzoek.</p> <p>Bijvoorbeeld:<code> {"Content-type":"application/json"}</code></p> <p>Opmerking: als u fouten krijgt en het moeilijk is om de oorsprong ervan te bepalen, kunt u overwegen koppen te wijzigen op basis van de documentatie van [!DNL Workfront] . Wanneer uw Aangepaste API-aanroep een HTTP-aanvraagfout van 422 retourneert, probeert u een header <code>"Content-Type":"text/plain"</code> te gebruiken.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Query string]</td> 
   <td> <p>Voeg de query voor de API-aanroep toe als een standaard JSON-object.</p> <p>Bijvoorbeeld: <code>{"name":"something-urgent"}</code></p> <p>Tip: We raden u aan informatie via de JSON-hoofdtekst te verzenden in plaats van als queryparameters.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Body]</td> 
   <td> <p>Voeg de inhoud van de hoofdtekst voor de API-aanroep toe in de vorm van een standaard JSON-object.</p> <p>Opmerking:  <p>Wanneer u voorwaardelijke instructies gebruikt, zoals <code>if</code> in uw JSON, plaatst u de aanhalingstekens buiten de voorwaardelijke instructie.</p> 
     <div class="example" data-mc-autonum="<b>Example: </b>"> 
      <p> <img src="assets/quotes-in-json-350x120.png" style="width: 350;height: 120;"> </p> 
     </div> </p> </td> 
  </tr> 
 </tbody> 
</table>



### Entiteitsitem lezen

Deze actiemodule retourneert gegevens van een entiteitsitem. Het item wordt aangegeven door de velden Primaire sleutel.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
    <td>[!UICONTROL Connection]</td>
    <td> <p>Voor instructies over het verbinden van Microsoft Dynamics 365 Financiën en Verrichtingen met [!DNL Workfront Fusion], zie <a href="#create-a-connection" class="MCXref xref"> een verbinding </a> in dit artikel creëren.</p> </td> 
  </tr> 
  <tr> 
    <td>[!UICONTROL Entity]</td>
     <td>Ga of kaart het de entiteitstype van de Financiën en van Verrichtingen van de Dynamiek in dat u wilt lezen.</td> 
  </tr> 
  <tr> 
    <td>[!UICONTROL Primary key fields]</td>
     <td> In de velden Primaire sleutel wordt het item geïdentificeerd. Voor elk primair zeer belangrijk gebied dat u wilt verstrekken, klik <b> toevoegen punt </b> en ga of kaart de unieke sleutel en de waarde in die dat punt identificeren. </td> 
  </tr> 
 </tbody> 
</table>

### Entiteitsitem bijwerken

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
    <td>[!UICONTROL Connection]</td>
    <td> <p>Voor instructies over het verbinden van Microsoft Dynamics 365 Financiën en Verrichtingen met [!DNL Workfront Fusion], zie <a href="#create-a-connection" class="MCXref xref"> een verbinding </a> in dit artikel creëren.</p> </td> 
  </tr> 
  <tr> 
    <td>[!UICONTROL Entity]</td>
     <td>Ga of kaart het de entiteitstype van de Financiën en van Verrichtingen van de Dynamiek in dat u wilt bijwerken.</td> 
  </tr>  
  <tr> 
    <td>[!UICONTROL Primary key fields]</td>
     <td> In de velden Primaire sleutel wordt het item geïdentificeerd. Voor elk primair zeer belangrijk gebied dat u wilt verstrekken, klik <b> toevoegen punt </b> en ga of kaart de unieke sleutel en de waarde in die dat punt identificeren. </td> 
  </tr> 
  <tr> 
    <td>[!UICONTROL Body]</td>
     <td> <p>Ga of kaart een lichaam JSON in dat de gegevens bevat die u in het nieuwe entiteitpunt wilt omvatten.</p> </td> 
  </tr> 
 </tbody> 
</table>

### Zoeken

Deze zoekmodule retourneert resultaten op basis van criteria die u opgeeft.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection]</td> 
   <td> <p>Zie <a href="#connect-workfront-to-workfront-fusion" class="MCXref xref"> Verbinding maken [!DNL Workfront] met [!DNL Workfront Fusion]</a> in dit artikel voor instructies over het verbinden van uw [!DNL Workfront] -app met [!DNL Workfront Fusion] .</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Entity]</td> 
   <td>Ga of kaart het de entiteitstype van de Financiën en van Verrichtingen van de Dynamiek in dat u wilt zoeken.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Search criteria]</td> 
   <td> <p>Voer het veld in waarnaar u wilt zoeken, de operator die u in de query wilt gebruiken en de waarde waarnaar u in het veld zoekt.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Limit]</td> 
   <td> <p>Ga of kaart het maximumaantal verslagen in u de module tijdens elke cyclus van de scenariouitvoering wilt terugkeren.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Sort by]</td> 
   <td> <p>Typ of wijs het veld toe waarop u de resultaten wilt sorteren.</p> </td> 
  </tr> 
 </tbody> 
</table>


<!--

### List All

This module lists all records for a given entity.  The item is identified by its Primary key fields.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
    <td>[!UICONTROL Connection]</td>
    <td> <p>For instructions about connecting Microsoft Dynamics 365 Finance and Operations to [!DNL Workfront Fusion], see <a href="#create-a-connection" class="MCXref xref">Create a connection</a> in this article.</p> </td> 
  </tr> 
  <tr> 
    <td>[!UICONTROL Record Type]</td>
     <td>Choose the Dynamics Finance and Operations entity type that you want the module to list.</td> 
  </tr> 
  <tr> 
    <td>[!UICONTROL Outputs]</td>
     <td> <p>Select the information you want included in the output bundle for this module.</p> </td> 
  </tr> 
 </tbody> 
</table>

### Watch Record

This trigger module starts a scenario when a record of the given type is created or updated.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
    <td> <p>For instructions about connecting Microsoft Dynamics 365 Finance and Operations to [!DNL Workfront Fusion], see <a href="#create-a-connection" class="MCXref xref">Create a connection</a> in this article.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Record Type]</td> 
   <td> <p>Select the type of [!DNL Workfront] record that you want the module to watch.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Filter]</td> 
   <td> <p>Enter the field that you want to search by, the operator you want to use in your query, and the value that you are searching for in the field.</p> <p>Note: Do not use <code>username </code>in your search criteria. Including <code>username </code>in an API query to [!DNL Workfront] logs the user into Workfront, and the search will not be successful.</p> <p>Note: <code>In</code> and <code>NotIn</code>work with arrays. The inputs should be in array format.</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Limit]</td> 
   <td> <p>Enter or map the maximum number of records you want the module to return during each scenario execution cycle.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Outputs]</td> 
   <td> <p>Select the information you want included in the output bundle for this module.</p> </td> 
  </tr> 
 </tbody> 
</table>

-->
