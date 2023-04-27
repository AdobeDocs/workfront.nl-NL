---
product-area: projects
navigation-topic: financials
title: Informatie beheren in het gebied Projectfinanciering
description: Informatie beheren in het gebied Projectfinanciering
author: Alina
feature: Work Management
exl-id: 147f5d55-a827-4cca-9ab0-afb03a4bcd5a
source-git-commit: d8c274d2153836647367c263cad8d786402cbe7f
workflow-type: tm+mt
source-wordcount: '1304'
ht-degree: 0%

---

# Informatie beheren in het gebied Projectfinanciering

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: some information in here is duplicated in Edit projects. If you need to update one of the fields in this area, do it in both places.)</p>
-->

U kunt de financiële informatie van een project bekijken of uitgeven door tot het gebied van de Financiën van de sectie van de Details van het Project toegang te hebben. Er is een beperkt aantal velden dat u in dit gebied kunt weergeven of bewerken. Voor informatie over het bewerken van alle informatie voor een project raadpleegt u [Projecten bewerken](../../../manage-work/projects/manage-projects/edit-projects.md).

## Toegangsvereisten

U moet de volgende toegang hebben om de stappen in dit artikel uit te voeren:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-abonnement*</td> 
   <td> <p>Alle</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-licentie*</td> 
   <td> <p>Controleren of hoger</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraties op toegangsniveau*</td> 
   <td> <p>Toegang tot projecten en financiële gegevens bekijken of vergroten</p> <p>Toegang tot projecten en financiële gegevens bewerken om financiële informatie over het project te bewerken</p> <p>Opmerking: Als u nog steeds geen toegang hebt, vraagt u de Workfront-beheerder of deze aanvullende beperkingen op uw toegangsniveau instelt. Voor informatie over hoe een beheerder van Workfront uw toegangsniveau kan veranderen, zie <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Aangepaste toegangsniveaus maken of wijzigen</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objectmachtigingen</td> 
   <td> <p>De toestemmingen van de mening aan een project of hoger die de toestemmingen van de Financiën van de Mening omvatten</p> <p>Machtigingen beheren voor het project met onder andere de functie Financiën beheren om financiële informatie voor het project te bewerken</p> <p>Voor informatie over het aanvragen van aanvullende toegang raadpleegt u <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Toegang tot objecten aanvragen </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Neem contact op met uw Workfront-beheerder om te weten te komen welk plan, licentietype of toegang u hebt.

## Overzicht van het gebied Financiën

Houd rekening met het volgende wanneer u informatie bekijkt of bewerkt in het gedeelte Financiën:

* De financiële informatie u op het gebied van de Financiën van de Details van het Project kunt vinden vertegenwoordigt waarden die tot het projectniveau van taken rollen, evenals informatie die direct op het project is ingegaan. Sommige financiële informatie kan op het project evenals het taakniveau worden beheerd.
* U moet de toestemmingen van de Mening over het project evenals toegang tot Financiële Gegevens van uw toegangsniveau hebben om het gebied van Financiën op een project te kunnen bekijken.
* U moet over beheerdersmachtigingen voor het project beschikken en toegang tot financiële gegevens vanaf uw toegangsniveau om de gegevens in het gebied Financiën te kunnen bewerken. Wij raden echter aan dat alleen de eigenaar van het project de gegevens in dit gebied bewerkt.

## Financiële informatie over een project weergeven

1. Ga naar een project.
1. Klikken **Projectdetails** in het linkerdeelvenster.
1. Klik op de knop **Bewerken** pictogram ![](assets/edit-icon.png) in de rechterbovenhoek van de sectie Details klikt u op **Financiën**.

   ![](assets/finance-area-in-details-view-only-nwe-350x188.png)

   >[!NOTE]
   >
   >Afhankelijk van hoe uw beheerder van Workfront uw Malplaatje van de Lay-out vormde, zou de sectie van het Overzicht niet eerst kunnen worden vermeld, in welk geval het wordt doen ineenstorten. Zie voor meer informatie [De weergave Details aanpassen met een lay-outsjabloon](../../../administration-and-setup/customize-workfront/use-layout-templates/customize-details-view-layout-template.md).

1. De volgende velden weergeven in het gedeelte Financiën van het project:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Prestatiesindexmethode</td> 
      <td> Controls the method Workfront uses to calculate Earned Value metrics. Het kan op uren-gebaseerd, of op kosten-gebaseerd zijn. <br>Raadpleeg het artikel voor meer informatie over de PIM <a href="../../../manage-work/projects/project-finances/set-pim.md" class="MCXref xref">De PIM-methode (Performance Index) instellen</a></td> 
     </tr> 
     <tr> 
      <td role="rowheader">CPI/SPI/CSI</td> 
      <td> <p>Dit zijn de metriek van projectprestaties die tonen hoe uw project, op een bepaald ogenblik presteert. Hun waarden worden berekend op basis van de prestatiesindexmethode.<br>Zie de volgende artikelen voor meer informatie: </p> 
       <ul> 
        <li> <p><a href="../../../manage-work/projects/project-finances/calculate-cpi.md" class="MCXref xref">Kostenprestatie-index (CPI) berekenen</a> </p> </li> 
        <li> <p><a href="../../../manage-work/projects/project-finances/calculate-spi.md" class="MCXref xref">Prestatie-index (SPI) voor planning berekenen </a> </p> </li> 
        <li> <p><a href="../../../manage-work/projects/project-finances/calculate-csi.md" class="MCXref xref">Prestatie-index (CSI) voor kostenplanning berekenen</a> </p> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Schatting bij voltooiing</td> 
      <td> De voorspelde totale kosten van uw project, in uren vertegenwoordigd als de Methode van de Index van Prestaties (PIM) op uren-gebaseerd is, en het wordt vertegenwoordigd in een muntwaarde, als de Methode van de Index van Prestaties (PIM) op kosten-gebaseerd is.<br>Raadpleeg het artikel voor meer informatie over het berekenen van de schatting bij voltooiing <a href="../../../manage-work/projects/project-finances/calculate-eac.md" class="MCXref xref">Schatting berekenen bij voltooiing (EAC)</a></td> 
     </tr> 
     <tr> 
      <td role="rowheader">Begroting</td> 
      <td>Dit is de begroting voor het project. Dit wordt handmatig opgegeven door de eigenaar van het project.</td> 
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
      <td>Alle kosten van het project. De werkelijke kosten zijn de som van alle werkelijke kosten: arbeidskosten (gebaseerd op Werkelijke uren en de tarieven verbonden aan de baanrollen of gebruikers die hen registreren), uitgaven, en vaste kosten, die met een project of een taak kunnen worden geassocieerd.</td> 
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
      <td> <p>Inkomsten die in rekening worden gebracht aan klanten of andere partijen en die worden vastgelegd in factureringsverslagen. Raadpleeg het artikel voor meer informatie over factureringsrecords <a href="../../../manage-work/projects/project-finances/create-billing-records.md" class="MCXref xref">Factureringsrecords maken</a>. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> </td> 
      <td> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> </td> 
      <td> </td> 
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

1. Klikken **Projectdetails** in het linkerdeelvenster.
1. Klik op de knop **Bewerken** pictogram ![](assets/edit-icon.png) in de rechterbovenhoek van de sectie Details klikt u op **Financiën** . Hierdoor wordt de financiële ruimte geopend voor bewerking.
1. Bewerk een veld dat u kunt bewerken door één keer op het veld te klikken of klik op **+Toevoegen** om informatie toe te voegen aan een leeg veld.

   >[!TIP]
   >
   >Velden kunnen niet worden bewerkt als ze automatisch door Workfront worden berekend of als u geen bewerkingsmachtigingen hebt.

   ![](assets/edit-finance-area-in-project-details-nwe-350x275.png)

1. Werk een van de onderstaande velden bij.

   >[!NOTE]
   >
   >Afhankelijk van de manier waarop uw Workfront-beheerder onze lay-outsjabloon instelt, kunnen de velden in de sectie Projectdetails in uw omgeving verschillen. Zie voor meer informatie [De weergave Details aanpassen met een lay-outsjabloon](../../../administration-and-setup/customize-workfront/use-layout-templates/customize-details-view-layout-template.md).

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Prestatiesindexmethode</td> 
      <td> <p>Controls the method Workfront uses to calculate project performance metrics. Dit wordt opstelling op het systeemniveau door uw beheerder, maar u kunt het op het projectniveau ook uitgeven. U kunt een van de volgende opties selecteren:</p> 
       <ul> 
        <li><strong>Uur:</strong>Workfront gebruikt de geplande uren voor de berekening van de CPI en de EAC van het project en de EAC van het project wordt weergegeven als een aantal, in uren. </li> 
        <li><strong>Op basis van kosten:</strong>Workfront gebruikt de geplande loonkosten voor de berekening van de CPI en de EAC van het project, en de EAC wordt weergegeven als een valutawaarde. Wanneer u deze optie selecteert, moet u ervoor zorgen dat uw taaktoewijzingen (taakrollen of gebruikers) aan kostentarieven zijn gekoppeld.</li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Schatting bij voltooiing</td> 
      <td> <p>Vertegenwoordigt de verwachte totale kosten van uw project of taak wanneer het voltooit. Dit wordt opstelling op het systeemniveau door uw beheerder, maar u kunt het op het projectniveau ook uitgeven. U kunt een van de volgende opties selecteren:</p> 
       <ul> 
        <li><strong>Berekenen op projectniveau</strong>: EAC voor de bovenliggende taak en het project wordt bepaald door de werkelijke uren/werkelijke loonkosten in de EAC-formules in te voeren. Deze berekening omvat Werkelijke uren/kosten en uitgaven die rechtstreeks aan de oudertaak of het project worden toegevoegd.</li> 
        <li><strong>Omhoog rollen vanuit Taken/Subtaken</strong>: EAC voor de oudertaak en het project worden bepaald door EAC voor elke kindtaak samen te vatten. Deze berekening sluit Werkelijke uren/kosten en kosten uit die rechtstreeks aan de oudertaak of het project worden toegevoegd.</li> 
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
      <td> <p>Geef een valuta op voor dit project als deze afwijkt van de standaardvaluta in uw systeem. De standaardvaluta in uw systeem wordt bepaald door uw beheerder van Workfront. Raadpleeg het artikel voor meer informatie over het instellen van wisselkoersen in Workfront <a href="../../../administration-and-setup/manage-workfront/exchange-rates/set-up-exchange-rates.md" class="MCXref xref">Wisselkoersen instellen</a>.</p> </td> 
     </tr>
    </tbody> 
   </table>

1. Klikken **Wijzigingen opslaan**.
