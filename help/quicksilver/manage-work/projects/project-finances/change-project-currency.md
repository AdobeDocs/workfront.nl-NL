---
product-area: projects
navigation-topic: financials
title: De projectvaluta wijzigen
description: Als projectmanager, kunt u een project vormen om een munt buiten de standaardmunt voor uw systeem van Adobe Workfront te gebruiken. Hierdoor kunt u financiële informatie over uw project in de gewenste valuta weergeven bij het berekenen van de arbeidskosten en -inkomsten.
author: Lisa
feature: Work Management
exl-id: c496fe92-5c17-41a5-972b-1c063643bde3
source-git-commit: b983a780198743a2b87b4b48cf4d6afdf1cee437
workflow-type: tm+mt
source-wordcount: '532'
ht-degree: 0%

---

# De projectvaluta wijzigen

Als projectmanager, kunt u een project vormen om een munt buiten de standaardmunt voor uw systeem van Adobe Workfront te gebruiken. Hierdoor kunt u financiële informatie over uw project in de gewenste valuta weergeven bij het berekenen van de arbeidskosten en -inkomsten.

Alvorens u afwisselende die valuta kunt gebruiken zoals in deze sectie wordt beschreven, moet de beheerder van Workfront veelvoudige die valuta eerst toelaten en vormen, zoals in het artikel [ wordt beschreven de wisselkoers van de opstelling ](../../../administration-and-setup/manage-workfront/exchange-rates/set-up-exchange-rates.md).

## Toegangsvereisten

+++ Breid uit om de toegangseisen voor de functionaliteit in dit artikel weer te geven.

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
   <td>
   <p>Nieuw: Standaard</p>
   <p>of</p>
   <p>Huidig: Plan</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraties op toegangsniveau</td> 
   <td>Toegang tot projecten bewerken</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objectmachtigingen</td> 
   <td>Rechten voor een project beheren</td> 
  </tr> 
 </tbody> 
</table>

Voor meer detail over de informatie in deze lijst, zie [ vereisten van de Toegang in de documentatie van Workfront ](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

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
1. Klik **toevoegen** in het **3&rbrace; gebied van de Valuta &lbrace;en selecteer de munt die u als standaardmunt voor het project wilt gebruiken.** Alle valuta&#39;s die uw Workfront-beheerder voor uw Workfront-exemplaar heeft ingesteld, worden weergegeven.

   ![ Valuta op project ](assets/currency-on-project-expanded-nwe.png)

1. (Voorwaardelijk) Als u een andere valuta dan de standaardvaluta selecteert die voor uw Workfront-systeem is ingesteld, geeft u de wisselkoers op voor de valuta die u hebt geselecteerd, aangezien deze betrekking heeft op de valuta die is ingesteld als de basisvaluta in het systeem.
1. Klik **sparen Veranderingen**.
