---
user-type: administrator
product-area: system-administration;projects
navigation-topic: configure-system-defaults
title: Adobe Enterprise-opslag inschakelen voor uw organisatie
description: U kunt Adobe Enterprise-opslag voor uw organisatie inschakelen om een uniforme opslagoplossing te gebruiken voor alle Adobe-producten.
author: Courtney
feature: System Setup and Administration
role: Admin
exl-id: 48b581c7-a21a-45de-95c5-eafb0713b42e
last-update: 2026-04-01T18:03:50Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
source-git-commit: 18301970abddd8ed98abccf42562d950422bfa7c
workflow-type: tm+mt
source-wordcount: '320'
ht-degree: 0%

---

# Adobe Enterprise-opslag voor uw organisatie inschakelen

Adobe Enterprise Storage is een centrale opslagoplossing voor alle Adobe-producten. Het is een op cloud gebaseerde opslagoplossing die fungeert als centrale opslagplaats voor bedrijfsmiddelen in Adobe.

Adobe Enterprise storage is standaard ingeschakeld voor nieuwe klanten en kan voor bestaande klanten worden ingeschakeld bij contractvernieuwing.

Voor meer informatie over de ondernemingsopslag van Adobe, zie [&#x200B; overzicht van de ondernemingsopslag van Adobe &#x200B;](/help/quicksilver/review-and-approve-work/esm-overview.md).

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

## Adobe Enterprise-opslag voor uw organisatie inschakelen

Adobe Enterprise-opslag voor uw organisatie inschakelen:

{{step-1-to-setup}}

1. Selecteer **Systeem** in de linkernavigatie, dan selecteren **Voorkeur**.
1. De rol neer aan de **voorkeur van de Opslag** sectie.
1. In het Standaard drop-down menu, uitgezochte **de ondernemingsopslag van Adobe**.
1. (Facultatief) als u een combinatie van de ondernemingsopslag van Adobe en de Verouderde Opslag van Workfront wilt gebruiken, selecteer **toestaan gebruiker om opslagleverancier** checkbox te selecteren.

   >[!NOTE]
   >
   >Als u deze optie inschakelt, kunnen gebruikers de opslagprovider selecteren wanneer ze een nieuw project maken. de opslag van de onderneming wordt geëtiketteerd als &quot;Nieuw project&quot;aangezien het de standaardopslagleverancier is. Legacy Workfront Storage heet &quot;Legacy project&quot;.
   >
   >![&#x200B; nieuw project en erfenisprojectopties &#x200B;](assets/new-esm-project.png)

1. Kies een van de volgende opties in het vervolgkeuzemenu Toepassen op:

   - **Volledige organisatie**: Deze optie past de standaard opslagleverancier op uw volledig milieu van Workfront toe. Telkens wanneer een gebruiker een nieuw project maakt, wordt de standaard opslagprovider gebruikt.
   - **Specifieke groepen**: Deze optie past de standaardopslagleverancier slechts op specifieke groepen binnen uw organisatie toe. Wanneer een gebruiker in de opgegeven groepen een nieuw project maakt, wordt de standaardopslagprovider gebruikt

1. Klik **sparen**.
