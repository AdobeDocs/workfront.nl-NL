---
user-type: administrator
product-area: system-administration
navigation-topic: security
title: Toegang tot Adobe Workfront beperken tot IP-adres
description: U kunt een lijst van gewenste personen vormen van Adobe Workfront IP die toegang tot Workfront tot 45 IP adressen of IP adreswaaiers beperkt die u specificeert. Dit biedt een extra beveiligingslaag voor de Workfront-toepassing.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: aed65b42-d534-453a-885d-f922114987bc
source-git-commit: 7bd3d2252b124a07a112aaa2b7798063087e7cab
workflow-type: tm+mt
source-wordcount: '448'
ht-degree: 0%

---

# Toegang tot Adobe Workfront beperken tot IP-adres

U kunt een lijst van gewenste personen vormen van Adobe Workfront IP die toegang tot Workfront tot 45 IP adressen of IP adreswaaiers beperkt die u specificeert. Dit biedt een extra beveiligingslaag voor de Workfront-toepassing.

Deze IP adressen of IP adreswaaiers zouden door uw netwerkbeheerder moeten worden verstrekt.

## Toegangsvereisten

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
   <td> <p>U moet een Workfront-beheerder zijn.</p> <p><b>OPMERKING</b>: Als u nog steeds geen toegang hebt, vraagt u de Workfront-beheerder of deze aanvullende beperkingen op uw toegangsniveau instelt. Voor informatie over hoe een beheerder van Workfront uw toegangsniveau kan wijzigen, zie <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Aangepaste toegangsniveaus maken of wijzigen</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Overige lijsten van gewenste personen

Als uw firewall of postserver wordt gevormd om toegang tot slechts bepaalde verkopers toe te staan, moet u bepaalde IP adressen aan zijn lijst van gewenste personen toevoegen. Hierdoor wordt de communicatie tussen uw omgeving en de Adobe Workfront-servers geopend. Zie voor meer informatie hierover [De lijst van gewenste personen van uw firewall configureren](../../../administration-and-setup/get-started-wf-administration/configure-your-firewall.md).

Als uw organisatie het Enterprise-abonnement gebruikt, kunt u de Workfront e-mailtoepassing configureren om te bepalen welke e-maildomeinen e-mails van Workfront mogen accepteren en welke e-maildomeinen zich in het e-mailadres kunnen bevinden dat gebruikers in hun Workfront-gebruikersprofiel opgeven. Zie voor meer informatie [Uw e-maillijst van gewenste personen configureren](../../../administration-and-setup/get-started-wf-administration/configure-your-email-allowlist.md).

## IP adressen toevoegen aan de lijst van gewenste personen

Nadat u IP adressen aan de lijst van gewenste personen van Workfront toevoegt, slechts kunnen die IP adressen worden gebruikt om tot Workfront toegang te hebben. Gebruikers die Workfront proberen te openen vanaf een ander IP-adres ontvangen een foutbericht om aan te geven dat hun IP-adres is geblokkeerd.

1. Klik op de knop **Hoofdmenu** pictogram ![](assets/main-menu-icon.png) in de rechterbovenhoek van Adobe Workfront klikt u op **Instellen** ![](assets/gear-icon-settings.png).

1. Klikken **Systeem** > **Klantgegevens.**

1. In de **IP lijst van gewenste personen** sectie, selecteert u **Laat IP lijst van gewenste personen toe.**

   Deze optie is standaard uitgeschakeld.

1. Geef het IP-adres op dat u momenteel gebruikt voor toegang tot het Workfront-systeem.

   of

   Geef een bereik van IP-adressen op dat het adres bevat dat u momenteel gebruikt voor toegang tot het Workfront-systeem.

   Het IP adres u gebruikt om tot Workfront toegang te hebben moet aan de lijst van gewenste personen worden toegevoegd alvorens de lijst van gewenste personen wordt toegelaten.

1. Klikken **IP-bereik toevoegen,** Geef vervolgens het IP-adres of het IP-bereik op van de IP-adressen waartoe u Workfront wilt kunnen openen.
1. (Optioneel) Herhaal de vorige stap om extra IP-adressen of IP-adresbereiken toe te voegen.

   U kunt maximaal 45 adressen of bereiken toevoegen.

1. Klikken **Opslaan.**
