---
user-type: administrator
product-area: system-administration;user-management
navigation-topic: manage-group-statuses
title: Hoe groepen statussen overerven
description: Wanneer u de statussen opsomt die beschikbaar zijn voor een groep, ziet u het volgende
author: Caroline
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: 3937fd72-fa54-4777-9ec4-1f097df7a2ee
source-git-commit: 5d36c2c959dbfd00920eaf0a16409102b99de042
workflow-type: tm+mt
source-wordcount: '599'
ht-degree: 0%

---

# Hoe groepen statussen overerven

Wanneer u de statussen opsomt die beschikbaar zijn voor een groep, ziet u het volgende

* De statussen van de douane die voor de groep worden gecreeerd, zoals die in [ worden verklaard creëren of uitgeven een groepsstatus ](../../../administration-and-setup/manage-groups/manage-group-statuses/create-or-edit-a-group-status.md).
* Statussen die van het systeem en van hoger in de groepshiërarchie worden overgeërfd, zoals in dit artikel wordt uitgelegd.

## Statussen overnemen

Uw groep erft statussen wanneer een van de volgende dingen gebeurt:

* U maakt de groep.
* Een beheerder sluit een status in een hoger niveaugroep.
* Een beheerder verwijdert een andere groep en kiest uw groep om deze plaats in te nemen.

In de onderstaande tabel wordt elk van deze omstandigheden toegelicht.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Wanneer u een groep maakt</td> 
   <td> <p>Wanneer u een nieuwe groep maakt, overerft deze automatisch:</p> 
    <ul> 
     <li>De niet-vergrendelde status in de groep één niveau omhoog, als de nieuwe groep een subgroep is.</li> 
    </ul> 
    <ul> 
     <li>Vergrendelde statussen op systeemniveau.</li> 
    </ul> 
     <b> VOORBEELD:</b></span></span> 
     <p>Veronderstel dat een groep genoemd Marketing 2 subgroepen genoemd de Mededelingen van de Marketing en Branding heeft.</p> 
     <p>Een groepbeheerder van de marketinggroep maakt een nieuwe aangepaste status met de naam Discovery.</p> 
     <p>Later, creeert u een nieuwe subgroep onder de groep van de Marketing en roept het Advertising.</p> 
     <p>Uw subgroep erft de status van de Ontdekking omdat u de groep creeerde nadat de andere beheerder de ontgrendelde status van de Ontdekking creeerde.</p> 
     <p>Omdat de subgroepen Marketing Communications en Branding al onder de marketinggroep bestonden toen dit gebeurde, nemen ze de ontgrendelde status van Detectie niet over.</p> 
    </div> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Wanneer een beheerder een status op een hoger niveau vergrendelt</td> 
   <td> <p>Wanneer een beheerder van Workfront een status op systeemniveau sluit, erft uw groep het samen met alle andere groepen in het systeem.</p> <p>Op dezelfde manier wanneer een beheerder een status voor een groep boven uw groep sluit, erft uw groep het samen met andere subgroepen onder de hogere groep.</p> <p><b> NOTA </b>: Later, als een beheerder één van deze statussen op het systeemniveau of in een groep boven uw groep ontgrendelt, behoudt uw groep de status die het vroeger erft. Het is nu een aparte versie van de status en u kunt deze alleen voor uw groep aanpassen.</p> 
    <p><b>VOORBEELD</b></p>
    <p>De de groepsbeheerder van de Marketing sluit de hierboven vermelde status van de Ontdekking om ervoor te zorgen dat alle 3 subgroepen het hebben.</p> 
    <p>Samen met uw Advertising-groep hebben de groepen Marketing Communications en Branding nu de status Discovery. Zij erven het toen het in de Marketing groep boven hen werd gesloten.</p> 
    <p>De de groepsbeheerder van de Marketing ontgrendelt dan de status van de Ontdekking zodat alle drie subgroepen hun eigen versie van de status van de Ontdekking hebben. Nu kunnen u en de beheerders van de andere twee groepen de status van de Ontdekking aanpassen om aan de behoeften van uw groepen te voldoen.</p> 
  </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Wanneer een beheerder een groep verwijdert</td> 
   <td> <p>Wanneer een beheerder een groep schrapt en van u verkiest om zijn plaats in het systeem te nemen, erft uw groep de douanestatus van de geschrapte groep als zij niet reeds in uw groep bestaan.</p> 
   <p><b>VOORBEELD </b></p>
     <p>Een groep genoemd Overseinen moet met uw groep van Advertising samenvoegen, zodat schrapt een beheerder van Workfront de groep van het Overseinen en kiest uw groep om zijn plaats te nemen.</p> 
     <p>De groep van het Overseinen had een unieke status genoemd in Proces. Je Advertising-groep heeft nu die status beschikbaar voor gebruik.</p> 
    </div> </td> 
  </tr> 
 </tbody> 
</table>

## Statusconfiguraties overnemen

Wanneer u een top-level groep creeert, erft het de volgende configuraties van het systeemniveau. Wanneer u een subgroep maakt, overerft deze de volgende configuraties van de volgende hogere groep.

* Standaardstatusconfiguraties

  Voor informatie over deze, zie [ de douanestatus van het Gebruik als standaardstatussen ](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/use-custom-statuses-as-default-statuses.md).

* Configuraties van de statusweergavevolgorde

  Voor informatie over deze, zie [ systeem-niveau en groepsstatussen opnieuw ordenen ](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/reorder-system-statuses.md).

Als iemand deze configuraties wijzigt nadat de groep is gemaakt, heeft dit geen invloed op de status.
