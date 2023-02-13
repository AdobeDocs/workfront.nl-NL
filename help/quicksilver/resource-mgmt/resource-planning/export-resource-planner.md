---
product-area: resource-management
navigation-topic: resource-planning
title: Informatie exporteren uit de bronnenplanner
description: U kunt informatie van om het even welke mening van de Planner van het Middel naar een dossier van Excel (.xlsx) uitvoeren dat op uw computer wordt bewaard.
author: Alina
feature: Resource Management
exl-id: 07acd28a-5dc0-45b4-bdf2-20abbd5e098c
source-git-commit: d3172a681ef6ac8b7bde44c680ad7febc3f26121
workflow-type: tm+mt
source-wordcount: '661'
ht-degree: 0%

---

# Informatie exporteren uit de bronnenplanner

U kunt informatie van om het even welke mening van de Planner van het Middel naar een dossier van Excel (.xlsx) uitvoeren dat op uw computer wordt bewaard.

>[!IMPORTANT]
>
>Er gelden beperkingen voor welke informatie wordt weergegeven en welke informatie u kunt exporteren vanuit de functie voor middelenbeheer. Voor informatie over deze beperkingen raadpleegt u [Weergavebeperkingen van de functie Bronnen](../../resource-mgmt/resource-planning/resource-planner-display-limitations.md)

## Toegangsvereisten

U moet het volgende hebben:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-abonnement*</td> 
   <td> <p>Pro en hoger</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-licentie*</td> 
   <td> <p>Controleren of hoger <!--
      <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
       (this seems to be the case in NWE only, not classic. Waiting on Vazgen's response for this)
      </MadCap:conditionalText>
     --></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraties op toegangsniveau*</td> 
   <td> <p>De mening of hogere toegang tot Projecten, Gebruikers, en het Beheer van het Middel</p> <p><b>OPMERKING</b>

Als u nog steeds geen toegang hebt, vraagt u de Workfront-beheerder of deze aanvullende beperkingen op uw toegangsniveau instelt. Voor informatie over hoe een beheerder van Workfront uw toegangsniveau kan veranderen, zie <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Aangepaste toegangsniveaus maken of wijzigen</a>.</p> </td>
</tr> 
  <tr> 
   <td role="rowheader">Objectmachtigingen</td> 
   <td> <p>Toestemmingen of hoger van de mening voor projecten</p> <p>Voor informatie over het aanvragen van aanvullende toegang raadpleegt u <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Toegang tot objecten aanvragen </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Neem contact op met uw Workfront-beheerder om te weten te komen welk plan, licentietype of toegang u hebt.

## Informatie exporteren uit de bronnenplanner

1. Klik op de knop **Hoofdmenu** pictogram ![](assets/main-menu-icon.png) in de rechterbovenhoek van Adobe Workfront.

1. Klikken **Bronnen**. De **Planner** worden standaard weergegeven.

1. Selecteer de weergave voor de Planner. U kunt een van de volgende opties selecteren:

   * Weergeven op gebruiker
   * Weergeven op project
   * Weergeven op rol

1. Klikken **Exporteren**.

   Het dialoogvenster Exportopties wordt weergegeven.

   ![](assets/rp-export-options-box-350x421.png)

1. Geef de volgende informatie op:\
   **Begindatum**: De begindatum van de exportbewerking. Het geëxporteerde bestand bevat informatie over de toewijzing en beschikbaarheid vanaf de eerste dag van de week die de dag bevat die u hier opgeeft.\
   **Aantal perioden**: Het aantal tijdsperioden dat u in het bestand wilt opnemen. De standaardwaarde is 4 punten.\
   **Type**: Het type tijdsperioden waarmee u de informatie in het geëxporteerde bestand wilt weergeven (weken, maanden of kwartalen).\
   Hieronder ziet u de maximale tijdsperioden die u kunt exporteren:

   * 52 weken
   * 36 maanden
   * 12 kwart

   **Selecteren voor exporteren**: Afhankelijk van de weergave die u hebt geselecteerd, kunt u de beschikbaarheid- en budgetinformatie exporteren voor alle objecten die op het scherm worden weergegeven of voor specifieke objecten.
U kunt de volgende gegevens exporteren:

   * Selecteer in de projectweergave om te exporteren:

      * Projecten
      * Projecten en rollen
      * Alles (dit is de standaardoptie)
   * Selecteer in de gebruikersweergave om te exporteren:

      * Gebruikers
      * Gebruikers en projecten
      * Alles (dit is de standaardoptie)
   * Selecteer in de weergave Rol de optie die u wilt exporteren:

      * Rollen
      * Rollen en projecten
      * Alles (dit is de standaardoptie)

   **Gegevensopmaak**: Afhankelijk van hoe u uw dossier van Excel wilt worden getoond, selecteer de volgende opties:

   * **Ruw**: Selecteer deze optie om de beschikbaarheid- en toewijzingsgegevens weer te geven die zijn losgekoppeld van de objecten waartoe deze behoort in het Excel-bestand. (dit is de standaardoptie)
   * **Gegroepeerd**: Selecteer deze optie om de beschikbaarheid- en toewijzingsinformatie weer te geven die is gegroepeerd op de objecten waartoe deze behoort. Hierdoor wordt de geëxporteerde informatie weergegeven zoals deze op het scherm wordt weergegeven.

   In het dialoogvenster Exportopties wordt een voorbeeld weergegeven van de weergave van de informatie in het geëxporteerde bestand.

1. Klikken **Exporteren** om de informatie uit de Planner van het Middel uit te voeren.\
   Alleen de gegevens die u hebt opgeslagen, worden geëxporteerd.

1. (Voorwaardelijk) Als u niet-opgeslagen begrotingsuren hebt in de weergave Rol of Project, klikt u op **Opslaan en doorgaan.**
Er wordt een Excel-bestand (.xlsx) gedownload naar de computer.
\
   Exporteren vanuit de functie Bronnen is niet beschikbaar terwijl het bestand is voorbereid voor downloaden.\
   (Voorwaardelijk) Als u een grote hoeveelheid gegevens exporteert, ontvangt u een e-mail met een koppeling waarmee u het bestand kunt downloaden.\
   ![RP_eamil_with_exporting_planner_attached.png](assets/rp-eamil-with-exported-planner-attached-350x116.png)

1. (Voorwaardelijk) Wanneer u het e-mailbericht ontvangt met het geëxporteerde bestand, klikt u op **Downloaden** om het bestand te downloaden.\
   Hiermee gaat u terug naar Workfront waar u het bestand kunt downloaden.\
   Het downloaden kan alleen worden voltooid als u bent aangemeld bij Workfront.\
   Als u het bestand niet downloadt wanneer het wordt geleverd, blijft de koppeling Downloaden 7 dagen actief nadat u het exporteren hebt gestart.
