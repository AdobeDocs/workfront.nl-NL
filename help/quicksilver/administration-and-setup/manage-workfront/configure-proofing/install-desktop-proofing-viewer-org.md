---
user-type: administrator
product-area: system-administration;documents
navigation-topic: configure-proofing-functionality
title: Installeer de Desktop Proofing Viewer voor uw organisatie
description: De Desktop Proofing Viewer, die voornamelijk is ontworpen voor het controleren van interactieve inhoud, is een toepassing die op de lokale computer van elke gebruiker moet worden geïnstalleerd. Als Adobe Workfront-beheerder of Workfront Proof-beheerder kunt u deze installatie uitvoeren.
author: Courtney
feature: System Setup and Administration, Digital Content and Documents
role: Admin
exl-id: c89b21c6-fe70-4f46-aebd-5b82a667db72
source-git-commit: 5cc1acffff12d78e48228f3ae223514c0ff379ef
workflow-type: tm+mt
source-wordcount: '558'
ht-degree: 0%

---

# Installeer de Desktop Proofing Viewer voor uw organisatie

<!--Audited: 05/2024-->

De Desktop Proofing Viewer, die voornamelijk is ontworpen voor het controleren van interactieve inhoud, is een toepassing die op de lokale computer van elke gebruiker moet worden geïnstalleerd. Als Adobe Workfront-beheerder of Workfront Proof-beheerder kunt u deze installatie uitvoeren.

## Toegangsvereisten

U moet de volgende toegang hebben om de stappen in dit artikel uit te voeren:

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-plan</td> 
   <td> <p>Huidig abonnement: Pro of hoger</p> <p>of</p> <p>Ouder abonnement: Premium of Selecteren</p> <p>Voor meer informatie over het proefdrukken van toegang met de verschillende plannen, zie <a href="../../../administration-and-setup/manage-workfront/configure-proofing/access-to-proofing-functionality.md" class="MCXref xref">Toegang tot proefdrukfunctionaliteit in Workfront</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-licentie</td> 
   <td> <p>Huidig plan: Werk of Plan</p> <p>Ouder plan: Willekeurig (proefdrukken moet zijn ingeschakeld voor de gebruiker)</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraties op toegangsniveau</td> 
   <td> <p>Beheerder moet zijn geselecteerd in het machtigingsprofiel voor proefdrukken. Zie voor meer informatie <a href="../../../administration-and-setup/manage-workfront/configure-proofing/configure-a-users-proofing-access.md" class="MCXref xref">De proefdruktoegang van een gebruiker configureren</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

Zie voor meer informatie over de informatie in deze tabel [Toegangsvereisten in Workfront-documentatie](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

## Systeemvereisten

De Desktop Proofing Viewer wordt ondersteund op de volgende besturingssystemen:

* Windows 7 en hoger, 32 en 64 bits
* Mac OS X 10.9 en hoger, 64-bits

## Vereisten

Om gebruikers in staat te stellen de Desktop Proofing Viewer te gebruiken, moet u het systeem configureren om de Desktop Proofing Viewer te starten als de standaardweergave voor interactieve proefdrukken voordat u de toepassing installeert.

## De Desktop Proofing Viewer configureren als standaard voor interactieve proefdrukken

Nadat u de Desktop Proofing Viewer voor uw organisatie hebt geïnstalleerd, kunt u deze instellen als de standaardviewer voor interactieve proefdrukken.

{{step1-to-proofing}}

1. Klikken **Accountinstellingen** in de rechterbovenhoek van Workfront Proof klikt u op de knop **Instellingen** tab.

1. Onder **Standaardwaarden proefdrukken** aan het einde van de **Desktop Proofing Viewer voor interactieve proefdrukken** rij, klik **Instellen**.

   ![Standaardwaarden proefdrukken](assets/proof-defaults.png)

1. Klikken **Ingeschakeld en standaard** en klik vervolgens op **Opslaan**.

## De Desktop Proofing Viewer installeren voor uw gebruikers

* [De Desktop Proofing Viewer installeren op Mac](#installing-the-desktop-proofing-viewer-on-mac)
* [De Desktop Proofing Viewer installeren in Windows](#installing-the-desktop-proofing-viewer-on-windows)

### De Desktop Proofing Viewer installeren op Mac {#installing-the-desktop-proofing-viewer-on-mac}

1. Voer op de computer van de gebruiker een van de volgende handelingen uit om de app te downloaden:

   * Als u de productieomgeving gebruikt, klikt u op [Mac Production Download voor de Desktop Proofing Viewer](https://assets.proofhq.com/nativeviewer/desktop_viewer/Workfront+Proof-2.1.19.pkg).
   * Als u de voorvertoningsomgeving gebruikt, klikt u op [Mac Preview Download voor de Desktop Proofing Viewer](https://assets.preview.proofhq.com/nativeviewer/desktop_viewer/Workfront+Proof+Preview-2.1.19.pkg).

1. Open het bestand dat u zojuist hebt gedownload om de installatie te starten.
1. Klik in het installatievak dat verschijnt op **Doorgaan** en klik vervolgens op **Installeren**.

   ![Installatievak](assets/install-wf-proof-box.png)

1. Zorg ervoor dat elke gebruiker de installatie voltooit door een interactieve proefdruk te openen vanuit het gebied Documenten in Workfront.

### De Desktop Proofing Viewer installeren in Windows {#installing-the-desktop-proofing-viewer-on-windows}

1. Voer op de computer van de gebruiker een van de volgende handelingen uit om de app te downloaden:

   * Klik in de productieomgeving op [Downloaden van Windows Productie voor de Desktop Proofing Viewer](https://assets.proofhq.com/nativeviewer/desktop_viewer/Workfront+Proof+Setup+2.1.19.exe).
   * Klik in de voorvertoningsomgeving op [Windows Preview-download voor de Desktop Proofing Viewer](https://assets.preview.proofhq.com/nativeviewer/desktop_viewer/Workfront+Proof+Preview+Setup+2.1.19.exe).

1. Open het bestand dat u zojuist hebt gedownload om de installatie te starten.
1. Klik in het beveiligingswaarschuwingsvenster dat wordt weergegeven op **Uitvoeren**.

   ![Screen_Shot_2018-05-02_at_10.56.55_AM.png](assets/screen-shot-2018-05-02-at-10.56.55-am-350x271.png)

   De Desktop Proofing Viewer wordt geïnstalleerd en uitgevoerd.

1. (Voorwaardelijk) Als u de toepassing installeert met Internet Explorer, vernieuwt u de startpagina in de browser nadat de toepassing is geïnstalleerd.
1. Zorg ervoor dat elke gebruiker de installatie voltooit door een interactieve proefdruk te openen vanuit het gebied Documenten in Workfront.
