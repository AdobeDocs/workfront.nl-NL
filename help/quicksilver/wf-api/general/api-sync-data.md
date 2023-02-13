---
content-type: api
keywords: API,gegevens,sync,dagboek,item,object
navigation-topic: general-api
title: Gebruik de API om gegevens voor programma's en services te synchroniseren
description: Gebruik de API om gegevens voor programma's en services te synchroniseren
author: John
feature: Workfront API
exl-id: 1d0583fc-1573-4279-a3fa-a912d9a4213c
source-git-commit: e6bad8cbe84d0f116e9679ecaba5178973a2604f
workflow-type: tm+mt
source-wordcount: '472'
ht-degree: 0%

---


# De API gebruiken om gegevens voor programma&#39;s en services te synchroniseren

Dit zijn enkele algemene manieren waarop u de API kunt gebruiken om gegevens voor programma&#39;s en services te synchroniseren.

## Bijna realtime updates

Adobe Workfront gebruikt &quot;Event Subscriptions&quot; (ook wel webhooks genoemd) om updates in real time over ondersteunde objecten en acties via de API naar het gewenste eindpunt of de gewenste eindpunten te verzenden. U kunt een update voor nieuwe objecten en acties verwachten binnen 5 seconden, maar de updates zijn gemiddeld over ongeveer 1 seconde beschikbaar. Voor meer informatie over welk type objecten wordt ondersteund, welke typen acties worden ondersteund, technische details en voorbeelden van hoe u gebeurtenisabonnementen kunt instellen, raadpleegt u [Event Subscription API](../../wf-api/general/event-subs-api.md) en [Vereisten voor levering van abonnementen](../../wf-api/general/setup-event-sub-endpoint.md).

## Batchupdates

Updates in batch zijn een manier om uw systeem te configureren voor updates door periodieke aanvragen naar Workfront-servers uit te voeren. Er zijn veel manieren om dit te doen, maar over het algemeen bestaat het proces uit het hebben van uw dienst een verzoek aan de servers van Workfront API en het zoeken naar voorwerpen die sinds de laatste verzoekvraag zijn gecreeerd of gewijzigd. Voor informatie over potentiële verzoeken en nuttige parameters gelieve te zien gelieve [Gedrag van GET](../../wf-api/general/api-basics.md#get-behavior) van de [Basisbeginselen van API](../../wf-api/general/api-basics.md) artikel.

Aangezien u opstelling uw dienst voor batch-updates bent zijn een paar belangrijke dingen om in mening te houden:

### Invoerdatums

Invoerdatums worden opgeslagen met ISO 8601-opmaak. Deze standaard bevat gegevens over datum, tijd en tijdzone.

**Voorbeeld:** Datumnotatie ISO 8601

<!-- [Copy](javascript:void(0);) -->
 
<pre><code>2020-05-18T17:00:00:000-0600</code></pre> 

Zowel de datum waarop een object is gemaakt als de laatste datum waarop het object is gewijzigd, worden opgeslagen als respectievelijk &quot;entryDate&quot; en &quot;lastUpdateDate&quot;. Zie voor uitgebreide informatie over Workfront-objecten, de bijbehorende velden en veldnamen de [API Explorer](../../wf-api/general/api-explorer.md). De entryDate voor een bepaald Workfront-object verandert niet, waarbij de lastUpdatedDate telkens wanneer het object wordt gewijzigd, verandert.

**Voorbeeld:** GET-aanvraag voor een uitgaveobject, met gebruik van de **lastUpdateDate** veld. Dit verzoek retourneert alle problemen die sinds die opgegeven datum zijn bijgewerkt.

<!-- [Copy](javascript:void(0);) -->
 

```
GET
https://<domain>.my.workfront.com/attask/api/v11.0/OPTASK/search?fields=ID,name,lastUpdateDate&$$LIMIT=200&lastUpdateDate=2020-05-13T18:18:37.255Z&lastUpdateDate_Mod=gte
```

### Object Dagboekinvoer

Als u wijzigingen met betrekking tot een specifiek veld op een object wilt verkrijgen, kunt u het object Journal Entry opvragen. Het Workfront Journal Entry-object kan zo worden ingesteld dat informatie over specifieke objectvelden wordt geregistreerd wanneer deze velden worden gewijzigd, zie [Systeemupdates configureren](../../administration-and-setup/set-up-workfront/system-tracked-update-feeds/configure-system-updates.md) voor meer informatie.

Wanneer een gebied opstelling is om als deel van het voorwerp van de Ingang van het Dagboek worden geregistreerd zal een overeenkomstige Ingang van het Dagboek worden gecreeerd telkens als dat gebied wordt gewijzigd. Dan, kunt u het voorwerp van de Ingang van het Dagboek vragen gebruikend een API vraag gelijkend op het volgende:

<!-- [Copy](javascript:void(0);) -->

<pre><code>GET https://&#123;&#123;domain&#125;&#125;.my.workfront.com/attask/api/v11.0/JRNLE/search?fields=newTextVal,oldTextVal,newDateVal,oldDateVal,newNumberVal,oldNumberVal,entryDate,objObjCode,objID,fieldName&fieldName=name&objObjCode=OPTASK&entryDate=2020-05-13T18:18:37.255Z&entryDate_Mod=gte</code></pre>

>[!NOTE]
>
>&quot;entryDate&quot; wordt gebruikt om naar een dagboekingang van een verandering te kijken, in tegenstelling tot het bekijken van het veranderde voorwerp, zelf.
