---
user-type: administrator
product-area: system-administration;setup
navigation-topic: start-with-workfront-administration
title: Uw e-mailLijst van gewenste personen configureren
description: Als uw organisatie het WorkfrontEnterprise-plan gebruikt, kunt u een Workfront-lijst van gewenste personen voor e-mail maken om te bepalen welke e-maildomeinen e-mails van Workfront mogen accepteren en welke e-maildomeinen zich kunnen bevinden in het e-mailadres dat gebruikers in hun gebruikersprofiel opgeven. Dit is handig als het beveiligingsbeleid van uw organisatie gebruikers beperkt in het verzenden van gegevens die in Workfront zijn opgeslagen naar externe e-mailadressen. U kunt alleen uw interne bedrijfsdomeinen in de lijst van gewenste personen opnemen om ervoor te zorgen dat dit beleid wordt gevolgd.
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: 76b6acc4-c432-47b4-90bf-6e37e970625f
source-git-commit: 15ea03bf586054f7ef421f8cacede6f42835a6e4
workflow-type: tm+mt
source-wordcount: '399'
ht-degree: 0%

---

# Uw e-maillijst van gewenste personen configureren

Als uw organisatie het Workfront Enterprise-plan gebruikt, kunt u een Workfront e-maillijst van gewenste personen maken om het volgende te beheren:

* Welke e-maildomeinen mogen e-mails van Workfront accepteren.
* Welke e-maildomeinen kunnen in het e-mailadres zijn dat de gebruikers in hun gebruikersprofiel specificeren.

Dit is handig als het beveiligingsbeleid van uw organisatie gebruikers beperkt in het verzenden van gegevens die in Workfront zijn opgeslagen naar externe e-mailadressen. U kunt alleen uw interne bedrijfsdomeinen in de lijst van gewenste personen opnemen om ervoor te zorgen dat dit beleid wordt gevolgd.

>[!IMPORTANT]
>
>Uw IT-team moet ervoor zorgen dat inkomende e-mail van `notifications@my.workfront.com` niet wordt geblokkeerd in het systeem van uw organisatie.
>
>Alle e-mailberichten van Workfront worden vanaf dat adres verzonden om een betere e-maillevering mogelijk te maken en spoofing van e-mails te voorkomen. Dit omvat zowel geautomatiseerde alarm als gebruiker-aan-gebruiker mededeling.
>
>Zo ziet de From-regel in een Workfront-e-mail die u ontvangt van een gebruiker met de naam Joan Harris er als volgt uit:
>&#x200B;>`Joan Harris <notifications@my.workfront.com>`

Voor informatie over het vormen van de firewall van uw organisatie om communicatie tussen uw milieu en de servers van Adobe Workfront te openen, zie [&#x200B; de lijst van gewenste personen van uw firewall &#x200B;](../../administration-and-setup/get-started-wf-administration/configure-your-firewall.md) vormen.

## Toegangsvereisten

+++ Breid uit om de toegangseisen voor de functionaliteit in dit artikel weer te geven.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Workfront-pakket</td> 
   <td><p>Alle</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-licentie</td> 
   <td><p>Standard</p> <p>Plan</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraties op toegangsniveau</td> 
   <td>U moet een Workfront-beheerder zijn. </td> 
  </tr> 
 </tbody> 
</table>

Voor informatie, zie [&#x200B; vereisten van de Toegang in de documentatie van Workfront &#x200B;](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Overige lijsten van gewenste personen

Als uw firewall of postserver wordt gevormd om toegang tot slechts bepaalde verkopers toe te staan, moet u bepaalde IP adressen aan zijn lijst van gewenste personen toevoegen. Hierdoor wordt de communicatie tussen uw omgeving en de Adobe Workfront-servers geopend. Voor informatie over dat, zie [&#x200B; de lijst van gewenste personen van uw firewall &#x200B;](../../administration-and-setup/get-started-wf-administration/configure-your-firewall.md) vormen.

## Uw e-maillijst van gewenste personen configureren

{{step-1-to-setup}}

1. Klik **Systeem** > **Info van de Klant**.
1. In de **E-mail Lijst van gewenste personen** sectie, uitgezochte **laat de Lijst van gewenste personen van het Domein** toe, dan klik **voegt Domein** toe.
1. In de doos die toont, typ een domein dat u, zoals `ourcompany.com` wilt toestaan, dan **klikken voegt Domein** toe.
1. Herhaal de vorige stap om andere domeinen toe te voegen die u wilt toestaan.
1. Wanneer u wordt gebeëindigd, klik **sparen**.
