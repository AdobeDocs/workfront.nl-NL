---
product-area: templates
navigation-topic: templates-navigation-topic
title: Sjabloontaken kopiëren en verplaatsen
description: U kunt een sjabloontaak naar dezelfde sjabloon of naar een andere sjabloon verplaatsen.
author: Alina
feature: Work Management
exl-id: a2e09e63-5c88-460c-9996-3a39fbb82150
source-git-commit: b02c81873d84946f8db54bcf9a1a464de38781de
workflow-type: tm+mt
source-wordcount: '2128'
ht-degree: 0%

---

# Sjabloontaken kopiëren en verplaatsen

U kunt een sjabloontaak van een sjabloon naar een andere sjabloon kopiëren of deze naar een andere sjabloon of naar een andere plaats in dezelfde sjabloon verplaatsen.

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
   <td> <p>Toegang tot sjablonen bewerken</p> <p><b>OPMERKING</b>

Als u nog steeds geen toegang hebt, vraagt u de Workfront-beheerder of deze aanvullende beperkingen op uw toegangsniveau instelt. Voor informatie over hoe een beheerder van Workfront uw toegangsniveau kan wijzigen, zie <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref"> tot douanetoegangsniveaus </a> leiden of wijzigen.</p> </td>
</tr> 
  <tr> 
   <td role="rowheader">Objectmachtigingen</td> 
   <td> <p>Rechten voor een sjabloon en de sjabloontaak beheren </p> <p>Voor informatie bij het vragen van om extra toegang, zie <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref"> de toegang van het Verzoek tot voorwerpen </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

*Neem contact op met uw Workfront-beheerder om te weten te komen welk abonnement, licentietype of toegang u hebt.

## Overwegingen bij het kopiëren of verplaatsen van sjabloontaken

Houd rekening met het volgende wanneer u sjabloontaken kopieert:

* De volgende informatie wordt niet overgedragen naar de gekopieerde taak:

   * Mijlpalen

* U kunt bepaalde items die aan de sjabloontaak zijn gekoppeld tijdens het kopiëren naar de gekopieerde taak kopiëren. De volgende objecten worden echter standaard niet overgedragen naar de gekopieerde taak:

   * Opmerkingen van gebruikers

* Aangepaste formulieren worden samen met de sjabloontaak gekopieerd wanneer u een sjabloontaak kopieert. De gegevens in de aangepaste velden worden alleen naar de nieuwe sjabloontaak overgedragen wanneer u Aangepaste gegevens wilt kopiëren.

* De volgende punten brengen aan de gekopieerde malplaatjetaak door gebrek over:

   * Subtaken

Houd rekening met het volgende wanneer u sjabloontaken verplaatst:

* De volgende informatie wordt standaard overgedragen naar de verplaatste taak:

   * Aangepaste formulieren en aangepaste veldgegevens
   * Subtaken
   * Opmerkingen van gebruikers

* De volgende informatie wordt niet overgedragen naar de verplaatste taak:

   * Mijlpalen.

## Sjabloontaken kopiëren

U kunt één sjabloontaak kopiëren of meerdere sjabloontaken bulksgewijs kopiëren.

1. Ga naar de sjabloon die de sjabloontaak of sjabloontaken bevat die u wilt kopiëren.
1. Klik **Taken van het Malplaatje** in het linkerpaneel.
1. Voer een van de volgende handelingen uit:
   * Klik op de naam van een sjabloontaak om deze te openen.
   * Selecteer een of meerdere sjabloontaken in de lijst.
1. (Voorwaardelijk) klik het **Meer** menu ![](assets/more-icon.png) bij de bovenkant van de lijst van de malplaatjetaak of rechts van de naam van de malplaatjetaak als u de taak opende, dan klik **Exemplaar aan** of **Exemplaar**, afhankelijk waar u tot de optie van het Exemplaar toegang hebt.
Het vak Sjabloontaak kopiëren wordt geopend.
   ![](assets/copy-template-task-box-unshimmed.png)
1. (Facultatief) noem de malplaatjetaak op het **gebied van de Naam van de Taak van het Malplaatje**.

   >[!TIP]
   >
   >Dit veld is grijs en kan niet worden bewerkt als u meerdere sjabloontaken in een lijst wilt kopiëren. U kunt de muisaanwijzer boven het veld Naam sjabloontaak en een lijst met alle geselecteerde sjabloontaken weergeven.

1. Begin typend de naam van het **Malplaatje van de Bestemming** waar u de malplaatjetaak in het **Uitgezochte Malplaatje van de Bestemming** gebied wilt kopiëren, dan het selecteren wanneer het in de lijst toont.

   De huidige sjabloonnaam wordt standaard weergegeven. Als u de sjabloontaak binnen dezelfde sjabloon wilt kopiëren, laat u dit veld ongewijzigd.

   >[!TIP]
   >
   >U kunt ook het referentienummer typen of de id van de sjabloon invoeren. Hierdoor kunt u beter onderscheid maken tussen sjablonen met identieke namen.

1. (Voorwaardelijk) klik **verzoektoegang** om toegang tot het bestemmingsmalplaatje te verzoeken, als u geen toegang tot het geselecteerde malplaatje hebt.
1. (Voorwaardelijk) blijf de malplaatjetaak aan het geselecteerde bestemmingsmalplaatje kopiëren zonder toegang te vragen als u toegang hebt om malplaatjetaken aan één van de malplaatjetaken op het bestemmingsmalplaatje toe te voegen.

1. Klik **Opties** in het linkerpaneel, dan schrap de attributen van de malplaatjetaak die u niet met de malplaatjetaak wilt kopiëren. Alle opties zijn standaard geselecteerd.

   >[!TIP]
   >
   >Deselecterend **Uitgezochte allen** deselecteert alle opties.

   Schakel een van de volgende opties uit als u deze niet wilt overbrengen naar de gekopieerde sjabloontaak. In de volgende tabel wordt beschreven wat er gebeurt wanneer de opties zijn uitgeschakeld:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
    <tr> 
      <td role="rowheader">Alles selecteren</td> 
      <td>Schakel deze optie uit als u alle informatie uit de sjabloontaak wilt verwijderen wanneer u deze naar de nieuwe locatie kopieert. </td> 
     </tr>
     <tr> 
      <td role="rowheader">Restrictie</td> 
      <td> <p>De beperking van de malplaatjetaak wordt geplaatst aan zo spoedig mogelijk of zo laat mogelijk gebaseerd op het plaatsen van de Wijze van het malplaatjeschema.</p> <p> Als deze optie is geselecteerd, wordt de huidige beperking van de sjabloontaak overgedragen naar de gekopieerde sjabloontaak. </p> 
      <p><b>OPMERKING</b>

   Wanneer het kopiëren van een malplaatjetaak met datum-specifieke beperkingen aan een ander malplaatje en de beperkingsdata van de malplaatjetaak zijn buiten de data van het nieuwe malplaatje, of verandert de beperking van de malplaatjetaak in zo spoedig mogelijk of zo laat mogelijk of de Geplande Begin of Geplande Afsluitingsdata van de malplaatjes worden aangepast.

   Hieronder volgen voorbeelden van datumspecifieke beperkingen:
   <ul>
      <li> Moet beginnen op</li>
      <li> Moet worden voltooid op</li>
      <li> Niet eerder starten dan</li>
      <li> Niet later starten dan</li>
      </ul>
     </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Toewijzingen</td> 
      <td> <p>Alle toewijzingen worden verwijderd uit de sjabloontaak. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Goedkeuringsproces</td> 
      <td>Alle goedkeuringsprocessen worden verwijderd uit de sjabloontaak.</td> 
     </tr>

   <tr> 
      <td role="rowheader">Alle voorgangers</td> 
      <td> <p>Dit betekent dat de afhankelijkheden niet worden overgedragen naar de gekopieerde sjabloontaken. </p> <p>Als deze optie is geselecteerd, blijven de voorgangers in de groep met gekopieerde sjabloontaken behouden en worden andere verwijderd.</p> </td> 
     </tr>
     <tr> 
      <td role="rowheader">Aangepaste gegevens</td> 
      <td> <p>De waarden voor de aangepaste velden worden gewist en de aangepaste formulieren worden overgebracht naar de gekopieerde sjabloontaak. </p> <p>Als deze optie is geselecteerd, worden zowel de formulieren als de waarden voor de aangepaste velden overgebracht naar de gekopieerde sjabloontaak. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Financiële informatie</td> 
      <td>De financiële informatie van de gekopieerde sjabloontaak wordt verwijderd en de Workfront werkt het kostentype van de sjabloontaak bij tot Geen kosten en het type van de sjabloontaak als Niet te factureren.
      </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Documenten</td> 
      <td> <p>De documenten in bijlage aan de malplaatjetaak worden niet overgebracht naar de gekopieerde malplaatjetaak. Dit zijn versies, proefdrukken en gekoppelde documenten.</p> <p><b>OPMERKING</b></p>

   <p>Dit omvat geen documentgoedkeuringen. Documentgoedkeuringen kunnen nooit worden gekopieerd wanneer een sjabloontaak wordt gekopieerd.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Herinneringsmeldingen</td> 
      <td>De herinneringen aan sjabloontaken worden niet overgedragen naar de gekopieerde sjabloontaak. </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Uitgaven</td> 
      <td>De uitgaven die op de malplaatjetaak worden geregistreerd brengen niet naar de gekopieerde malplaatjetaak over. </td> 
     </tr>  
    </tbody> 
   </table>


1. (Facultatief) klik **Uitgezochte Ouder** in het linkerpaneel, dan selecteer de malplaatjetaak in het bestemmingsmalplaatje dat u de ouder van de gekopieerde malplaatjetaak wilt worden.

   >[!TIP]
   >
   >Wanneer het selecteren om veelvoudige malplaatjetaken in een lijst te kopiëren, worden alle geselecteerde malplaatjetaken de kinderen van de geselecteerde ouder en toegevoegd na de bestaande kindtaken.

   Voer een van de volgende handelingen uit om een bovenliggend element te selecteren:

   * In de lijst van de malplaatjetaak, selecteer één van de ouders in het malplaatjeplan.
   * Klik het pictogram van het onderzoekspictogram ![ Onderzoek ](assets/search-icon.png) en onderzoek naar een taak van het oudermalplaatje door naam.

   De sjabloontaak moet in de lijst worden weergegeven.

1. Selecteer het keuzerondje voor het bovenliggende element nadat u het hebt gevonden.

   Als u geen taak van het oudermalplaatje selecteert, worden de malplaatjetaken gekopieerd als belangrijkste malplaatjetaken eerder dan subtaken en zij worden geplaatst aan het eind van de lijst van de malplaatjetaak op het bestemmingsmalplaatje.

1. Klik **Taak van het Malplaatje van het Exemplaar**.

   De gekopieerde sjabloontaken bevinden zich nu op de opgegeven sjabloon en zijn subtaken voor de geselecteerde bovenliggende sjabloontaak of de laatste sjabloontaken voor de sjabloon.


## Sjabloontaken verplaatsen

U kunt een sjabloontaak verplaatsen naar een andere sjabloontaak in dezelfde sjabloon of naar een andere sjabloon. U kunt één sjabloontaak of meerdere sjabloontaken bulksgewijs verplaatsen.

1. Ga naar de sjabloon die de sjabloontaak of sjabloontaken bevat die u wilt verplaatsen.
1. Klik **Taken van het Malplaatje** in het linkerpaneel.
1. Voer een van de volgende handelingen uit:
   * Klik op de naam van een sjabloontaak om deze te openen.
   * Selecteer een of meerdere sjabloontaken in de lijst.
1. (Voorwaardelijk) klik het **Meer** menu ![](assets/more-icon.png) bij de bovenkant van de lijst van de malplaatjetaak of rechts van de naam van de malplaatjetaak als u de taak opende, dan klik **Beweging aan** of **Beweging**, afhankelijk van waar u tot de optie van de Beweging toegang hebt.
Het vak Sjabloontaak verplaatsen wordt geopend.
   ![](assets/move-template-task-box-unshimmed.png)

1. (Facultatief) noem de malplaatjetaak op het **gebied van de Naam van de Taak van het Malplaatje**.

   >[!TIP]
   >
   >Dit veld is grijs en kan niet worden bewerkt als u meerdere sjabloontaken in een lijst wilt verplaatsen. U kunt de muisaanwijzer boven het veld Naam sjabloontaak en een lijst met alle geselecteerde sjabloontaken weergeven.

1. Begin typend de naam van het **Malplaatje van de Bestemming** waar u de malplaatjetaak in het **Uitgezochte Malplaatje van de Bestemming** gebied wilt bewegen, dan het selecteren wanneer het in de lijst toont.

   >[!TIP]
   >
   >U kunt ook het referentienummer typen of de id van de sjabloon invoeren. Hierdoor kunt u beter onderscheid maken tussen sjablonen met identieke namen.

1. (Voorwaardelijk) klik **verzoektoegang** om toegang tot het malplaatje te verzoeken, als u geen toegang tot het bestemmingsmalplaatje hebt.
1. (Voorwaardelijk) blijf de malplaatjetaak aan het geselecteerde bestemmingsmalplaatje verplaatsen zonder toegang te vragen als u toegang hebt om malplaatjetaken aan één van de malplaatjetaken op het bestemmingsmalplaatje toe te voegen.

1. Klik **Opties** in het linkerpaneel, dan schrap de attributen van de malplaatjetaak die u niet met de malplaatjetaak wilt kopiëren. Alle opties zijn standaard geselecteerd.

   >[!TIP]
   >
   >* De sectie Opties is alleen beschikbaar nadat u een doelsjabloon hebt geselecteerd.
   >* Deselecterend **Uitgezochte allen** deselecteert alle opties.

   Schakel een van de volgende opties uit als u de gegevens niet wilt overbrengen naar de verplaatste sjabloontaak. In de volgende tabel wordt beschreven wat er gebeurt wanneer de opties zijn uitgeschakeld:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
    <tr> 
      <td role="rowheader">Alles selecteren</td> 
      <td>Schakel deze optie uit als u alle informatie uit de sjabloontaak wilt verwijderen wanneer u deze naar de nieuwe locatie verplaatst. </td> 
     </tr>
     <tr> 
      <td role="rowheader">Restrictie</td> 
      <td> <p>De beperking van de malplaatjetaak wordt geplaatst aan zo spoedig mogelijk of zo laat mogelijk gebaseerd op het plaatsen van de Wijze van het malplaatjeschema.</p> <p> Als deze optie is geselecteerd, wordt de huidige beperking van de sjabloontaak overgedragen naar de verplaatste sjabloontaak. </p>

   <p><b>OPMERKING</b>

   Wanneer het bewegen van een malplaatjetaak met datum-specifieke beperkingen aan een ander malplaatje en de beperkingsdata van de malplaatjetaak zijn buiten de data van het nieuwe malplaatje, of verandert de beperking van de malplaatjetaak in zo spoedig mogelijk of zo laat mogelijk of de Geplande Begin of Geplande Afsluitingsdata van de malplaatjes worden aangepast.

   Hieronder volgen voorbeelden van datumspecifieke beperkingen:
   <ul>
      <li> Starten bij</li>
      <li> Moet worden voltooid op</li>
      <li> Niet eerder starten dan</li>
      <li> Niet later starten dan</li>
      </ul>


   </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Toewijzingen</td> 
      <td> <p>Alle toewijzingen worden verwijderd uit de sjabloontaak. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Goedkeuringsproces</td> 
      <td>Alle goedkeuringsprocessen worden verwijderd uit de sjabloontaak.</td> 
     </tr>

   <tr> 
      <td role="rowheader">Alle voorgangers</td> 
      <td> <p>Dit betekent dat de afhankelijkheden niet worden overgedragen met de verplaatste sjabloontaken. </p> <p>Als deze optie is geselecteerd, blijven de voorgangers in de groep verplaatste sjabloontaken behouden en worden andere verwijderd.</p> </td> 
     </tr>
     <tr> 
      <td role="rowheader">Aangepaste gegevens</td> 
      <td> <p>De waarden voor de aangepaste velden worden gewist en de aangepaste formulieren worden overgebracht met de verplaatste sjabloontaak. </p> <p>Als deze optie is geselecteerd, worden zowel de formulieren als de waarden voor de aangepaste velden overgedragen met de verplaatste sjabloontaak. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Financiële informatie</td> 
      <td>De financiële informatie van de verplaatste malplaatjetaak wordt verwijderd en Workfront werkt het Type van de Kosten van de malplaatjetaak aan Geen Kosten en het Type van de Inkomsten van de malplaatjetaak als niet Billable bij.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Documenten</td> 
      <td> <p>De documenten die aan de sjabloontaak zijn gekoppeld, worden niet overgedragen met de verplaatste sjabloontaak. Dit zijn versies, proefdrukken en gekoppelde documenten.</p>

   <p><b>OPMERKING</b></p>

   <ul><li>
      <p>Dit omvat geen documentgoedkeuringen. Documentgoedkeuringen kunnen nooit worden verplaatst wanneer een sjabloontaak wordt verplaatst.</p> </li>
      <li>Als u ervoor kiest de documenten niet te laten verplaatsen met de sjabloontaak, worden de documenten verwijderd en gedurende 30 dagen in de prullenbak geplaatst. Een beheerder kan ze herstellen en ze worden hersteld op de verplaatste sjabloontaak.

   Als de sjabloontaak wordt verwijderd nadat deze is verplaatst, worden de herstelde documenten geplaatst in het gebied Documenten van de gebruikerspagina van de beheerder die ze herstelt. </li> </ul>

   </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Herinneringsmeldingen</td> 
      <td>De herinneringen aan sjabloontaken worden niet overgedragen naar de verplaatste sjabloontaak. </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Uitgaven</td> 
      <td>De uitgaven die op de malplaatjetaak worden geregistreerd brengen niet met de verplaatste malplaatjetaak over. </td> 
     </tr>  
    </tbody> 
   </table>


1. (Facultatief) klik **Uitgezochte Ouder** in het linkerpaneel, dan selecteer de malplaatjetaak in het bestemmingsmalplaatje dat u de ouder van de verplaatste malplaatjetaak wilt worden.

   >[!TIP]
   >
   >Wanneer u selecteert om meerdere sjabloontaken in een lijst te verplaatsen, worden alle geselecteerde sjabloontaken de onderliggende taken van het geselecteerde bovenliggende element en worden deze toegevoegd na de bestaande onderliggende taken.

   Voer een van de volgende handelingen uit om een bovenliggend element te selecteren:

   * In de lijst van de malplaatjetaak, selecteer één van de ouders in het malplaatjeplan.
   * Klik het pictogram van het onderzoekspictogram ![ Onderzoek ](assets/search-icon.png) en onderzoek naar een taak van het oudermalplaatje door naam.

   De sjabloontaak moet in de lijst worden weergegeven.

1. Selecteer het keuzerondje voor het bovenliggende element nadat u het hebt gevonden.

   Als u geen taak van het oudermalplaatje selecteert, worden de malplaatjetaken verplaatst als belangrijkste malplaatjetaken eerder dan subtasks en zij worden geplaatst aan het eind van de lijst van de malplaatjetaak op het bestemmingsmalplaatje.

1. Klik **de Taak van het Malplaatje van de Beweging**.

   De verplaatste sjabloontaken bevinden zich nu op de opgegeven sjabloon en zijn subtaken voor de geselecteerde bovenliggende sjabloontaak of de laatste sjabloontaken voor de sjabloon.
