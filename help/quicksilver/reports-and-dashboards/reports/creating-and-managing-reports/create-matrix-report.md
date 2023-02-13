---
product-area: reporting
navigation-topic: create-and-manage-reports
title: Een matrixrapport maken
description: Matrix-rapporten bevatten samenvattingsgegevens in een samengevoegde tabelindeling, zodat het eenvoudiger is deze weer te geven dan wanneer ze in een lijst worden weergegeven, zoals in een traditioneel rapport.
author: Nolan
feature: Reports and Dashboards
exl-id: 714f2802-089f-4a41-8205-f397cf474a24
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '1115'
ht-degree: 0%

---

# Een matrixrapport maken

Matrix-rapporten bevatten samenvattingsgegevens in een samengevoegde tabelindeling, zodat het eenvoudiger is deze weer te geven dan wanneer ze in een lijst worden weergegeven, zoals in een traditioneel rapport.

## Wanneer gebruikt u een matrixrapport

U kunt een matrixrapport voor om het even welk rapport tot stand brengen dat 2 of meer Groepen bevat. Een traditioneel rapport kan tot 3 Groepen bevatten, en een matrixrapport kan tot 4 Groepen bevatten.

Bijvoorbeeld, wilt u een rapport van het Uur tot stand brengen dat de uren toont die tijdens een periode van drie maanden worden geregistreerd, en u wilt dat het rapport volgens wie de uren, evenals door maand en week ingaan wordt georganiseerd.

![](assets/report-matrix-overview-350x123.png)

## Hoe gegevens in een matrixrapport worden weergegeven

De informatie in het matrixrapport wordt altijd getoond als numerieke waarde. In de meeste gevallen, zijn de kolommen die een numerieke waarde bevatten best voor het tonen in een matrixrapport (zoals het geregistreerde uren en daadwerkelijke kosten).

Andere kolommen (zoals Status) kunnen echter nog steeds worden weergegeven in het matrixrapport, zoals in de volgende afbeelding wordt getoond:\
![](assets/report-matrix-status-350x73.png)

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
   <td> <p>Plan </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraties op toegangsniveau*</td> 
   <td> <p>Toegang tot rapporten, dashboards, kalenders bewerken</p> <p>Toegang tot filters, weergaven, groepen bewerken</p> <p>Opmerking: Als u nog steeds geen toegang hebt, vraagt u de Workfront-beheerder of deze aanvullende beperkingen op uw toegangsniveau instelt. Voor informatie over hoe een beheerder van Workfront uw toegangsniveau kan wijzigen, zie <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Aangepaste toegangsniveaus maken of wijzigen</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objectmachtigingen</td> 
   <td> <p>Rechten voor een rapport beheren</p> <p>Voor informatie over het aanvragen van aanvullende toegang raadpleegt u <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Toegang tot objecten aanvragen </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Neem contact op met uw Workfront-beheerder om te weten te komen welk plan, licentietype of toegang u hebt.

## Een matrixrapport instellen

1. Creeer een traditioneel rapport dat numerieke gegevens in de rapportoutput bevat.\
   Voor informatie over hoe te om een rapport tot stand te brengen, zie [Een aangepast rapport maken](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).

1. Ga naar het rapport dat u in Stap 1 creeerde, klik **Handelingen rapporteren** selecteert u vervolgens **Bewerken**.

1. (Voorwaardelijk) Als u reeds een Mening creeerde en u het op dit rapport wilt toepassen, klik **Een bestaande weergave toepassen** Selecteer vervolgens de optie Weergave in de vervolgkeuzelijst.
1. (Voorwaardelijk) Als u een nieuwe Mening voor het rapport wilt tot stand brengen, voltooi de volgende stappen:

   1. Klik op de knop **Kolommen (weergave)** selecteert u vervolgens een kolom die u wilt samenvatten in het matrixrapport.
   1. In de **Kolominstellingen** gebied, klikt u op **Deze kolom samenvatten met** selecteert u een van de beschikbare opties voor het samenvatten van de gegevens.

      >[!IMPORTANT]
      >
      >Als deze optie niet is geselecteerd, wordt de informatie uit de kolom niet correct weergegeven in het matrixrapport.

      ![](assets/qs-report-matrix-summarized-350x392.png)

   1. Herhaal dit proces voor elke kolom op het tabblad Kolommen (Weergave) en klik vervolgens op **Gereed**.

1. Klik op de knop **Groepen** tab.
1. (Voorwaardelijk) Als u reeds een Groepering creeerde en u wilt het op dit rapport toepassen, klik **Een bestaande groepering toepassen** Selecteer vervolgens Groeperen in de vervolgkeuzelijst.
1. (Voorwaardelijk) als u een nieuwe matrixgroepering voor het rapport wilt tot stand brengen, voltooi de volgende stappen:

   1. Selecteren **Overschakelen naar matrixgroepering** in de rechterbovenhoek van de builderinterface.
   1. In de **Rijgroepen** in de sectie, identificeert u de rijgroepering, waarmee de horizontale groepen van de tabel worden ingesteld.
   1. (Optioneel) Als u een extra rijgroepering wilt toevoegen, klikt u op **Secundaire rijgroepering toevoegen**.
   1. In de **Kolomgroepen** de kolomgroepering aan, die de verticale groepen van de tabel bepaalt.
   1. (Optioneel) Als u een extra kolomgroepering wilt toevoegen, klikt u op **Secundaire kolomgroepering toevoegen**.
   1. (Voorwaardelijk) Als u een groepering door datum toevoegt, specificeer ook of de resultaten door dag, week, maand, kwartaal of jaar worden gegroepeerd.\
      ![](assets/qs-grouping-by-date-options-for-matrix-report-350x450.png)

   1. (Voorwaardelijk) Als u hebt geselecteerd om op datum te groeperen en resultaten per kwartaal weer te geven, geeft u bijvoorbeeld op of u kwarten zonder gegevens wilt weergeven door de optie **Rijen zonder resultaten tonen** selectievakje.\
      ![](assets/qs-show-quarters-with-no-results-on-matrix-report-350x175.png)

      >[!NOTE]
      >
      >De **Rijen zonder resultaten tonen** Het veld is alleen beschikbaar voor matrixgroepen en niet voor standaardgroepen.\
      >Alleen de kwartalen zonder gegevens tussen twee kwartalen met geldige gegevens geven nul weer voor de gegevenswaarden op het matrixtabblad. De kwartalen die geen gegevens hebben die aan het begin en het eind van het tijdkader worden gevestigd door uw filter wordt geselecteerd verschijnen bij allen niet in de matrixgroepering die. De kwartalen zonder resultaten zullen niet in een groepering op het lusje van Details van het rapport tonen.

1. (Optioneel en voorwaardelijk) Klik op **Matrixinstellingen** Selecteer vervolgens een van de volgende opties:\
   **Aantal records tonen:** Selecteer deze optie om een rij weer te geven met het totale aantal items voor het opgegeven veld.\
   **Waarde kolom tonen:** Selecteer deze optie om de volgende informatie in de matrix weer te geven:

   * Aantal records
   * De kolom Waarde

      >[!NOTE]
      >
      >Deze kolom bevat informatie die beschrijft wat de gegevens in elke rij vertegenwoordigen.\
      >De volgende uitzonderingen gelden voor bovenliggende objecten (bijvoorbeeld bovenliggende taken) wanneer u waarden samenvoegt voor de volgende velden in groepen:
      >
      >   
      >   
      >   * Alle getallen en valutavelden behalve Werkelijke uren (bijvoorbeeld Geplande/Werkelijke loonkosten, Geplande/Werkelijke kosten, Geplande/Werkelijke kosten, Geplande/Geplande uren) tellen alleen de waarden voor de kindertaken en standalone taken samen. De waarden voor de bovenliggende taken of ouders van ouders worden niet samengevoegd.
      >   * Werkelijke uren tellen de waarden voor de hoofdouder en de standalone taken samen; zij tellen niet de aantallen voor de ouders van oudertaken of de kindtaken samen.
      >   * Aangepaste gegevensvelden voor getal- en valutawaarden voegen alle taken samen: ouders, kinderen, ouders van ouders en zelfstandige taken. Als u het matrixrapport hebt gemaakt om de geplande uren of de werkelijke uren in het dialoogvenster weer te geven **Waarde** kolom, moet u er rekening mee houden dat uren- of kosteninformatie voor bovenliggende objecten (zoals bovenliggende taken) niet wordt weergegeven in het matrixrapport. Als u uren op bovenliggende objecten wilt weergeven, moet u de opdracht **Details** tab.

   **Voorwaardelijke regels:** Stel eventuele opmaakregels in voor waarden die worden samengevoegd.\
   Nadat u een regel hebt toegevoegd, kunt u veld- en tekststijlen definiëren voor de weergave van velden die overeenkomen met die regel. Klikken **Regel toevoegen** nadat u klaar bent met het definiëren van de regel, **Gereed** om de regel op te slaan.

1. Klik op de knop **Filters** om te bepalen welke informatie in het rapport zal tonen.
1. (Voorwaardelijk) Als u reeds een Filter creeerde en u wilt het op dit rapport toepassen, klik **Een bestaand filter toepassen** Selecteer vervolgens het filter in de vervolgkeuzelijst.
1. (Voorwaardelijk) als u een nieuwe Filter voor dit rapport wilt tot stand brengen, zie [Filter- en voorwaardenmodificatoren](../../../reports-and-dashboards/reports/reporting-elements/filter-condition-modifiers.md)

   <!--
   <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
   and
   <a href="../../../reports-and-dashboards/reports/reporting-elements/advanced-filter-condition-qualifiers.md" class="MCXref xref">Advanced Filter and condition qualifiers </a>
   </MadCap:conditionalText>
   -->

   voor informatie over de verschillende aanduidingen die u kunt gebruiken bij het maken van filters.

1. Klikken **Opslaan en sluiten** om het matrixrapport op te slaan en te bekijken.
