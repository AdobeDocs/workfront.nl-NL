---
title: Een aanvraagformulier maken en beheren in Adobe Workfront-planning
description: Nadat u een recordtype hebt geselecteerd in het gedeelte Adobe Workfront Planning, kunt u een aanvraagformulier maken en dit koppelen aan dat recordtype. Vervolgens kunt u een koppeling naar de koppeling delen met andere interne of externe gebruikers. Gebruikers met een koppeling naar het formulier kunnen de veldwaarden erin invullen en door deze te verzenden, kunnen zij een nieuwe record toevoegen voor het bijbehorende recordtype.
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
exl-id: 49f25b03-90bb-4317-9e48-289fd61df791
source-git-commit: 9debb7c6d9df0f9f4962f3e66f146e5f605d20f0
workflow-type: tm+mt
source-wordcount: '1237'
ht-degree: 0%

---

# Een aanvraagformulier maken en beheren in Adobe Workfront Planning

<!--update the metadata with real information when making this available in TOC and in the left nav-->

{{planning-important-intro}}

U kunt een aanvraagformulier maken en dit koppelen aan een recordtype in Adobe Workfront Planning. Vervolgens kunt u een koppeling naar de koppeling delen met andere interne of externe gebruikers.

Gebruikers met een koppeling naar het formulier kunnen de veldwaarden erop bijwerken en nieuwe records toevoegen door het formulier te verzenden.

In dit artikel wordt beschreven hoe een werkruimtebeheerder een aanvraagformulier kan maken dat is gekoppeld aan een recordtype.

Voor informatie over het voorleggen van een verzoek aan een verslagtype om een verslag tot stand te brengen, zie [ de Verzoeken van de Planning van Adobe Workfront voorleggen om verslagen ](/help/quicksilver/planning/requests/submit-requests.md) tot stand te brengen.

## Toegangsvereisten

+++ Breid uit om de toegangseisen voor de functionaliteit in dit artikel weer te geven.

U moet de volgende toegang hebben om de stappen in dit artikel uit te voeren:

<table style="table-layout:auto">
 <col>
 </col>
 <col>
 </col>
 <tbody>
    <tr>
<tr>
<td>
   <p> Producten</p> </td>
   <td>
   <ul><li><p> Adobe Workfront</p></li>
   <li><p> Adobe Workfront Planning<p></li></ul></td>
  </tr>  
 <tr>
   <td role="rowheader"><p>Adobe Workfront-abonnement*</p></td>
   <td>
<p>Een van de volgende Workfront-plannen:</p>
<ul><li>Selecteren</li>
<li>Eerste</li>
<li>Ultieme</li></ul>
<p>Workfront Planning is niet beschikbaar voor oudere Workfront-plannen</p>
   </td>

<tr>
   <td role="rowheader"><p>Planning van Adobe Workfront*</p></td>
   <td>
<p>Alle </p>  
<p>Neem contact op met uw Workfront-accountmanager voor meer informatie over wat er in elk Workfront-planningsplan is opgenomen. </td>

<tr>
   <td role="rowheader"><p>Adobe Workfront-platform</p></td>
   <td>
<p>Het geval van Workfront van uw organisatie moet aan de Adobe Verenigde Ervaring worden genegeerd om tot alle mogelijkheden van de Planning van Workfront te kunnen toegang hebben.</p>
<p>Voor meer informatie, zie <a href="/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md"> Adobe Verenigde Ervaring voor Workfront </a>. </p>
   </td>

</tr>
  </tr>
  <tr>
   <td role="rowheader"><p>Adobe Workfront-licentie*</p></td>
   <td>
   <p>Standaard</p>
   <p>Workfront Planning is niet beschikbaar voor oudere Workfront-licenties</p>
  </td>
  </tr>
  <tr>
   <td role="rowheader"><p>Configuratie op toegangsniveau</p></td>
   <td> <p>Er zijn geen toegangsniveaucontroles voor de Planning van Adobe Workfront</p>  
</td>
  </tr>
<tr>
   <td role="rowheader"><p>Objectmachtigingen</p></td>
   <td>
   <ul>
   <li><p>Machtigingen beheren in een werkruimte</p></li>
    <li><p>Systeembeheerders kunnen werkruimten beheren die ze niet hebben gemaakt. </p></li>
    </ul>
   <p>Voor informatie over het delen van machtigingen voor Workfront Planning-objecten raadpleegt u  
   <a href="/help/quicksilver/planning/access/sharing-permissions-overview.md"> Overzicht van het delen van toestemmingen in de Planning van Adobe Workfront </a> 
  </td>
  </tr>
<tr>
   <td role="rowheader"><p>Lay-outsjabloon</p></td>
   <td> <p>Aan alle gebruikers, inclusief Workfront-beheerders, moet een lay-outsjabloon worden toegewezen die het planningsgebied in het hoofdmenu bevat. </p>  
</td>
  </tr>
 </tbody>
</table>

*Voor meer informatie over de toegangsvereisten van Workfront, zie [ vereisten van de Toegang in de documentatie van Workfront ](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Een aanvraagformulier maken voor een recordtype

{{step1-to-planning}}

1. Klik op de werkruimte waar u records wilt toevoegen.

   De werkruimte wordt geopend en de recordtypen worden als kaarten weergegeven.

1. Klik op een opnametype. Voor informatie over het creëren van een verslagtype, zie [ recordtypes ](/help/quicksilver/planning/architecture/create-record-types.md) creëren.

   De pagina met recordtypen wordt geopend in de weergave die u het laatst hebt geopend. Standaard wordt een pagina met recordtypen geopend in de tabelweergave.

1. Klik **Meer** menu ![](assets/more-menu.png) aan het recht van het verslagtype naam in de paginakop, dan klik **creeer verzoekvorm**.
1. Werk de naam van het aanvraagformulier bij. Door gebrek, is de naam van de vorm **Naamloze verzoekvorm**. <!--check this; you logged a bug to rename it to this but was it fixed?-->
1. (Facultatief) voeg a **Beschrijving** voor de verzoekvorm toe.

   <!--Not possible yet: The Description is visible when you access the request form from the Requests area of Workfront.-->

1. Klik **creëren**. Het aanvraagformulier voor het geselecteerde recordtype wordt geopend.

   ![](assets/campaigns-request-form-edit-mode.png)

   Het aanvraagformulier bevat standaard de volgende informatie:

   * De gebieden van het verslag beschikbaar in de lijstmening van het geselecteerde verslagtype. <!--they are working on removing the limitation below-->

     >[!IMPORTANT]
     >
     >   Velden van de volgende typen worden niet weergegeven in het aanvraagformulier:
     >
     >    * Personen (inclusief Gemaakt door en Laatst gewijzigd door)
     >    * Verbonden velden (bevat verbindingen met Workfront en Experience Manager-elementen)
     >    * Verbonden opzoekvelden
     >    * Formule
     >    * Aanmaakdatum
     >    * Laatst gewijzigd

   * **Standaard sectie**: Dit is de standaardsectieonderbreking die Workfront op de verzoekvorm van toepassing is. De standaardsectie kan niet worden anders genoemd of worden verwijderd.
   * **Onderwerp** gebied: Het gebied dat het verzoek in Workfront zal identificeren. Deze mogelijkheid is nog niet beschikbaar. De configuratie en de waarde van het onderwerpveld kunnen niet worden bewerkt.
   * Alle velden die aan het recordtype zijn gekoppeld.

     De velden in het aanvraagformulier zijn zichtbaar voor iedereen die een aanvraag naar dit recordtype indient.

1. (Optioneel) Houd de muisaanwijzer boven alle velden in het formulier die u wilt verwijderen en klik vervolgens op het pictogram **x** om deze te verwijderen. Zij worden toegevoegd aan het **lusje van Gebieden** links van de vorm.

   Bijvoorbeeld, verwijder het **Onderwerp** gebied, aangezien dit niet in de Planning van Workfront zichtbaar is. <!--remove this step when we connect intake with the Requests area in Workfront-->
1. Klik op een veld en gebruik vervolgens de besturingselementen in het rechterdeelvenster van het formulier om de grootte van het veld te definiëren, of een van de volgende gegevens:

   * **Etiket**: dit is de naam van het gebied aangezien het op de verzoekvorm zal verschijnen. Hiermee wijzigt u de naam van het recordveld niet.
   * **Instructies**: Voeg meer informatie over het gebied toe.
   * **maak een vereist gebied**: Wanneer geselecteerd, moet het gebied een waarde hebben. Anders kan het formulier niet worden verzonden.
   * **voegt logica** toe: Bepaal welke voorwaarden moeten worden voldaan opdat het gebied tonen of verborgen zijn.

   >[!NOTE]
   >
   >   Het veldtype van elk veld wordt boven in het rechtervenster weergegeven, nadat u het veld op het formulier hebt geselecteerd.
   >   
   >
   >   De velden Valuta, Nummer en Percentage worden weergegeven als een tekstveldtype voor één regel. De veldindeling blijft echter behouden en de waarden binnen deze velden worden weergegeven als de waarden Valuta, Nummer en Percentage.

1. (Facultatief) klik de **elementen van de Inhoud** tabel op de linkerkant van de vorm, en voeg om het even welke volgende elementen toe:

   * **Beschrijvende tekst**
   * **Sectieonderbreking**

   Voor meer informatie over de bouw van een douanevorm, zie [ Ontwerp een vorm met de vormontwerper ](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md).

1. (Facultatief) klik **Voorproef** om te bekijken hoe de vorm voor andere gebruikers zal tonen wanneer zij het zullen gebruiken om een nieuw verslag voor te leggen.
1. Klik **Publish** om de vorm te publiceren en een unieke verbinding voor het te verkrijgen.

   De volgende dingen doen zich voor:

   * De Publish-knop wordt verwijderd.
   * De **unpublish** knoop wordt toegevoegd aan de vorm. Als u erop klikt, is het formulier niet toegankelijk.
   * A **de knoop van het Aandeel** wordt toegevoegd aan de vorm.

1. Klik **Aandeel** om de vorm met anderen te delen.

   ![](assets/share-box-for-request-form.png)

1. Selecteer een van de volgende opties om aan te geven welke typen gebruikers toegang hebben tot dit formulier:

   * Iedereen met weergave of hogere toegang tot de werkruimte
   * Iedereen met een hogere of hogere toegang tot de werkruimte
   * Iedereen met de koppeling

   >[!IMPORTANT]
   >
   >Wanneer u **iedereen met de verbinding** selecteert, kan iedereen tot de vorm toegang hebben en een nieuw verslag voorleggen, zelfs mensen buiten uw organisatie die geen rekening van Workfront hebben.

1. (Voorwaardelijk) als u **Iedereen met de verbinding** in de vorige stap selecteerde, selecteer de **vervaldatum van de Verbinding** van de beschikbare kalender. Personen ontvangen een fout nadat de koppeling is verlopen en u moet de datum van de koppeling bijwerken voordat ze het formulier weer kunnen openen.

   U kunt toekomstige datums selecteren binnen 180 dagen vanaf de huidige datum.

1. Klik **sparen en kopieer verbinding** om de het delen details voor de vorm te bewaren.

   De opties voor het delen van formulieren worden opgeslagen en de koppeling wordt naar het klembord gekopieerd. U kunt deze nu delen met anderen.

   Voor informatie over het creëren van verslagen die een verbinding aan een verzoekvorm gebruiken, zie [ verzoeken van de Planning van Adobe Workfront voorleggen ](/help/quicksilver/planning/requests/submit-requests.md).

1. Klik **sparen** in de laag-juiste hoek van het scherm om de vorm te bewaren.
1. Klik op de pijl die naar links wijst links van de naam van het formulier in de koptekst om het formulier te sluiten.

   De pagina met recordtypen wordt geopend.
1. (Facultatief) klik **Meer** menu ![](assets/more-menu.png) rechts van de naam van het verslagtype in de kopbal, dan doe één van het volgende:
   * Klik **de verzoekvorm van de Update** om het even welke veranderingen in de verzoekvorm aan te brengen.
   * Klik **verbinding van het Exemplaar aan de verzoekvorm** om de verbinding aan de vorm met anderen te delen.

   >[!TIP]
   >
   >Er zijn aanwijzingen dat de link in dit geval openbaar wordt gedeeld.
   >![](assets/publicly-shared-link-to-form-on-record-type-menu-highlighted.png)
