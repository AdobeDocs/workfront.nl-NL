---
user-type: administrator
product-area: system-administration;setup
navigation-topic: start-with-workfront-administration
title: Uw e-maillijst van gewenste personen configureren
description: Als uw organisatie het WorkfrontEnterprise-plan gebruikt, kunt u een Workfront-lijst van gewenste personen voor e-mail maken om te bepalen welke e-maildomeinen e-mails van Workfront mogen accepteren en welke e-maildomeinen zich kunnen bevinden in het e-mailadres dat gebruikers in hun gebruikersprofiel opgeven. Dit is handig als het beveiligingsbeleid van uw organisatie gebruikers beperkt in het verzenden van gegevens die in Workfront zijn opgeslagen naar externe e-mailadressen. U kunt alleen uw interne bedrijfsdomeinen in de lijst van gewenste personen opnemen om ervoor te zorgen dat dit beleid wordt gevolgd.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 76b6acc4-c432-47b4-90bf-6e37e970625f
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '510'
ht-degree: 0%

---

# Uw e-maillijst van gewenste personen configureren

Als uw organisatie het WorkfrontEnterprise-plan gebruikt, kunt u een Workfront-lijst van gewenste personen voor e-mail maken om het volgende te beheren:

* Welke e-maildomeinen mogen e-mails van Workfront accepteren.
* Welke e-maildomeinen kunnen in het e-mailadres zijn dat de gebruikers in hun gebruikersprofiel specificeren.

Dit is handig als het beveiligingsbeleid van uw organisatie gebruikers beperkt in het verzenden van gegevens die in Workfront zijn opgeslagen naar externe e-mailadressen. U kunt alleen uw interne bedrijfsdomeinen in de lijst van gewenste personen opnemen om ervoor te zorgen dat dit beleid wordt gevolgd.

>[!IMPORTANT]
>
>Uw IT-team moet ervoor zorgen dat inkomende e-mail van `notifications@my.workfront.com` wordt niet geblokkeerd in het systeem van uw organisatie.
>
>Alle e-mailberichten van Workfront worden vanaf dat adres verzonden om een betere e-maillevering mogelijk te maken en spoofing van e-mails te voorkomen. Dit omvat zowel geautomatiseerde alarm als gebruiker-aan-gebruiker mededeling.
>
>Zo ziet de From-regel in een Workfront-e-mail die u ontvangt van een gebruiker met de naam Joan Harris er als volgt uit:
>
```
>Joan Harris <notifications@my.workfront.com>
>```

Voor informatie over het configureren van de firewall van uw organisatie om de communicatie tussen uw omgeving en de Adobe Workfront-servers te openen, raadpleegt u [De lijst van gewenste personen van uw firewall configureren](../../administration-and-setup/get-started-wf-administration/configure-your-firewall.md).

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
   <td> <p>U moet een Workfront-beheerder zijn. Zie voor meer informatie <a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Volledige administratieve toegang verlenen aan een gebruiker</a>.</p> <p><b>OPMERKING</b>: Als u nog steeds geen toegang hebt, vraagt u de Workfront-beheerder of deze aanvullende beperkingen op uw toegangsniveau instelt. Voor informatie over hoe een beheerder van Workfront uw toegangsniveau kan wijzigen, zie <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Aangepaste toegangsniveaus maken of wijzigen</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Overige lijsten van gewenste personen

Als uw organisatie het plan van de Onderneming heeft, kunt u een lijst van gewenste personen vormen van Adobe Workfront IP die toegang tot Workfront tot 45 IP adressen of IP adreswaaiers beperkt die u specificeert. Dit biedt een extra beveiligingslaag voor de Workfront-toepassing. Zie voor meer informatie [Toegang tot Adobe Workfront beperken tot IP-adres](../../administration-and-setup/manage-workfront/security/restrict-access-workfront-ip-address.md).

Ook, als uw firewall of postserver wordt gevormd om toegang tot slechts bepaalde verkopers toe te staan, moet u bepaalde IP adressen aan zijn lijst van gewenste personen toevoegen. Hierdoor wordt de communicatie tussen uw omgeving en de Adobe Workfront-servers geopend. Zie voor meer informatie hierover [De lijst van gewenste personen van uw firewall configureren](../../administration-and-setup/get-started-wf-administration/configure-your-firewall.md).

## Uw e-maillijst van gewenste personen configureren

1. Klik op de knop **Hoofdmenu** pictogram ![](assets/main-menu-icon.png) in de rechterbovenhoek van Adobe Workfront klikt u op **Instellen** ![](assets/gear-icon-settings.png).

1. Klikken **Systeem** > **Klantgegevens**.

1. In de **E-mailLijst van gewenste personen** sectie, selecteert u **DomeinLijst van gewenste personen inschakelen** en klik vervolgens op **Domein toevoegen**.
1. Typ in het vak dat wordt weergegeven een domein dat u wilt toestaan, zoals `ourcompany.com`en klik vervolgens op **Domein toevoegen**.

1. Herhaal de vorige stap om andere domeinen toe te voegen die u wilt toestaan.
1. Als u klaar bent, klikt u op **Opslaan**.
