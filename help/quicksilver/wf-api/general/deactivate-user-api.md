---
content-type: api
product-area: user-management
navigation-topic: general-api
title: Een gebruiker deactiveren via de API
description: Een gebruiker deactiveren via de API
author: John
feature: Workfront API
exl-id: 45b06cce-4622-4739-b9f3-2edb9101c099
source-git-commit: c1cec2c08c66c704385cde1abd0c019fd59702da
workflow-type: tm+mt
source-wordcount: '199'
ht-degree: 0%

---


# Een gebruiker deactiveren via de API

Wanneer een gebruiker uw organisatie verlaat, kunt u de gebruiker deactiveren, hun Adobe Workfront-licentie beschikbaar maken voor een andere gebruiker en voorkomen dat deze per ongeluk werk krijgt toegewezen. Door een gebruiker te deactiveren, behoudt u de werkgeschiedenis, inclusief de werktoewijzingen en de koppeling met notities, uren en documenten.

Als u meer wilt weten over het deactiveren van een gebruiker, raadpleegt u &quot; [Een gebruiker deactiveren of opnieuw activeren](../../administration-and-setup/add-users/create-and-manage-users/deactivate-a-user.md).

Voor informatie over het gebruik van de Core API raadpleegt u [Basisbeginselen van API](../../wf-api/general/api-basics.md).

Een gebruiker deactiveren via de API:

1. Een API-sleutel genereren met behulp van de volgende API-aanvraag:

```
<domain>.my.workfront.com/attask/api/v15.0/user?action=generateApiKey&username=`username`&password=`password`&method=PUT`
```

1. Zoek GUID voor de gebruiker die u wilt deactiveren.

   1. Gebruik het volgende API verzoek om GUID voor alle gebruikers in uw systeem terug te winnen, merk op dat **isActive** veldpresentaties **true** voor gebruikers die momenteel actief zijn en **false** voor gedeactiveerde gebruikers:

```
<domain>`.my.workfront.com/attask/api/v15.0/USER/search?fields=isActive
```

1. Zoek GUID voor de gebruiker die u wilt deactiveren, gebruik het volgende **PUT** verzoek om de gebruiker te wijzigen **isActive** veldwaarde naar **false**:

```
<domain>`.my.workfront.com/attask/api/v15.0/USER/`<user's GUID>`?updates={"isActive":"false"}&method=put&apiKey=`<apiKey>`&fields=isActive
```

1. Uit het antwoord zal blijken dat de **isActive** veldwaarde is gewijzigd van **true** tot **false** die aangeeft dat de gebruiker is gedeactiveerd:

<!-- [Copy](javascript:void(0);) -->
<pre></pre>
