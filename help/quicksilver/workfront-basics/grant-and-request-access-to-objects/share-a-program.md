---
title: Een programma delen
product-area: projects
keywords: delen,programma,machtigingen
navigation-topic: grant-and-request-access-to-objects
description: Uw Adobe Workfront-beheerder kan u toegang verlenen tot weergave- of bewerkingsprogramma's wanneer u uw toegangsniveau toewijst. U moet een licentie voor het abonnement hebben om toegang te hebben tot het bewerken van een programma.
author: Courtney
feature: Get Started with Workfront
exl-id: bfa6ce97-24ad-44b3-9c2f-7fac6b748f94
source-git-commit: dbc4404501e20b3f1905a5eebd13734a65db27ae
workflow-type: tm+mt
source-wordcount: '892'
ht-degree: 0%

---

# Een programma delen


Uw Adobe Workfront-beheerder kan u toegang verlenen tot weergave- of bewerkingsprogramma&#39;s wanneer u uw toegangsniveau toewijst. U moet een licentie voor het abonnement hebben om toegang te hebben tot het bewerken van een programma. Voor meer informatie, zie [ toegang van de Verlening tot programma&#39;s ](../../administration-and-setup/add-users/configure-and-grant-access/grant-access-programs.md).

Samen met het toegangsniveau dat u wordt verleend, kunt u toestemmingen ook ontvangen om specifieke programma&#39;s van gebruikers te bekijken of te beheren die hen met u kunnen delen. Voor meer informatie over toegangsniveaus en toestemmingen, zie [ hoe de toegangsniveaus en de toestemmingen samen ](../../administration-and-setup/add-users/access-levels-and-object-permissions/how-access-levels-permissions-work-together.md) werken.

Machtigingen gelden specifiek voor elk item in Workfront en definiëren welke handelingen gebruikers op dat item kunnen uitvoeren.


## Toegangsvereisten

+++ Breid uit om de toegangseisen voor de functionaliteit in dit artikel weer te geven. 

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-pakket</td> 
   <td> <p>Alle</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-licentie</td> 
   <td> <p>Standard</p> 
   <p>Werk of hoger</p> 
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraties op toegangsniveau</td> 
   <td> <p>Toegang tot of hoger weergeven voor de objecten die u wilt delen</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objectmachtigingen</td> 
   <td> <p>Machtigingen of hoger weergeven voor de objecten die u wilt delen</p></td> 
  </tr> 
 </tbody> 
</table>

Voor meer detail over de informatie in deze lijst, zie [ vereisten van de Toegang in de documentatie van Workfront ](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Overwegingen bij het delen van een programma

Naast de overwegingen hieronder, zie ook [ Overzicht van het delen van toestemmingen op voorwerpen ](../../workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md).

>[!NOTE]
>
>Een Workfront-beheerder kan machtigingen toevoegen of verwijderen voor alle items in het systeem, zonder de eigenaar van die items te zijn.

* De maker van een programma beschikt standaard over de machtiging Beheren.

* U kunt programma&#39;s afzonderlijk delen, maar u kunt ook verschillende programma&#39;s tegelijk delen.

  Voor meer informatie over het delen van punten in Workfront, zie [ een voorwerp ](../../workfront-basics/grant-and-request-access-to-objects/share-an-object.md) delen.

* U kunt alleen weergavemachtigingen of beheermachtigingen verlenen voor programma&#39;s:

* Wanneer u een programma deelt, erven de gebruikers de zelfde toestemmingen aan alle kindvoorwerpen verbonden aan het programma, door gebrek.

  Voor meer informatie over de hiërarchie van voorwerpen in Workfront, zie [ voorwerpen in Adobe Workfront ](../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md) begrijpen.

* U kunt overgeërfde machtigingen uit het programma verwijderen. Zie voor meer informatie over het verwijderen van machtigingen uit objecten   [ verwijdert toestemmingen uit voorwerpen ](../../workfront-basics/grant-and-request-access-to-objects/remove-permissions-from-objects.md).

## Een programma delen

{{step1-to-programs}}

1. Voor de **pagina van Programma&#39;s**, selecteer het programma u wilt delen. De programmapagina wordt geopend.

1. Aan het recht van de programmanaam, klik **Aandeel**. Het **de dialoogvakje van de Naam van het Programma van het Aandeel []** opent.

   ![ het programmaknoop van het Aandeel ](assets/share-program-button.png)

1. In de **programmatoegang van de Verlening tot** gebied, begin typend de naam van de gebruiker, het team, de rol, de groep, of het bedrijf u het programma met wilt delen, dan klik de naam wanneer het in de drop-down lijst verschijnt.

   >[!TIP]
   >
   >U kunt een programma alleen delen met actieve gebruikers, teams, rollen of bedrijven.


1. (Facultatief) selecteer **wie toegang** drop-down heeft en het de toegangsniveau van het programma selecteert:

   * **slechts kunnen de uitgenodigde mensen toegang hebben:** slechts de gebruikers die aan het programma worden uitgenodigd kunnen tot het (Gebrek) toegang hebben.
   * **iedereen in het systeem kan** bekijken: Alle gebruikers in het systeem kunnen het programma zonder een uitnodiging bekijken.


1. Klik op de vervolgkeuzelijst rechts van de naam van de gebruiker en selecteer het desbetreffende machtigingsniveau voor dit programma:

   * **Mening**: De gebruiker kan het programma herzien en delen.
   * **leidt**: De gebruiker heeft volledige toegang tot het programma zonder administratieve rechten, die op het toegangsniveau (omvat ook alle toestemmingen van de Mening) worden verleend.

1. (Optioneel) Klik op het pictogram Geavanceerde opties naast het machtigingsniveau dat u hebt toegekend om specifieke machtigingen voor het programma te configureren.

   ![ gevormde geavanceerde toestemmingsopties ](assets/advanced-options-icon.png)

1. (Facultatief) om geërfte toestemmingen voor de kindvoorwerpen van het programma uit te zetten, klik **Draai** gealigneerd met **Geërfde toestemmingen**.

1. (Facultatief) om het programma snel te delen gebruikend een verbinding, klik **verbinding van het Exemplaar** en door:sturen het aan de ontvanger.

1. Klik **sparen**.

## Programma&#39;s bulksgewijs delen

{{step1-to-programs}}

1. Op de **pagina van Programma&#39;s**, selecteer de doos links van elk programma u wilt delen, dan klik het **pictogram van het Aandeel** ![ Aandeel ](assets/share-icon.png) bij de bovenkant van de pagina. Het deelmodaal wordt geopend.

   ![ Bulk deelt programma&#39;s ](assets/bulk-share-programs.png)

1. In de **programmatoegang van de Verlening tot** gebied, begin typend de naam van de gebruiker, het team, de rol, de groep, of het bedrijf u de programma&#39;s met wilt delen, dan klik de naam wanneer het in de drop-down lijst verschijnt.

   >[!TIP]
   >
   >U kunt programma&#39;s met actieve gebruikers, teams, rollen, of bedrijven slechts delen.


1. (Facultatief) selecteer **wie toegang** drop-down heeft en het de toegangsniveau van de programma&#39;s selecteert:

   * **slechts kunnen de uitgenodigde mensen toegang hebben:** slechts de gebruikers die aan de programma&#39;s worden uitgenodigd kunnen tot hen (Gebrek) toegang hebben.
   * **iedereen in het systeem kan** bekijken: Alle gebruikers in het systeem kunnen de programma&#39;s zonder een uitnodiging bekijken.


1. Klik op de vervolgkeuzelijst rechts van de naam van de gebruiker en selecteer het desbetreffende machtigingsniveau voor de programma&#39;s:

   * **Mening**: De gebruiker kan de programma&#39;s herzien en delen.
   * **leidt**: De gebruiker heeft volledige toegang tot de programma&#39;s zonder administratieve rechten, die op het toegangsniveau (omvat ook alle toestemmingen van de Mening) worden verleend.

1. (Optioneel) Klik op het pictogram Geavanceerde opties naast het machtigingsniveau dat u hebt toegekend om specifieke machtigingen voor de programma&#39;s te configureren.

   ![ gevormde geavanceerde toestemmingsopties ](assets/advanced-options-icon.png)

1. Klik **sparen**.

## Programmamachtigingen

In de volgende tabel wordt weergegeven welke machtigingen u gebruikers kunt verlenen wanneer u hen toestaat een programma te bekijken of te beheren:

| **Acties** | **leiden** | **Mening** |
|---|---|---|
| Programmadetails bewerken | ✓ |   |
| Een programma weergeven | ✓ | ✓ |
| Een programma verwijderen | ✓ |   |
| Een aangepast formulier bijvoegen | ✓ |   |
| Een aangepast veld bewerken | ✓ |   |
| Een project toevoegen of verwijderen &#42; | ✓ |   |
| Een project goedkeuren | ✓ |   |
| Een documentmap toevoegen &#42; | ✓ | ✓ |
| Een document toevoegen | ✓ | ✓ |
| Updates/opmerkingen toevoegen | ✓ | ✓ |
| Delen | ✓ | ✓ |
| Delen op het hele systeem |   | ✓ |

*This de toestemmingen worden gecontroleerd door het toegangsniveau en de toestemmingen op andere voorwerpen, zoals projecten.


