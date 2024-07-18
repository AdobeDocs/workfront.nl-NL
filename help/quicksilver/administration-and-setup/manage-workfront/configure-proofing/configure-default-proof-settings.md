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

## Nieuwe standaardproefinstellingen configureren

1. Klik het **Belangrijkste pictogram van het Menu** ![](assets/main-menu-icon.png) in de hoger-juiste hoek van Adobe Workfront, dan klik **Opstelling**.
1. In het linkerpaneel, klik **Proefdrukken** > **montages van het Bewijs**.
1. In de **Nieuwe proefdrukgebreken** sectie, vorm de volgende montages:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader" colspan="2"><b>Ontvangers</b></td> 
     </tr> 
     <tr> 
      <td role="rowheader">Aanmelding vereisen</td> 
      <td> <p>Revisoren moeten zich met hun e-mail en wachtwoord aanmelden voordat ze de proefdrukken kunnen bekijken die in de account van uw organisatie zijn gemaakt. Als deze optie is ingeschakeld, kunnen gebruikers de proefdruk niet delen met gastrevisoren.</p> <p><b> BELANGRIJK </b>: Wanneer toegelaten, login wordt vereist voor alle pas gecreëerde proefdrukken.</p> </td> 
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
      <td> <p>Besluitvormers wordt gevraagd hun aanmeldingsgegevens voor Workfront in te voeren wanneer zij een besluit nemen over een bewijs.</p> <p><b> BELANGRIJK </b>: Wanneer toegelaten, kunnen de gebruikers niet het bewijs met de recensenten van de Gast delen die login geloofsbrieven niet hebben.</p> </td> 
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

1. Klik **sparen**.

## Proofingbeslissingen configureren

Gebruikers kunnen de status van het bewijs na controle aangeven aan de hand van proefdrukbesluiten.

>[!NOTE]
>
>De logica achter proefdrukbesluiten wordt gebruikt om de algemene status van een proefwerkschema te berekenen als er veelvoudige besluiten van diverse niveaus zijn. De besluiten &quot;Goedgekeurd&quot;en &quot;Goedgekeurd met veranderingen&quot;brengen de volgende fase in een automatisch werkschema teweeg.

Om proefdrukbesluiten te vormen:

1. Klik het **Belangrijkste pictogram van het Menu** ![](assets/main-menu-icon.png) in de hoger-juiste hoek van Adobe Workfront, dan klik **Opstelling**.
1. In het linkerpaneel, klik **Proefdrukken** > **montages van het Bewijs**.
1. In de **sectie van Besluiten**, kunt u

   1. **noem het besluit** anders: Klik op de tekst binnen de besluitvormingsdoos, en begin typend het nieuwe besluitvormingsetiket.

      >[!TIP]
      >
      >Behoud de logica voor een besluit wanneer u het anders noemt. Bijvoorbeeld, kon het afgewezen standaardbesluit in *Nieuwe vereiste versie* worden veranderd, maar het zou niet moeten worden veranderd in *verzenden naar Printers*.

      ![](assets/rename-decision-350x109.png)

   1. **herschikt de besluitvormingsorde**: Sleep de besluitvormingsvakjes in de orde u hen in de het proef kijker wilt verschijnen.

      ![](assets/move-decision-350x110.png)

   1. **verberg een besluit**: Beweeg over de besluitvormingsdoos, en klik het pictogram van de Huid in de hoger-juiste hoek.

      ![](assets/hide-decision-350x109.png)

1. (Facultatief) om terug naar de gebreken van Workfront te gaan, klik **herstellen gebreken**.
1. Klik **sparen**.
