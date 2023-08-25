---
title: Klassieke lay-outsjablonen verwijderen
user-type: administrator
product-area: system-administration;templates;user-management
navigation-topic: layout-templates
description: Layoutsjablonen uit de klassieke Workfront-ervaring zijn niet meer beschikbaar in de Workfront-interface, maar kunnen nog steeds van invloed zijn op Workfront-gegevens. Dit kan inconsistenties veroorzaken in velden die worden beïnvloed door lay-outsjablonen (zoals Gedeeld met) in rapporten of dashboards.
author: Becky
feature: System Setup and Administration
role: Admin
source-git-commit: c68b63230b07ea8c8475b710e256b5e0f049b1eb
workflow-type: tm+mt
source-wordcount: '280'
ht-degree: 0%

---

# Administratieve toegang verlenen voor een lay-outsjabloon

Layoutsjablonen uit de klassieke Workfront-ervaring zijn niet meer beschikbaar in de Workfront-interface, maar kunnen nog steeds van invloed zijn op Workfront-gegevens. Dit kan inconsistenties veroorzaken in velden die worden beïnvloed door lay-outsjablonen (zoals Gedeeld met) in rapporten of dashboards.

U kunt deze inconsistenties oplossen door de klassieke lay-outsjablonen te verwijderen. Aangezien deze niet beschikbaar zijn in de Workfront-interface, moet u ze verwijderen met de Workfront API.

## Toegangsvereisten

U moet de volgende toegang hebben om de stappen in dit artikel uit te voeren:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-plan</td> 
   <td>Alle</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-licentie</td> 
   <td>Plan</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraties op toegangsniveau</td> 
   <td> <p>Om deze stappen op systeemniveau uit te voeren, hebt u het toegangsniveau van de Beheerder van het Systeem nodig.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Verwijder de klassieke lay-outsjablonen met een API-aanroep

U kunt API-aanroepen invoeren in de URL-balk van uw browser en op Enter drukken. De API-reactie wordt weergegeven in uw browser.

>[!NOTE]
>
>De globale en de lay-outmalplaatjes van het Systeem kunnen niet worden geschrapt.

1. Meld u aan bij Workfront.
1. Zoek de lay-outsjabloon die u wilt verwijderen met behulp van de volgende API-aanroep:
   `https://{yourDomain}.com/attask/api/v16.0/LYTMPL/search`
1. Noteer de id van de lay-outsjabloon die u wilt verwijderen.
1. Zoek de sessie-id met de volgende API-aanroep:
   `https://{yourDomain}.com/attask/api/v16.0/session`

   >[!IMPORTANT]
   >
   >Deel uw sessie-id nooit met iemand.

1. Plaats de id van de lay-outsjabloon en de sessie-id in de volgende API-aanroep:
   `https://{yourDomain}.com/attask/api/v16.0/LYTMPL?ID={layoutTemplateID}&method=delete&sessionID={yourSessionID}`
1. Plak de API-aanroep vanuit stap 4 in de URL-balk van uw browser en druk op Enter.

   Hiermee verwijdert u de lay-outsjabloon.



