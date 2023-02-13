---
title: Ondersteuningsbeleid voor AtTask OnPremise
user-type: administrator
content-type: faq
product-area: system-administration
navigation-topic: administrator-faqs
description: Adobe Workfront is overgestapt op een 100% Software-As-A-Service-model en heeft op 31 december 2011 de verkoop van on-premise software stopgezet. Vanaf 2014 wordt AtTask OnPremise niet meer ondersteund, met uitzondering van problemen met licentiesleutels. De toepassing op locatie kan niet meer worden gedownload of geïnstalleerd.
feature: System Setup and Administration
role: Admin
exl-id: 37c65360-6587-43b3-8eaf-4f1a9b375c1d
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '247'
ht-degree: 0%

---

# Ondersteuningsbeleid voor AtTask OnPremise

Adobe Workfront is overgestapt op een 100% Software-As-A-Service-model en heeft op 31 december 2011 de verkoop van on-premise software stopgezet. Vanaf 2014 wordt AtTask OnPremise niet meer ondersteund, met uitzondering van problemen met licentiesleutels. De toepassing op locatie kan niet meer worden gedownload of geïnstalleerd.

Download de installatiehandleiding als u de toepassing al hebt en OnPremise opnieuw moet installeren.

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">OnPremise optimization tips can be found.</p>
-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">To learn more about reporting in AtTask OnPremise, click.</p>
-->

Download instructies over SSL/TSL-installatie.

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

## De OnPremise-licentiecode bijwerken

Als u een nieuwe licentiecode nodig hebt, belt u de Workfront-klantenondersteuning op 844-306-HELP(4357).

Nadat u een nieuwe licentiecode hebt gekregen,

1. Stop de atTask-server.
1. Wijzig de naam van het huidige bestand license.key (in de map AtTaskDoc).
1. Kopieer het nieuwe bestand license.key naar zijn plaats.
1. Start de atTask-server opnieuw.

Dit artikel bevat de volgende bijlagen:
