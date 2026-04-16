---
user-type: administrator
product-area: system-administration;setup
title: Aangepaste lokalisatie configureren
description: Met aangepaste lokalisatie kunt u aangepaste termen en woordgroepen definiëren in verschillende talen. Workfront geeft deze termen vervolgens weer in de taal die is ingesteld in de browserinstellingen.
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: bdc6d5ee-2037-4d0b-bf18-3e6cc9cb078e
source-git-commit: 28178c3794832e14552d988259c1792a6fed1da1
workflow-type: tm+mt
source-wordcount: '386'
ht-degree: 1%

---

# Aangepaste lokalisatie configureren

Met aangepaste lokalisatie kunt u aangepaste termen en woordgroepen definiëren in verschillende talen. Workfront geeft deze termen vervolgens weer in de taal die is ingesteld in de Adobe Identity Management (IMS)-instellingen van de gebruiker. Als de gebruiker zich niet op Adobe IMS bevindt, worden de termen weergegeven in de taalset in de browserinstellingen van de gebruiker.

U kunt bijvoorbeeld het label &#39;Doelpubliek&#39; instellen om het Duitse woord &#39;Zielgruppe&#39; te vertalen. Elke gebruiker met Duits als hoofdtaal van zijn browser geselecteerd ziet het woord &quot;Zielgruppe&quot; als een label voor alle velden met het label &quot;Doelpubliek&quot; in het Engels.

U kunt vertalingen in meerdere talen configureren. Tot de huidige beschikbare talen behoren:

* Chinees (traditioneel)
* Chinees (vereenvoudigd)
* Frans
* Duits
* Italiaans
* Japans
* Koreaans
* Portugees (Brazilië)
* Spaans

## Toegangsvereisten

+++ Breid uit om de toegangseisen voor de functionaliteit in dit artikel weer te geven.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-pakket</td> 
   <td> <p>Workflow Prime of hoger </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-licentie</td> 
   <td> <p>Standard</p>
    </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraties op toegangsniveau</td> 
   <td> <p>U moet een Workfront-beheerder zijn om vertalingen te configureren.</p>  </td> 
  </tr>
 </tbody> 
</table>

Voor informatie, zie [&#x200B; vereisten van de Toegang in de documentatie van Workfront &#x200B;](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Overwegingen bij het instellen van lokalisatie

Houd rekening met het volgende wanneer u lokalisatie configureert:

* U kunt een termijn vormen om in veelvoudige talen te vertalen.
* Lokalisatie is van toepassing op aangepaste veldlabels (inclusief als kolomkop) en knopinfo.
* De localisatie van de douane kan op berichten van BedrijfsRegels van toepassing zijn, maar moet in de BedrijfsRegel worden toegelaten.

  Voor instructies, zie [&#x200B; localisatie in een BedrijfsRegel &#x200B;](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/business-rules.md#using-custom-localization-with-business-rules) in artikel toelaten en bedrijfsregels uitgeven.

## Vertalingen configureren

De vertalingen worden gevormd in het gebied van de Opstelling.

1. Klik het **[!UICONTROL Main Menu]** pictogram ![&#x200B; Belangrijkste Menu &#x200B;](/help/_includes/assets/main-menu-icon.png) in de hoger-juiste hoek van Adobe Workfront, of (als beschikbaar), klik het **[!UICONTROL Main Menu]** pictogram ![&#x200B; Belangrijkste Menu &#x200B;](/help/_includes/assets/main-menu-icon-left-nav.png) in de upper-left hoek, dan klik **[!UICONTROL Setup]** ![&#x200B; pictogram van de Opstelling &#x200B;](/help/_includes/assets/gear-icon-setup.png).
1. In het gebied van de Opstelling, klik **Localization** in het linkernavigatievenster.
1. Om een nieuwe vertaling toe te voegen, klik **Nieuwe rij**.
1. In de **Engelse** kolom, ga de Engelse termijn in die zou moeten worden vertaald.
1. In de kolom voor de taal die u de termijn wilt worden vertaald, ga de termijn in de doeltaal in.
1. Als u het woord in extra talen wilt vertalen, voegt u de vertaling toe aan de desbetreffende taalkolom.
1. Als u de volgorde van taalkolommen wilt wijzigen, klikt u op de kop van een kolom die u wilt verplaatsen en sleept u deze naar de gewenste locatie.
