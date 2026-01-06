---
product-area: projects
navigation-topic: financials
title: Informatie beheren in het gebied Projectfinanciering
description: U kunt de financiële informatie van een project bekijken of uitgeven door tot het gebied van de Financiën van de sectie van de Details van het Project toegang te hebben.
author: Lisa
feature: Work Management
exl-id: 147f5d55-a827-4cca-9ab0-afb03a4bcd5a
source-git-commit: dbc4404501e20b3f1905a5eebd13734a65db27ae
workflow-type: tm+mt
source-wordcount: '1275'
ht-degree: 0%

---

# Informatie beheren in het gebied Projectfinanciering

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: some information in here is duplicated in Edit projects. If you need to update one of the fields in this area, do it in both places.)</p>
-->

U kunt de financiële informatie van een project bekijken of uitgeven door tot het gebied van de Financiën van de sectie van de Details van het Project toegang te hebben. Er is een beperkt aantal velden dat u in dit gebied kunt weergeven of bewerken. Voor informatie over het uitgeven van alle informatie voor een project, zie [&#x200B; projecten &#x200B;](../../../manage-work/projects/manage-projects/edit-projects.md) uitgeven.

## Toegangsvereisten

+++ Breid uit om de toegangseisen voor de functionaliteit in dit artikel weer te geven.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Adobe Workfront-pakket</td> 
   <td>Alle</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-licentie</td>
   <td>
   <p>Licht of hoger</p>
   <p>Controleren of hoger</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraties op toegangsniveau</td> 
   <td> <p>Toegang tot projecten en financiële gegevens bekijken of vergroten</p> <p>Toegang tot projecten en financiële gegevens bewerken om financiële informatie over het project te bewerken</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objectmachtigingen</td> 
   <td> <p>De toestemmingen van de mening aan een project of hoger die de toestemmingen van de Financiën van de Mening omvatten</p> <p>Machtigingen beheren voor het project met onder andere de functie Financiën beheren om financiële informatie voor het project te bewerken</p> </td> 
  </tr> 
 </tbody> 
</table>

Voor informatie, zie [&#x200B; vereisten van de Toegang in de documentatie van Workfront &#x200B;](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Overzicht van het gebied Financiën

Houd rekening met het volgende wanneer u informatie bekijkt of bewerkt in het gedeelte Financiën:

* De financiële informatie u op het gebied van de Financiën van de Details van het Project kunt vinden vertegenwoordigt waarden die tot het projectniveau van taken rollen, evenals informatie die direct op het project is ingegaan. Sommige financiële informatie kan op het project evenals het taakniveau worden beheerd.
* U moet de toestemmingen van de Mening over het project evenals toegang tot Financiële Gegevens van uw toegangsniveau hebben om het gebied van Financiën op een project te kunnen bekijken.
* U moet over beheerdersmachtigingen voor het project beschikken en toegang tot financiële gegevens vanaf uw toegangsniveau om de gegevens in het gebied Financiën te kunnen bewerken. Wij raden echter aan dat alleen de eigenaar van het project de gegevens in dit gebied bewerkt.

## Financiële informatie over een project weergeven

1. Ga naar een project.
1. Klik **Details van het Project** in het linkerpaneel.
1. Klik **uitgeven** pictogram ![&#x200B; geeft pictogram &#x200B;](assets/edit-icon.png) in de hoger-juiste hoek van de sectie van Details uit, dan klik **Financiën**.

   ![&#x200B; het gebied van Financiën in detailmening &#x200B;](assets/finance-area-in-details-view-only-nwe-350x188.png)

   >[!NOTE]
   >
   >Afhankelijk van hoe uw beheerder van Workfront uw Malplaatje van de Lay-out vormde, zou de sectie van het Overzicht niet eerst kunnen worden vermeld, in welk geval het wordt doen ineenstorten. Voor informatie, zie [&#x200B; de mening van Details aanpassen gebruikend een lay-outmalplaatje &#x200B;](../../../administration-and-setup/customize-workfront/use-layout-templates/customize-details-view-layout-template.md).

1. De volgende velden weergeven in het gedeelte Financiën van het project:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Prestatiesindexmethode</td> 
      <td> Controls the method Workfront uses to calculate Earned Value metrics. Het kan op uren-gebaseerd, of op kosten-gebaseerd zijn. <br> voor meer informatie over PIM, zie het artikel <a href="../../../manage-work/projects/project-finances/set-pim.md" class="MCXref xref"> plaatsen de Methode van de Index van Prestaties (PIM) </a></td> 
     </tr> 
     <tr> 
      <td role="rowheader">CPI/SPI/CSI</td> 
      <td> <p>Dit zijn de metriek van projectprestaties die tonen hoe uw project, op een bepaald ogenblik presteert. Hun waarden worden berekend op basis van de prestatiesindexmethode.<br> voor meer informatie zie de volgende artikelen: </p> 
       <ul> 
        <li> <p><a href="../../../manage-work/projects/project-finances/calculate-cpi.md" class="MCXref xref"> berekent de Index van de Prestaties van Kosten (CPI) </a> </p> </li> 
        <li> <p><a href="../../../manage-work/projects/project-finances/calculate-spi.md" class="MCXref xref"> de Index van de Prestaties van het Programma berekenen (SPI) </a> </p> </li> 
        <li> <p><a href="../../../manage-work/projects/project-finances/calculate-csi.md" class="MCXref xref"> berekent de Index van de Prestaties van het Programma van Kosten (CSI) </a> </p> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Schatting bij voltooiing</td> 
      <td> De voorspelde totale kosten van uw project, in uren vertegenwoordigd als de Methode van de Index van Prestaties (PIM) op uren-gebaseerd is, en het wordt vertegenwoordigd in een muntwaarde, als de Methode van de Index van Prestaties (PIM) op kosten-gebaseerd is.<br> voor meer informatie over het berekenen van Schatting bij Voltooiing, zie het artikel <a href="../../../manage-work/projects/project-finances/calculate-eac.md" class="MCXref xref"> Schatting bij Voltooiing (EAC) berekenen </a></td> 
     </tr> 
     <tr> 
      <td role="rowheader">Begroting</td> 
      <td>Dit is de begroting voor het project. Dit wordt manueel gespecificeerd door de Eigenaar van het Project.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Vaste kosten</td> 
      <td>Dit zijn de vaste kosten van het project, onafhankelijk van andere activiteiten in verband met het project. Ze worden handmatig ingevoerd door de projecteigenaar.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Geplande kosten</td> 
      <td>De geraamde kosten van het project, gebaseerd op geplande uren en de tarieven die zijn gekoppeld aan de taaktoewijzing (rollen of gebruikers).</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Werkelijke kosten</td> 
      <td>Alle kosten van het project. De werkelijke kosten zijn de som van alle werkelijke kosten: loonkosten (gebaseerd op Werkelijke uren en de tarieven die gekoppeld zijn aan de functies of gebruikers die deze bijhouden), kosten en vaste kosten, die aan een project of taak kunnen worden gekoppeld.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Vaste inkomsten</td> 
      <td>Stel de verwachte inkomsten in op basis van het projectschema. De vaste opbrengsten worden handmatig opgegeven door de eigenaar van het project.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Geplande inkomsten</td> 
      <td>Verwachte inkomsten op basis van de geplande uren en de tarieven die zijn gekoppeld aan de taaktoewijzing (functies of gebruikers).</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Werkelijke ontvangsten</td> 
      <td>Werkelijke inkomsten uit het project op basis van de werkelijke uren en de tarieven die aan de taaktoewijzing zijn gekoppeld (functies of gebruikers).</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Gefactureerde inkomsten</td> 
      <td> <p>Inkomsten die in rekening worden gebracht aan klanten of andere partijen en die worden vastgelegd in factureringsverslagen. Voor meer informatie over het factureren verslagen, zie het artikel <a href="../../../manage-work/projects/project-finances/create-billing-records.md" class="MCXref xref"> het factureren verslagen </a> creëren. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> </td> 
      <td> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> </td> 
      <td> </td> 
     </tr> 
    </tbody> 
   </table>

## Financiële informatie over een project bewerken

Als Eigenaar van het Project, kunt u de informatie op subtab Financiën van een project uitgeven.

Informatie bewerken op het subtabblad Projectfinanciering:

1. Ga naar een project waarvan u de eigenaar bent.

   >[!NOTE]
   >
   >U hebt beheermachtigingen voor het project nodig om de volgende stappen uit te voeren. We raden ook aan dat alleen de eigenaar van het project wijzigingen aanbrengt in het subtabblad Financiën van het project.

1. Klik **Details van het Project** in het linkerpaneel.
1. Klik **uitgeven** pictogram ![&#x200B; geeft pictogram &#x200B;](assets/edit-icon.png) in de hoger-juiste hoek van de sectie van Details uit, dan klik **Financiën**. Hierdoor wordt de financiële ruimte geopend voor bewerking.
1. Bewerk elk veld dat u kunt bewerken door één keer op het veld te klikken of klik op **+Toevoegen** om informatie toe te voegen aan een leeg veld.

   >[!TIP]
   >
   >Velden kunnen niet worden bewerkt als ze automatisch door Workfront worden berekend of als u geen bewerkingsmachtigingen hebt.

   ![&#x200B; geef financieringsgebied &#x200B;](assets/edit-finance-area-in-project-details-nwe-350x275.png) uit

1. Werk een van de onderstaande velden bij.

   >[!NOTE]
   >
   >Afhankelijk van de manier waarop uw Workfront-beheerder onze lay-outsjabloon instelt, kunnen de velden in de sectie Projectdetails in uw omgeving verschillen. Voor informatie, zie [&#x200B; de mening van Details aanpassen gebruikend een lay-outmalplaatje &#x200B;](../../../administration-and-setup/customize-workfront/use-layout-templates/customize-details-view-layout-template.md).

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Prestatiesindexmethode</td> 
      <td> <p>Controls the method Workfront uses to calculate project performance metrics. Dit wordt opstelling op het systeemniveau door uw beheerder, maar u kunt het op het projectniveau ook uitgeven. U kunt een van de volgende opties selecteren:</p> 
       <ul> 
        <li><strong> op uur-Gebaseerd:</strong> Workfront gebruikt de Geplande Uren in het berekenen van CPI en EAC van het project, en EAC van de projectvertoningen als aantal, in uren. </li> 
        <li><strong> Op kosten-Gebaseerd:</strong> Workfront gebruikt de Geplande Kosten van de Arbeid in het berekenen van CPI en EAC van het project, en de vertoningen EAC als muntwaarde. Wanneer u deze optie selecteert, moet u ervoor zorgen dat uw taaktoewijzingen (taakrollen of gebruikers) aan kostentarieven zijn gekoppeld.</li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Schatting bij voltooiing</td> 
      <td> <p>Vertegenwoordigt de verwachte totale kosten van uw project of taak wanneer het voltooit. Dit wordt opstelling op het systeemniveau door uw beheerder, maar u kunt het op het projectniveau ook uitgeven. U kunt een van de volgende opties selecteren:</p> 
       <ul> 
        <li><strong> berekent op het Niveau van het Project </strong>: EAC voor de oudertaak en het project worden bepaald door de daadwerkelijke uren/daadwerkelijke arbeidskosten in te gaan in de Formulas EAC. Deze berekening omvat Werkelijke uren/kosten en uitgaven die rechtstreeks aan de oudertaak of het project worden toegevoegd.</li> 
        <li><strong> Roll omhoog van Taken/Subtasks </strong>: EAC voor de oudertaak en het project worden bepaald door EAC voor elke kindtaak op te vatten. Deze berekening sluit Werkelijke uren/kosten en kosten uit die rechtstreeks aan de oudertaak of het project worden toegevoegd.</li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Begroting</td> 
      <td>Geef het budget voor dit project op.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Vaste kosten</td> 
      <td>Geef de vaste kosten voor dit project op. Hieronder vallen geen arbeids- of kostenkosten.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Vaste inkomsten</td> 
      <td> <p>Geef de vaste inkomsten van dit project op. Hieronder vallen geen inkomsten uit factureringsgegevens die aan partners of derden in rekening worden gebracht.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Projectvaluta</td> 
      <td> <p>Geef een valuta op voor dit project als deze afwijkt van de standaardvaluta in uw systeem. De standaardvaluta in uw systeem wordt bepaald door uw beheerder van Workfront. Voor meer informatie over vestiging ruilen in Workfront, zie het artikel <a href="../../../administration-and-setup/manage-workfront/exchange-rates/set-up-exchange-rates.md" class="MCXref xref"> de wisselkoers van de Opstelling </a>.</p> </td> 
     </tr>
    </tbody> 
   </table>

1. Klik **sparen Veranderingen**.
