---
filename: api-changes-search
content-type: api
keywords: object,status,zoeken,best,werkwijze,reactie
navigation-topic: api-navigation-topic
title: 'Core API-wijzigingen: Reacties voor zoeken naar status'
description: Wijzigingen in de manier waarop Workfront statusobjecten opslaat.
exl-id: 322f1525-d1d5-4845-a590-e34eb94ccdc2
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '446'
ht-degree: 0%

---

# Core API-wijzigingen: Antwoorden van statuszoekacties

Er zijn wijzigingen aangebracht in de manier waarop Workfront statusobjecten opslaat. Deze wijzigingen zijn niet van invloed op de manier waarop aanvragen voor statuszoekopdrachten worden gedaan, maar hebben invloed op de reactie die wordt geretourneerd door API-verzoeken die een zoekopdracht naar statusobjecten bevatten door een onvolledige lijst met groepsstatussen te retourneren.

## Aanbevolen procedures

Om de volledige lijst van statussen betrouwbaar te halen beschikbaar voor een groep, worden de volgende verzoeken beschouwd als beste praktijken.

>[!NOTE]
>
>Deze aanvraagstructuren worden aanbevolen voor alle gebruikers, ongeacht of de wijzigingen in de statuszoekopdracht al dan niet in uw cluster zijn aangebracht.

Status projectgroep:

>**Voorbeeld:**

```
/attask/api/<VERSION>/CSTEM/projectGroupStatuses?groupID=602d27640000bb3b779f770d5fb95d6d
```

Status taakgroep:

>**Voorbeeld:**

```
/attask/api/<VERSION>/CSTEM/taskGroupStatuses?groupID=602d27640000bb3b779f770d5fb95d6d
```

Status van Issue Group:

>**Voorbeeld:**

```
/attask/api/<VERSION>/CSTEM/opTaskGroupStatuses?groupID=602d27640000bb3b779f770d5fb95d6d
```

Al deze drie eindpunten aanvaarden het **includeHidden=true** parameter om de verborgen status van een project/taak/uitgave van een bepaalde groep op te halen. Door het modelleren van query&#39;s voor statuszoekopdrachten na deze voorbeelden van best practices wordt ervoor gezorgd dat alle informatie over de groepsstatus in elke reactie wordt opgenomen.

Hier is een voorbeeld van een vraag van het statusonderzoek die aan een taakgroep wordt gemaakt die een systeem-vlakke gesloten status omvat **Aangepast_1** en een ontgrendelde status **Aangepast_2**:

>**Voorbeeld:**

```
/attask/api/<VERSION>/CSTEM/taskGroupStatuses?groupID=602d286d000004fc8f53942de697a868
```

Als u deze indeling gebruikt, zorgt u ervoor dat alle volgende elementen in uw reactie worden opgenomen:

```
{
    "data": [
        {
            "color": "1C68FF",
            "equatesWith": "NEW",
            "groupID": "602d27640000bb3b779f770d5fb95d6d",
            "label": "New",
            "objCode": "CSTEM",
            "value": "NEW"
        },
        {
            "color": "39FF39",
            "equatesWith": "INP",
            "groupID": "602d27640000bb3b779f770d5fb95d6d",
            "label": "In Progress",
            "objCode": "CSTEM",
            "value": "INP"
        },
        {
            "color": "FF3939",
            "equatesWith": "CPL",
            "groupID": "602d27640000bb3b779f770d5fb95d6d",
            "label": "Complete",
            "objCode": "CSTEM",
            "value": "CPL"
        },
        {
            "color": "8BC34A",
            "equatesWith": "NEW",
            "groupID": "602d27640000bb3b779f770d5fb95d6d",
            "label": "Custom_1",
            "objCode": "CSTEM",
            "value": "JET"
        },
        {
            "color": "8BC34A",
            "equatesWith": "NEW",
            "groupID": "602d27640000bb3b779f770d5fb95d6d",
            "label": "Custom_2",
            "objCode": "CSTEM",
            "value": "OGC"
        }
    ]
}
```

## Wijzigingen in zoekquery voor oudere status begrijpen

Onder het oudere systeem zou een vraag van het statusonderzoek alle systeemstatussen kopi??ren beschikbaar voor alle groepen inbegrepen in een vraag. De erfenisreactie zou dan alle systeemstatussen en groep-vlakke statussen omvatten beschikbaar voor elke groep in vraag.

Deze query (die de huidige aanbevolen aanbevolen tips niet volgt):

>**Voorbeeld:**

```
/attask/api/<VERSION>/CSTEM/search?groupID=602d27640000bb3b779f770d5fb95d6d&enumClass=STATUS_TASK
```

Dit zou de volgende reactie hebben onder het oudere systeem, dat alle objectstatussen bevat:

```
{
    "data": [
        {
            "color": "1C68FF",
            "equatesWith": "NEW",
            "groupID": "602d27640000bb3b779f770d5fb95d6d",
            "label": "New",
            "objCode": "CSTEM",
            "value": "NEW"
        },
        {
            "color": "39FF39",
            "equatesWith": "INP",
            "groupID": "602d27640000bb3b779f770d5fb95d6d",
            "label": "In Progress",
            "objCode": "CSTEM",
            "value": "INP"
        },
        {
            "color": "FF3939",
            "equatesWith": "CPL",
            "groupID": "602d27640000bb3b779f770d5fb95d6d",
            "label": "Complete",
            "objCode": "CSTEM",
            "value": "CPL"
        },
        {
            "color": "8BC34A",
            "equatesWith": "NEW",
            "groupID": "602d27640000bb3b779f770d5fb95d6d",
            "label": "Custom_1",
            "objCode": "CSTEM",
            "value": "JET"
        },
        {
            "color": "8BC34A",
            "equatesWith": "NEW",
            "groupID": "602d27640000bb3b779f770d5fb95d6d",
            "label": "Custom_2",
            "objCode": "CSTEM",
            "value": "OGC"
        }
    ]
}
```

Nochtans, na de updates aan de manier worden gemaakt dat de statussen worden opgeslagen en gebruikt, kopi??ren de statussen niet voor groepen en door elke groep op het systeemniveau ge??rft. Dientengevolge, leest de onderzoek API vraag slechts die statussen die direct met een bepaalde groep worden geassocieerd, zodat omvat de reactie systeem-gesloten en ontgrendelde statussen, maar slechts voor die groepen die werden gecreeerd nadat de status in kwestie werd toegevoegd.

Als u de bijgewerkte methoden van best practices niet gebruikt om zoekopdrachten naar status te maken nadat het oudere systeem is bijgewerkt, wordt een onvolledige lijst met groepsstatussen geretourneerd in de reactie.

Hier is een voorbeeld van wat deze verouderde verzoekstructuur terugkeert nadat het erfenissysteem is bijgewerkt:

>**Voorbeeld:**

```
/attask/api/<VERSION>/CSTEM/search?groupID=602d27640000bb3b779f770d5fb95d6d&enumClass=STATUS_TASK
```

Deze reactie omvat alleen groepsspecifieke statussen en laat de statussen die op systeemniveau zijn gedeclareerd, buiten beschouwing:

```
{
  "data": [
    {
      "color": "8BC34A",
      "equatesWith": "NEW",
      "groupID": "602d286d000004fc8f53942de697a868",
      "label": "Custom_2",
      "objCode": "CSTEM",
      "value": "MMI"
    }
  ]
}
```
