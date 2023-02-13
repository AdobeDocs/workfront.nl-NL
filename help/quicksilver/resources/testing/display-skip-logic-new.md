---
title: Weergavelogica toevoegen en logica overslaan naar een aangepast formulier
description: Weergavelogica toevoegen en logica overslaan naar een aangepast formulier
draft: Probably
source-git-commit: c0722924d6621b382050a10e9aac549fc1204d72
workflow-type: tm+mt
source-wordcount: '1503'
ht-degree: 0%

---

# Weergavelogica toevoegen en logica overslaan naar een aangepast formulier

Met slimme regels kunt u een aangepast formulier dynamisch en relevanter maken voor de gebruikers die het invullen. Wanneer een gebruiker op een bepaalde manier reageert op een meerkeuzeveld op een formulier, wordt met een slimme regel aangegeven wat de gebruiker als volgende moet zien, op basis van dat antwoord.

De meerkeuzevelden zijn vervolgkeuzelijsten, selectievakjes en keuzerondjes.

* **Logica weergeven**: U vormt een regel van de vertoningslogica op het gebied, widget, of sectie die u de gebruiker wilt zien slechts nadat zij een specifieke keus in een voorafgaand meerkeuzeveld selecteren.

   **Voorbeeld:** U maakt een aanvraagformulier voor marketinginhoud waarin mensen in uw organisatie een nieuw logo, een nieuwe website-update, een brochure of andere soorten marketinginhoud kunnen aanvragen. Gebaseerd op type van inhoud die de gebruiker wil, moet u hen voor verschillende soorten details, zoals kleuren en ontwerpideeën vragen als zij een embleem, of een lijst van producteigenschappen nodig hebben als zij een brochure nodig hebben.

   In het veld waarin wordt gevraagd naar kleuren en details voor een nieuw logo, kunt u een regel voor weergavelogica toevoegen waarmee dat veld alleen wordt weergegeven nadat de gebruiker het keuzerondje Logo in het eerste veld heeft geselecteerd.

   Op dezelfde manier kunt u in het veld waarin u wordt gevraagd naar productfuncties, een regel voor weergavelogica toevoegen waarmee dat veld alleen wordt weergegeven nadat een gebruiker het keuzerondje Brochure in het eerste veld heeft geselecteerd.

   ![](assets/display-logic-logo-request-350x196.png)

   U kunt de regels van de vertoningslogica op om het even welk douanegebied, widget, of sectieonderbreking vormen die een meerkeuzeveld volgen.

* **Logische regel overslaan**: U configureert deze regel om delen van een formulier te verbergen die de gebruiker niet nodig heeft. Wanneer de gebruiker een specifiek item in een voorafgaand meerkeuzeveld selecteert, slaat de logicaregel voor overslaan deze over naar het einde van het formulier of naar een aangepast veld, een widget of een sectie die u wilt zien.

   **Voorbeeld:** Iemand gebruikt het bovenstaande formulier voor het aanvragen van marketinginhoud om te vragen om een witboek, dat wordt geleverd door Verkoop, niet door Marketing. Voor deze gebruiker, kan een overslaan logische regel de vraag verbergen die voor details ertoe aanzet en aan een lijn van tekst overslaan die hen verwijst naar de afdeling zij nodig hebben.

   ![](assets/skip-logic-white-paper-request-350x221.png)

   In dit geval kunt u een beschrijvend tekstveld toevoegen waarin de gebruiker naar de afdeling Verkoop verwijst. In het eerste aangepaste veld waarin wordt gevraagd welk type marketinginhoud de gebruiker nodig heeft, kunt u een logicaregel voor overslaan toevoegen die alleen de tekstregel weergeeft wanneer een gebruiker in het eerste veld het keuzerondje Witboek selecteert.

   Dit is vooral handig als u veel andere velden met logo&#39;s, updates van websites en brochures toevoegt die deze gebruiker niet hoeft te zien.
U kunt een logicaregel voor overslaan alleen toepassen op een aangepast veld, niet op een widget of sectie.

Voor informatie over aangepaste velden en widgets in aangepaste formulieren raadpleegt u [Een aangepast veld toevoegen aan een aangepast formulier](../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-a-custom-field-to-a-custom-form.md) en [Een middelenwidget toevoegen of bewerken in een aangepast formulier](../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-widget-or-edit-its-properties-in-a-custom-form.md).

## Toegangsvereisten

U moet het volgende hebben om de stappen in dit artikel uit te voeren:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr data-mc-conditions=""> 
   <td role="rowheader"> <p>Adobe Workfront-abonnement*</p> </td> 
   <td>Alle</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-licentie*</td> 
   <td> <p>Plan </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">Configuraties op toegangsniveau*</td> 
   <td> <p>Administratieve toegang tot aangepaste formulieren</p> <p>Ga voor informatie over hoe Workfront-beheerders deze toegang verlenen naar <a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md" class="MCXref xref">Gebruikers administratieve toegang verlenen tot bepaalde gebieden</a>.</p> </td> 
  </tr>  
 </tbody> 
</table>

&#42;Neem contact op met uw Workfront-beheerder om te weten te komen welk plan, type licentie of configuraties op toegangsniveau u hebt.

## Een voorbeeld van een aangepast formulier maken met weergave en logica overslaan

De beste manier om te leren hoe te om vertoning toe te voegen en logica aan een douaneformulier over te slaan is door het praktische voorbeeld dat in de twee volgende secties wordt verklaard:

* [Logica weergeven - praktisch voorbeeld](#display-logic-practical-example)
* [Logica overslaan - praktisch voorbeeld](#skip-logic-practical-example)

### Logica weergeven - praktisch voorbeeld {#display-logic-practical-example}

In dit voorbeeld maakt u een aangepast formulier met een meerkeuzerondje-veld. Vervolgens voegt u weergavelogica toe die dit veld verbindt met een tweede veld.

1. Klik op de knop **Hoofdmenu** pictogram ![](assets/main-menu-icon.png) in de rechterbovenhoek van Adobe Workfront klikt u op **Instellen** ![](assets/gear-icon-settings.png).

1. Selecteer in het linkerdeelvenster de optie **Aangepaste Forms** ![](assets/custom-forms-icon.png).

1. Klikken **Nieuw aangepast formulier**, selecteert u **Project** in het vak dat wordt weergegeven, selecteert u vervolgens **Doorgaan**.

1. In de **Formuliertitel** tekstvak, tekst **Aangepast voorbeeldformulier - Leren werken met weergavelogica en logica overslaan** om het formulier een naam te geven.

   ![](assets/form-title-box-350x247.png)

1. Het eerste veld toevoegen aan het formulier:

   1. Open de **Veld toevoegen** tab.

      ![](assets/add-a-field-tab-350x237.png)

   1. Selecteer **Keuzerondjes** veldtype, vervolgens typen *Welk type marketinginhoud hebt u nodig?* als de **Label** voor het veld.

   1. Onder **Keuzen** vervangen **Keuze 1** en **Keuze 2** met de volgende tekst om twee opties te maken kunnen gebruikers in het veld kiezen:

      *Website bijwerken*

      *Logoontwerp*

1. U voegt als volgt het volgende aangepaste veld toe en voegt er een regel met een weergaveregel aan toe:

   1. Open de **Veld toevoegen** opnieuw te openen en een nieuwe **Keuzerondjes** veld aangeroepen *Welk type update van website hebt u nodig?*

      De opties voor dit veld worden later toegevoegd.

   1. In de **Aanvullende instellingen** sectie, selecteert u **Logica toevoegen**.

      ![](assets/add-logic-btn-350x408.png)

1. In het vak dat wordt weergegeven, **Weergavelogica** het tweede veld zo configureren dat het alleen wordt weergegeven voor gebruikers die *Websites ontwerpen* in het eerste veld:

   1. Selecteer in het eerste vervolgkeuzemenu de optie **Welk type marketinginhoud hebt u nodig?**
   1. Selecteer in het tweede vervolgkeuzemenu de optie **Websites ontwerpen**.
   1. De derde vervolgkeuzelijst ingesteld op **Geselecteerd**, selecteert u **Opslaan**.

   Let op de kleine gekleurde vierkantjes met een D, waarmee wordt aangegeven dat het tweede veld is verbonden met weergavelogica aan de selectie van de gebruiker in het eerste veld:

   ![](assets/red-display-logic-indicators-350x250.png)

1. Selecteren **Voorvertoning** om ervoor te zorgen dat de logica werkt zoals u het op het formulier wilt, selecteert u **Voorvertoning beëindigen**.

1. Klikken **Opslaan + Sluiten** Sla het formulier op en ga vervolgens verder met [Logica overslaan - praktisch voorbeeld](#skip-logic-practical-example) hieronder.

### Logica overslaan - praktisch voorbeeld {#skip-logic-practical-example}

Logische functies overslaan werkt net als logica voor weergave, maar fungeert als omgekeerd: in plaats van specifieke aangepaste multikeuzelijsten weer te geven op basis van eerdere gebruikersselecties, bepaalt u welke velden moeten worden verborgen (overgeslagen), omdat ze niet relevant zijn voor de gebruiker.

U leert dit door te werken aan het voorbeeldformulier dat u in de sectie hebt gemaakt [Logica weergeven - praktisch voorbeeld](#display-logic-practical-example) in dit artikel.

1. Klik op de knop **Hoofdmenu** pictogram ![](assets/main-menu-icon.png) in de rechterbovenhoek van Adobe Workfront klikt u op **Instellen** ![](assets/gear-icon-settings.png).

1. Klikken **Aangepaste Forms**.
1. Klik op de naam van het formulier **Aangepast voorbeeldformulier - Leren werken met weergavelogica en logica overslaan** die u in de bovenstaande stappen hebt gemaakt, om deze te openen voor bewerking.
1. Selecteer het drop-down gebied u genoemde creeerde *Welk type website hebt u nodig?* voegt u de volgende opties voor het veld toe en klikt u op **Toepassen**:

   *E-handel*

   *Brochure*

   *Lidmaatschap*

1. Open de **Veld toevoegen** tabblad, maakt u een **Tekstveld met opmaak **veld genaamd *Wat is het doel van de website?* en klik vervolgens op **Toepassen**.

   In deze organisatie, wordt een de documentatieplaats van de Hulp gecreeerd door het Technisch schrijvende team, niet de afdeling van de Marketing. Er is dus geen verdere informatie nodig van een gebruiker die Help-documentatie selecteert in het tweede veld. Er wordt een tekstregel gemaakt (een beschrijvend tekstveld) waarmee ze het team voor technisch schrijven kunnen bekijken. En wij zullen een overslaan logische regel gebruiken die die gebruiker aan die lijn van tekst overslaat.

1. De tekstregel maken:

   1. Open de **Veld toevoegen** en maakt u een **Beschrijvende tekst, veld**.

   1. Voor de **Label**, type *Zie Technisch schrijvers team*.

   1. Voor de **Beschrijvende tekst**, type *Raadpleeg het team voor technisch schrijven over het maken van online Help-documentatie*.

   1. Selecteren **Toepassen**.

1. De logicaregel overslaan maken:

   1. Selecteer het tweede drop-down gebied, *Welk type website hebt u nodig?*
   1. In de **Aanvullende instelling** s sectie, selecteert u **Logica bewerken**.
   1. In de doos die toont, open **Logica overslaan** tab.
   1. Eerste vervolgkeuzelijst instellen op **Help-documentatie**, laat de tweede vervolgkeuzelijst ingesteld op **Geselecteerd** en stelt u de derde vervolgkeuzelijst in op **Zie het team voor technisch schrijven**.
   1. Selecteren **Opslaan**.

   Let op de kleine overslaan logische vierkantjes met een S die aangeven dat de gebruiker iets overslaat nadat een bepaalde keuze in het tweede veld is geselecteerd.

   ![](assets/notice-skip-logic-squares-350x249.png)

1. Klikken **Voorvertoning**  om ervoor te zorgen dat de logica op de gewenste manier wordt toegepast.
1. Klikken **Opslaan +Sluiten**.

Wanneer u een formulier als dit maakt, kunt u meer tekstvelden toevoegen om gebruikers te vragen informatie te vragen die in het tweede veld E-commerce of Brochure selecteren. Deze gebieden zouden kunnen vragen wie het doelpubliek voor de website is, wat het doel is om het te creëren, wat het budget is, enzovoort.

Met logische regels kunt u vertakkende vraagpaden maken.

Voor gebruikers die e-commerce selecteren, kunt u bijvoorbeeld velden maken met vragen over productfoto&#39;s, beschrijvingen, prijzen en betalingsopties. Voor gebruikers die Brochure selecteren, kunt u gebieden tot stand brengen vragend over inhoud.

Een gebruiker die Help-documentatie heeft geselecteerd, ziet geen van deze extra velden die voor hem of haar irrelevant zijn.

>[!TIP]
>
>U kunt zowel weergavelogica als logica overslaan aan een aangepast veld toevoegen als het volgende geldt voor het veld:
>
>* Het is een meerkeuzeveld (keuzerondjes, vervolgkeuzelijst of selectievakjes)
>* Voorafgegaan door een veld met meerdere keuzen
>* Het wordt gevolgd door een ander aangepast veld
>


<!--
<h2 data-mc-conditions="QuicksilverOrClassic.Draft mode">Multi-field display logic statements</h2>
-->

