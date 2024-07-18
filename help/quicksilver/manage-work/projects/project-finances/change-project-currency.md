---
product-area: projects
navigation-topic: financials
title: De projectvaluta wijzigen
description: Als projectmanager, kunt u een project vormen om een munt buiten de standaardmunt voor uw systeem van Adobe Workfront te gebruiken. Hierdoor kunt u financiële informatie over uw project in de gewenste valuta weergeven bij het berekenen van de arbeidskosten en -inkomsten.
author: Alina
feature: Work Management
exl-id: c496fe92-5c17-41a5-972b-1c063643bde3
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '564'
ht-degree: 0%

---

# De projectvaluta wijzigen

Als projectmanager, kunt u een project vormen om een munt buiten de standaardmunt voor uw systeem van Adobe Workfront te gebruiken. Hierdoor kunt u financiële informatie over uw project in de gewenste valuta weergeven bij het berekenen van de arbeidskosten en -inkomsten.

Alvorens u afwisselende die valuta kunt gebruiken zoals in deze sectie wordt beschreven, moet de beheerder van Workfront veelvoudige die valuta eerst toelaten en vormen, zoals in het artikel [ wordt beschreven de wisselkoers van de opstelling ](../../../administration-and-setup/manage-workfront/exchange-rates/set-up-exchange-rates.md).

## Toegangsvereisten

U moet de volgende toegang hebben om de stappen in dit artikel uit te voeren:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-abonnement*</td> 
   <td> <p>Alle</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-licentie*</td> 
   <td> <p>Plan </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraties op toegangsniveau*</td> 
   <td> <p>Toegang tot projecten bewerken</p> <p>Opmerking: als u nog steeds geen toegang hebt, vraag dan aan de Workfront-beheerder of deze aanvullende beperkingen op uw toegangsniveau heeft ingesteld. Voor informatie over hoe een beheerder van Workfront uw toegangsniveau kan wijzigen, zie <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref"> tot douanetoegangsniveaus </a> leiden of wijzigen.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objectmachtigingen</td> 
   <td> <p>Rechten voor een project beheren</p> <p>Voor informatie bij het vragen van om extra toegang, zie <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref"> de toegang van het Verzoek tot voorwerpen </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42; om te weten te komen welk plan, vergunningstype, of toegang u hebt, contacteer uw beheerder van Workfront.

## Overwegingen bij het wijzigen van de valuta van een project in Workfront

* U kunt de valuta van een project niet wijzigen als er financiële informatie in het project staat.
* Tarieven worden gebruikt voor loonkosten; inkomstenberekeningen en worden in de toekomst gebruikt voor rapportagedoeleinden.
* Als u voor een project geen andere valuta opgeeft, gaat Workfront ervan uit dat de valuta van het project de standaardvaluta van het systeem is. Voor informatie over systeem-vlakke standaardmunt, zie [ de wisselkoers van de Opstelling ](../../../administration-and-setup/manage-workfront/exchange-rates/set-up-exchange-rates.md).
* Standaard hebben alle gebruikers van volledige licenties toegang tot valuta&#39;s en wisselkoersen. De beheerder van Workfront moet extra administratieve toegang voor **Wisselkoersen** verlenen om gebruikers toe te laten om specifieke tarieven op projecten te plaatsen.
* De wisselkoersen in Workfront zijn niet dynamisch. De waarde wordt geplaatst door een beheerder en moet worden bijgewerkt wanneer de veranderingen in wisselkoersen voorkomen.
* Wanneer u een rapport creeert om op munt op een project te wijzen, door gebrek worden alle rapporten gegroepeerd door de standaardmunt van het project. Als u een rapport met veelvoudige projecten creeert die verschillende wisselkoersen hebben, dan wijzen om het even welke groeperingen die op het project worden toegepast op de standaardwisselkoers op het systeemniveau aan. Voor meer informatie, zie het artikel [ financiële gegevensrapporten met unieke wisselkoersen ](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-financial-data-reports-unique-exchange-rates.md) creëren.

## De valuta voor een project configureren

1. Ga naar het project waar u de standaardvaluta wilt veranderen.

   >[!TIP]
   >
   >Ervoor zorgen dat het project nog geen financiële informatie heeft. Zorg er bijvoorbeeld voor dat er geen geplande of werkelijke kosten verbonden zijn aan het project.

1. Klik **Details van het Project** in het linkerpaneel, dan ga naar het **Financiën** gebied.
1. Klik **toevoegen** in het **3} gebied van de Valuta {en selecteer de munt die u als standaardmunt voor het project wilt gebruiken.** Alle valuta&#39;s die uw Workfront-beheerder voor uw Workfront-exemplaar heeft ingesteld, worden weergegeven.

   ![](assets/currency-on-project-expanded-nwe.png)

1. (Voorwaardelijk) Als u een andere valuta dan de standaardvaluta selecteert die voor uw Workfront-systeem is ingesteld, geeft u de wisselkoers op voor de valuta die u hebt geselecteerd, aangezien deze betrekking heeft op de valuta die is ingesteld als de basisvaluta in het systeem.
1. Klik **sparen Veranderingen**.
