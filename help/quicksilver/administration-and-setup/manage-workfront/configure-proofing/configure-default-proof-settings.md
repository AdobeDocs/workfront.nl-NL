---
user-type: administrator
product-area: system-administration;setup
navigation-topic: configure-proofing-functionality
title: Standaardproefdrukinstellingen configureren
description: Met deze instellingen kunt u standaardwaarden instellen die van toepassing zijn op alle nieuwe proefdrukken die door uw gebruikers worden gemaakt. Gebruikers kunnen de meeste van deze instellingen echter overschrijven bij het maken van een proefdruk.
author: Courtney
feature: System Setup and Administration, Digital Content and Documents
role: Admin
exl-id: cfccb120-8759-49f2-8b7b-dabcd57d4fda
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '513'
ht-degree: 0%

---

# Standaardproefdrukinstellingen configureren

Met deze instellingen kunt u standaardwaarden instellen die van toepassing zijn op alle nieuwe proefdrukken die door uw gebruikers worden gemaakt. Gebruikers kunnen de meeste van deze instellingen echter overschrijven bij het maken van een proefdruk.

## Nieuwe standaardinstellingen voor proefdrukken configureren

1. Klik op de knop **Hoofdmenu** pictogram ![](assets/main-menu-icon.png) in de rechterbovenhoek van Adobe Workfront klikt u op **Instellen**.
1. Klik in het linkerdeelvenster op **Proefdrukken** > **Proefinstellingen**.
1. In de **Nieuwe standaardwaarden voor proefdrukken** de volgende instellingen configureren:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader" colspan="2"><b>Ontvangers</b></td> 
     </tr> 
     <tr> 
      <td role="rowheader">Aanmelding vereisen</td> 
      <td> <p>Revisoren moeten zich met hun e-mail en wachtwoord aanmelden voordat ze de proefdrukken kunnen bekijken die in de account van uw organisatie zijn gemaakt. Als deze optie is ingeschakeld, kunnen gebruikers de proefdruk niet delen met gastrevisoren.</p> <p><b>BELANGRIJK</b>: Als deze optie is ingeschakeld, moet u zich aanmelden voor alle nieuwe proefdrukken.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Eigenaar kopiëren uit oorspronkelijke proefversie voor nieuwe versies</td> 
      <td> <p>De eigenaar van de eerste versie van een proefdruk is ook de eigenaar van alle opeenvolgende versies van de proefdruk, ongeacht wie deze versies maakt. Deze instelling is standaard ingeschakeld.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Gebruikers toestaan hun proefdrukopmerkingen te verwijderen</td> 
      <td>Gebruikers kunnen hun eigen opmerkingen verwijderen. Deze instelling is standaard ingeschakeld.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Vereisen dat besluiten elektronisch worden ondertekend </td> 
      <td> <p>Besluitvormers wordt gevraagd hun aanmeldingsgegevens voor Workfront in te voeren wanneer zij een besluit nemen over een bewijs.</p> <p><b>BELANGRIJK</b>: Als deze optie is ingeschakeld, kunnen gebruikers de proefdruk niet delen met gastrevisoren die geen aanmeldingsgegevens hebben.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader" colspan="2"><b>Deadline</b></td> 
     </tr> 
     <tr> 
      <td role="rowheader">De standaarddeadline instellen</td> 
      <td> <p>Het systeem past deze deadline toe op alle nieuwe proefdrukken in uw account die geen automatische workflow hebben.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Ontvangers op de hoogte stellen voordat het bewijs gevaar loopt</td> 
      <td>Ontvangers worden via e-mail op de hoogte gebracht voordat het bewijs als riskant wordt beschouwd, afhankelijk van de hierboven vermelde termijn.</td> 
     </tr> 
     <tr> 
      <td role="rowheader" colspan="2"><b>E-mailmeldingen</b></td> 
     </tr> 
     <tr> 
      <td role="rowheader">Ontvangers op de hoogte stellen wanneer ze aan een bewijs worden toegevoegd</td> 
      <td>Ontvangers worden via e-mail op de hoogte gesteld wanneer ze aan een bewijs worden toegevoegd.</td> 
     </tr> 
    </tbody> 
   </table>

1. Klikken **Opslaan**.

## Proofingbeslissingen configureren

Gebruikers kunnen de status van het bewijs na controle aangeven aan de hand van proefdrukbesluiten.

>[!NOTE]
>
>De logica achter proefdrukbesluiten wordt gebruikt om de algemene status van een proefwerkschema te berekenen als er veelvoudige besluiten van diverse niveaus zijn. De besluiten &quot;Goedgekeurd&quot;en &quot;Goedgekeurd met veranderingen&quot;brengen de volgende fase in een automatisch werkschema teweeg.

Om proefdrukbesluiten te vormen:

1. Klik op de knop **Hoofdmenu** pictogram ![](assets/main-menu-icon.png) in de rechterbovenhoek van Adobe Workfront klikt u op **Instellen**.
1. Klik in het linkerdeelvenster op **Proefdrukken** > **Proefinstellingen**.
1. In de **Besluiten** sectie, kunt u

   1. **Naam van de beslissing wijzigen**: Klik op de tekst in het beslissingsvak en typ het nieuwe beslissingslabel.

      >[!TIP]
      >
      >Behoud de logica voor een besluit wanneer u het anders noemt. De standaardbeslissing Afgewezen kan bijvoorbeeld worden gewijzigd in *Nieuwe versie vereist*, maar het mag niet worden gewijzigd in *Naar printers verzenden*.

      ![](assets/rename-decision-350x109.png)

   1. **De beslissingsvolgorde wijzigen**: Sleep de beslissingsvakken in de volgorde waarin u ze wilt weergeven in de proefdrukviewer.

      ![](assets/move-decision-350x110.png)

   1. **Een beslissing verbergen**: Houd de cursor boven het beslissingsvak en klik op het pictogram Verbergen in de rechterbovenhoek.

      ![](assets/hide-decision-350x109.png)

1. (Optioneel) Klik op **Standaardinstellingen herstellen**.
1. Klikken **Opslaan**.
