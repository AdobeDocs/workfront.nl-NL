---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: get-started-with-workfront-fusion-2-0
title: IP Adressen om tot de Fusie van Adobe Workfront toegang te hebben
description: Adobe Workfront Fusion vereist naast een Adobe Workfront-licentie een Adobe Workfront Fusion-licentie.
author: Becky
feature: Workfront Fusion
exl-id: f6295cc7-367f-4c8b-891b-cc11ff42a225
source-git-commit: 55a4fda46f6d314c71d9ef98864b21b84f946b09
workflow-type: tm+mt
source-wordcount: '178'
ht-degree: 0%

---

# IP Adressen voor de toegang tot [!DNL Adobe Workfront Fusion]

>[!NOTE]
>
>[!DNL Adobe Workfront Fusion] vereist een [!DNL Adobe Workfront Fusion] naast een [!DNL Adobe Workfront license].

Als uw firewall of postserver wordt gevormd om toegang tot slechts bepaalde verkopers toe te staan, moet u bepaalde IP adressen aan zijn lijst van gewenste personen toevoegen om open communicatie tussen uw milieu en toe te staan [!DNL Adobe Workfront Fusion].

Voeg de volgende IP adressen aan uw lijst van gewenste personen toe om toe te laten [!DNL Workfront Fusion] om toegang te krijgen tot uw systeem.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] EU-datacenter</td> 
   <td> 
    <ul> 
     <li>52 30 133 50</li> 
     <li>54 220 93 204</li> 
     <li>34 254 76 122</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!DNL Adobe Workfront] VS-datacenter</p> </td> 
   <td> 
    <ul> 
     <li>54 244 142 219</li> 
     <li>52 39 217 230</li> 
     <li>44 241 82 96</li>
     <li>10.20.126.137</li>
     <li>34 223 32,4</li>
     <li>52 39 176 220</li>
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront Fusion] op de Microsoft Azure-cluster</td> 
   <td> 
    <ul> 
     <li>20.36.133.48/28</li> 
     <li>20.81.156.240/28</li> 
     <li>172.172.84.48/28</li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

Ook, als uw organisatie uitgaande netwerk het filtreren gebruikt, voeg het volgende domein aan uw lijst van gewenste personen toe om uw systeem toe te laten om tot Workfront Fusion toegang te hebben.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] EU-datacenter</td> 
   <td> <p> hook.app-eu.workfrontfusion.com </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!DNL Adobe Workfront] VS-datacenter</p> </td> 
   <td> <p>hook.app.workfrontfusion.com </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!DNL Adobe Workfront Fusion] op de Microsoft Azure-cluster</p> </td> 
   <td> <p>hook.app-az.workfrontfusion.com </p> </td> 
  </tr> 
 </tbody> 
</table>

>[!NOTE]
>
>Het uitgaande netwerk filtreren is ongewoon. Controleer met uw netwerkbeheerder om te zien of moet u uw lijst van gewenste personen bijwerken om voor het aan te passen.

Voor meer informatie over vestiging de lijst van gewenste personen van uw organisatie, zie [De lijst van gewenste personen van uw firewall configureren](../../administration-and-setup/get-started-wf-administration/configure-your-firewall.md).
