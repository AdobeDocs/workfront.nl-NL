---
title: Een afbeeldings- of andere middelenwidget toevoegen of bewerken in een aangepast formulier met de verouderde formulierbuilder
description: U kunt de eigenschappen van de volgende widgets voor elementen, zoals afbeeldingen, video's, PDF-bestanden en Adobe XD-bestanden, toevoegen of bewerken in een aangepast formulier. Dit is handig wanneer u visuele inhoud wilt opnemen, zoals brandingafbeeldingen, een instructievideo of een interactief prototype voor een app die u ontwerpt.
author: Lisa
feature: System Setup and Administration, Custom Forms
role: Admin
exl-id: 62a2f9a1-80de-40e7-9d8b-46ed9df083c1
source-git-commit: d32f274390f6ffc5fdd01c2c9b4b2abd99d7cb10
workflow-type: tm+mt
source-wordcount: '1345'
ht-degree: 0%

---

# Een afbeeldings- of andere middelenwidget toevoegen of bewerken in een aangepast formulier met de verouderde formulierbuilder

{{form-designer-default}}

U kunt de eigenschappen van een van de volgende widgets voor elementen toevoegen of bewerken in een aangepast formulier:

* Afbeelding
* Video
* PDF-bestand
* Adobe XD-bestand

Dit is handig wanneer u visuele inhoud wilt opnemen, zoals brandingafbeeldingen, een instructievideo of een interactief prototype voor een app die u ontwerpt.

Wanneer een aangepast formulier met een widget aan een object is gekoppeld, kunnen gebruikers die met het object werken dit in de volgende gebieden zien:

* Het gebied van Details van het voorwerp (bijvoorbeeld, voor een project, het gebied van de Details van het Project)
* Het vak Bewerken voor het object als dit de nieuwe Adobe Workfront-ervaring bevat die er uitziet (bijvoorbeeld de vakken Project bewerken en Taak bewerken)

Gebruikers kunnen de widget momenteel niet zien in de volgende gebieden: &#x200B;

* Lijsten en rapporten
* Home en overzicht
* Het vak Bewerken voor het object, als dit object er anders uitziet dan de nieuwe Adobe Workfront-ervaring (bijvoorbeeld het vak Kosten bewerken)
* De Workfront Mobile-toepassing


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
   <td>Plan</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">Configuraties op toegangsniveau*</td> 
   <td> <p>Administratieve toegang tot aangepaste formulieren</p> <p>Voor informatie over hoe de beheerders van Workfront deze toegang verlenen, zie <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md" class="MCXref xref"> gebruikers administratieve toegang verlenen tot bepaalde gebieden </a>.</p> </td> 
  </tr>  
 </tbody> 
</table>

&#42; om te weten te komen welk plan, vergunningstype, of configuraties van het toegangsniveau u hebt, contacteer uw beheerder van Workfront.

## Een middelenwidget toevoegen of bewerken in een aangepast formulier

1. Begin werkend aan een douanevorm, zoals die in [ wordt beschreven creeer of geef een douanevorm ](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md) uit.
1. Met **voeg een gebied** open lusje toe, doe één van het volgende:

   * Als u een nieuwe widget toevoegt, uitgezochte **Beeld**, **PDF**, of **Video** om het bij de bodem van de vorm toe te voegen, of het te slepen waar u het op de vorm wilt.

     ![](assets/add-widget.png)


   * Als u een widget wilt toevoegen die reeds aan een andere douanevorm is toegevoegd, klik **bibliotheek van het Gebied**, dan klik de naam van widget in de lijst die toont. Voor meer informatie, zie [ een douanegebied of widget in een douanevorm ](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/reuse-an-existing-field.md) opnieuw gebruiken.

   * Als u een widget bewerkt die al aan het aangepaste formulier is toegevoegd, selecteert u deze.

1. Typ of bewerk een van de volgende eigenschappen voor de widget:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Label</td> 
      <td> <p>(Vereist) Typ een beschrijvend label dat boven de widget moet worden weergegeven. U kunt het label op elk gewenst moment wijzigen.</p> <p><b> BELANGRIJK </b>: Gebruik geen speciale karakters in dit etiket. Ze worden niet correct weergegeven in rapporten.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Naam</td> 
      <td> <p>(Vereist) Met deze naam wordt de widget door het systeem geïdentificeerd.</p> <p>Wanneer u de widget voor het eerst configureert en u typt het label, wordt het veld Naam automatisch aangepast. Maar de gebieden van het Etiket en van de Naam zijn niet gesynchroniseerd-dit geeft u de vrijheid om het etiket te veranderen dat uw gebruikers zien zonder het moeten de naam veranderen die het systeem ziet.</p> <p><b> BELANGRIJK </b>: Alhoewel het mogelijk is dit te doen, adviseren wij dat u deze naam niet verandert nadat u of andere gebruikers beginnen de douanevorm in widget te gebruiken. Als u dat doet, herkent het systeem de widget niet meer waar er nu naar kan worden verwezen in andere gebieden van Workfront. </p> <p>Elke widgetnaam moet uniek zijn in het Workfront-exemplaar van uw organisatie. Op deze manier kunt u een formulier hergebruiken dat al voor een ander aangepast formulier is gemaakt. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">URL</td> 
      <td> <p>(Vereist) Typ of plak de URL van de widget waar deze op internet is opgeslagen.</p> 
       <p><strong> Belangrijk </strong>: URL voor moet een openbare URL zijn. </p>
      <p>Als u een videowidget toevoegt, kunt u dit op dit moment doen door het volgende toe te voegen in het vak URL:</p> 
      <ul> 
      <li> <p>YouTube- of Vimeo-koppeling</p> </li> 
      <li> <p>Video-koppeling Google Drive</p> </li> 
      <li> <p>Koppeling maken naar video met MP4- en MOV-extensie</p> </li> 
      <li> <p>Koppeling maken naar video die al is geüpload naar het gebied Documenten in uw Workfront-instantie. Voor instructies, zie <a href="#add-a-video-widget-to-a-custom-form-from-the-documents-area" class="MCXref xref"> een video widget aan een douanevorm van het gebied van Documenten </a> in dit artikel toevoegen.</p> 
      </li> 
      </ul> 
       </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Instructies</td> 
      <td> <p>Typ eventuele aanvullende informatie over de widget. Wanneer gebruikers het aangepaste formulier invullen, kunnen ze de muisaanwijzer boven het pictogram van het vraagteken plaatsen om knopinfo weer te geven met de informatie die u hier typt.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Grootte</td> 
      <td>Wijzig desgewenst de weergavegrootte van de widget.</td> 
     </tr> 
    </tbody> 
   </table>

1. Klik **toepassen**.
1. Als u uw aangepaste formulier op andere manieren wilt blijven bouwen, gaat u verder naar een van de volgende artikelen:

   * [ de douanegebieden en widgets van de Positie in een douanevorm ](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/position-fields-in-a-custom-form.md)
   * [ voeg een douanegebied aan een douanevorm ](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-a-custom-field-to-a-custom-form.md) toe
   * [ hergebruik een douanegebied of widget in een douanevorm ](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/reuse-an-existing-field.md)
   * [ voeg berekende gegevens aan een douanevorm toe ](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-calculated-data-to-custom-form.md)
   * [ hergebruik een bestaand berekend douanegebied in een douanevorm ](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/use-existing-calc-field-new-custom-form.md)
   * [ voeg vertoningslogica toe en overslaat logica aan een douanevorm ](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/display-or-skip-logic-custom-form.md)
   * [Een aangepast formulier voorvertonen en invullen](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/preview-and-complete-a-custom-form.md)


## Een XD toevoegen aan een aangepast formulier

1. Begin werkend aan een douanevorm, zoals die in [ wordt beschreven creeer of geef een douanevorm ](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md) uit.
1. Met **voeg een gebied** open lusje toe, uitgezochte **Adobe XD**.
1. Typ of bewerk een van de volgende eigenschappen voor de widget:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Label</td> 
      <td> <p>(Vereist) Typ een beschrijvend label dat boven de widget moet worden weergegeven. U kunt het label op elk gewenst moment wijzigen.</p> <p><b> BELANGRIJK </b>: Gebruik geen speciale karakters in dit etiket. Ze worden niet correct weergegeven in rapporten.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Naam</td> 
      <td> <p>(Vereist) Met deze naam wordt de widget door het systeem geïdentificeerd.</p> <p>Wanneer u de widget voor het eerst configureert en u typt het label, wordt het veld Naam automatisch aangepast. Maar de gebieden van het Etiket en van de Naam zijn niet gesynchroniseerd-dit geeft u de vrijheid om het etiket te veranderen dat uw gebruikers zien zonder het moeten de naam veranderen die het systeem ziet.</p> <p><b> BELANGRIJK </b>: Alhoewel het mogelijk is dit te doen, adviseren wij dat u deze naam niet verandert nadat u of andere gebruikers beginnen de douanevorm in widget te gebruiken. Als u dat doet, herkent het systeem de widget niet meer waar er nu naar kan worden verwezen in andere gebieden van Workfront. </p> <p>Elke widgetnaam moet uniek zijn in het Workfront-exemplaar van uw organisatie. Op deze manier kunt u een formulier hergebruiken dat al voor een ander aangepast formulier is gemaakt. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">URL</td> 
      <td> <p>(Vereist) Typ of plak een geldige XD prototypekoppeling.</p> 
      <p>Opmerking: de instelling Koppelingstoegang op het tabblad Delen in Adobe XD moet zijn ingesteld op Iedereen met de koppeling. Anders kunnen gebruikers het prototype niet bekijken. 
   </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Instructies</td> 
      <td> <p>(Optioneel) Typ aanvullende informatie over de widget. Wanneer gebruikers het aangepaste formulier invullen, kunnen ze de muisaanwijzer boven het pictogram van het vraagteken plaatsen om knopinfo weer te geven met de informatie die u hier typt.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Grootte</td> 
      <td>(Optioneel) Wijzig desgewenst de weergavegrootte van de widget.</td> 
     </tr> 
    </tbody> 
   </table>

1. Als u uw aangepaste formulier op andere manieren wilt blijven bouwen, gaat u verder naar een van de volgende artikelen:

   * [ de douanegebieden en widgets van de Positie in een douanevorm ](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/position-fields-in-a-custom-form.md)
   * [ voeg een douanegebied aan een douanevorm ](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-a-custom-field-to-a-custom-form.md) toe
   * [ hergebruik een douanegebied of widget in een douanevorm ](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/reuse-an-existing-field.md)
   * [ voeg berekende gegevens aan een douanevorm toe ](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-calculated-data-to-custom-form.md)
   * [ hergebruik een bestaand berekend douanegebied in een douanevorm ](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/use-existing-calc-field-new-custom-form.md)
   * [ voeg vertoningslogica toe en overslaat logica aan een douanevorm ](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/display-or-skip-logic-custom-form.md)
   * [Een aangepast formulier voorvertonen en invullen](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/preview-and-complete-a-custom-form.md)

## Een videowidget toevoegen aan een aangepast formulier vanuit het gebied Documenten {#add-a-video-widget-to-a-custom-form-from-the-documents-area}

>[!IMPORTANT]
>
>Wanneer u op deze manier een video toevoegt aan een aangepast formulier, gelden alleen de machtigingen die voor het aangepaste formulier zijn ingesteld voor de video wanneer gebruikers het formulier openen op een object, niet de machtigingen die voor de video in het gebied Documenten zijn ingesteld.

1. Ga naar de video in het gebied van Documenten en produceer een proef voor het, zoals die in [ wordt beschreven creeer een interactieve proef voor een website of andere Webinhoud ](../../../review-and-approve-work/proofing/creating-proofs-within-workfront/generate-interactive-proof-for-website-or-other-web-content.md).
1. Open de proefdruk.
1. Klik overal op de video met de rechtermuisknop aan, dan selecteer **VideoAdres van het Exemplaar**.
1. In de douanevorm waar u video widget toevoegt, kleef het gekopieerde adres in de **URL** doos.
