---
user-type: administrator
product-area: system-administration
navigation-topic: security
title: Toegang tot Adobe Workfront beperken tot IP-adres
description: U kunt een lijst van gewenste personen vormen van Adobe Workfront IP die toegang tot Workfront tot 75 IP adressen of IP adreswaaiers beperkt die u specificeert. Dit biedt een extra beveiligingslaag voor de Workfront-toepassing.
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: aed65b42-d534-453a-885d-f922114987bc
source-git-commit: 65121fae364683373d2bc9abbe6672755d0cd09c
workflow-type: tm+mt
source-wordcount: '477'
ht-degree: 0%

---

# Toegang tot Adobe Workfront beperken tot IP-adres

>[!IMPORTANT]
>
>Deze functionaliteit is momenteel niet beschikbaar voor organisaties die zijn aangemeld bij de Adobe Admin Console. Het zal in een toekomstige release beschikbaar zijn in de Adobe Admin Console.

U kunt een lijst van gewenste personen vormen van Adobe Workfront IP die toegang tot Workfront tot 75 IP adressen of IP adreswaaiers beperkt die u specificeert. Dit biedt een extra beveiligingslaag voor de Workfront-toepassing.

Deze IP adressen of IP adreswaaiers zouden door uw netwerkbeheerder moeten worden verstrekt.

## Toegangsvereisten

+++ Breid uit om de toegangseisen voor de functionaliteit in dit artikel weer te geven.

U moet het volgende hebben om de stappen in dit artikel uit te voeren:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-plan</td> 
   <td> <p>Enterprise</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-licentie</td> 
   <td>Plan</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraties op toegangsniveau</td> 
   <td> <p>U moet een Workfront-beheerder zijn.</p> <p><b> NOTA </b>: Als u nog geen toegang hebt, vraag uw beheerder van Workfront als zij extra beperkingen in uw toegangsniveau plaatsen. Voor informatie over hoe een beheerder van Workfront uw toegangsniveau kan wijzigen, zie <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref"> tot douanetoegangsniveaus </a> leiden of wijzigen.</p> </td> 
  </tr> 
 </tbody> 
</table>

+++

## Overige lijsten van gewenste personen

Als uw firewall of postserver wordt gevormd om toegang tot slechts bepaalde verkopers toe te staan, moet u bepaalde IP adressen aan zijn lijst van gewenste personen toevoegen. Hierdoor wordt de communicatie tussen uw omgeving en de Adobe Workfront-servers geopend. Voor informatie over dat, zie [ de lijst van gewenste personen van uw firewall ](../../../administration-and-setup/get-started-wf-administration/configure-your-firewall.md) vormen.

Als uw organisatie het Enterprise-abonnement gebruikt, kunt u de Workfront e-mailtoepassing configureren om te bepalen welke e-maildomeinen e-mails van Workfront mogen accepteren en welke e-maildomeinen zich in het e-mailadres kunnen bevinden dat gebruikers in hun Workfront-gebruikersprofiel opgeven. Voor meer informatie, zie [ uw e-maillijst van gewenste personen ](../../../administration-and-setup/get-started-wf-administration/configure-your-email-allowlist.md) vormen.

## IP adressen toevoegen aan de lijst van gewenste personen

Nadat u IP adressen aan de lijst van gewenste personen van Workfront toevoegt, slechts kunnen die IP adressen worden gebruikt om tot Workfront toegang te hebben. Gebruikers die Workfront proberen te openen vanaf een ander IP-adres ontvangen een foutbericht om aan te geven dat hun IP-adres is geblokkeerd.

{{step-1-to-setup}}

1. Klik **Systeem** > **Info van de Klant.**

1. In de **sectie van de lijst van gewenste personen van 0} IP, uitgezochte** laat IP lijst van gewenste personen toe.****

   Deze optie is standaard uitgeschakeld.

1. Geef het IP-adres op dat u momenteel gebruikt voor toegang tot het Workfront-systeem.

   of

   Geef een bereik van IP-adressen op dat het adres bevat dat u momenteel gebruikt om toegang te krijgen tot het Workfront-systeem.

   Het IP adres u gebruikt om tot Workfront toegang te hebben moet aan de lijst van gewenste personen worden toegevoegd alvorens de lijst van gewenste personen wordt toegelaten.

1. Klik **toevoegen IP Waaier,** dan specificeer het IP adres of de waaier van IP adressen die u tot Workfront wilt kunnen toegang hebben.
1. (Optioneel) Herhaal de vorige stap om extra IP-adressen of IP-adresbereiken toe te voegen.

   U kunt maximaal 75 adressen of bereiken toevoegen.

1. Klik **sparen.**
