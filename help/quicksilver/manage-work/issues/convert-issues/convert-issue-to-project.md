---
product-area: projects
navigation-topic: convert-issues
title: Een uitgave converteren naar een project in Adobe Workfront
description: Een uitgave converteren naar een project in Adobe Workfront
author: Alina
feature: Work Management
exl-id: e3ba15a3-6169-466c-9912-32a8afdcc68d
source-git-commit: 71ddeb83543c3c1491a412ac18deaa3ce1077c21
workflow-type: tm+mt
source-wordcount: '1966'
ht-degree: 0%

---

# Een uitgave converteren naar een project in Adobe Workfront

<!--Audited: 01/2024-->

Als meer werk moet worden gedaan om een kwestie te voltooien nadat de kwestie wordt voorgelegd, kunt u de kwestie in een project omzetten.

U kunt een uitgave in een nieuw project omzetten of u kunt het in een project omzetten gebruikend een malplaatje. Dit artikel beschrijft beide manieren om kwesties in projecten om te zetten.

>[!IMPORTANT]
>
>Voor algemene informatie over het omzetten van kwesties, adviseren wij dat u ook het artikel [&#x200B; Overzicht van het omzetten van kwesties in Adobe Workfront &#x200B;](../../../manage-work/issues/convert-issues/convert-issues.md) leest.

Wanneer het creëren van een project van een kwestie, bevolken sommige gebieden op het project van andere voorwerpen. Voor meer informatie, zie de &quot;Nieuwe sectie van het projectgebrek montages&quot;in het artikel [&#x200B; een project &#x200B;](../../../manage-work/projects/create-projects/create-project.md) creëren.

## Toegangsvereisten

+++ Breid uit om de toegangseisen voor de functionaliteit in dit artikel weer te geven.

U moet de volgende toegang hebben om de stappen in dit artikel uit te voeren:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-plan</td> 
   <td> <p>Alle</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-licentie</td> 
   <td>
   <p>Nieuw: Standaard </p> 
    <p>Huidig: Plan </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraties op toegangsniveau*</td> 
   <td> <p>Toegang tot problemen, taken en projecten bewerken</p> <p>Toegang tot financiële gegevens bewerken om financiële informatie bij te werken voor een geconverteerde versie van de uitgave</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objectmachtigingen</td> 
   <td> <p>Machtigingen weergeven voor de uitgave</p> <p>U krijgt beheermachtigingen voor het project nadat de uitgave is omgezet</p> </td> 
  </tr> 
 </tbody> 
</table>

Voor meer detail over de informatie in deze lijst, zie [&#x200B; vereisten van de Toegang in de documentatie van Workfront &#x200B;](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Overwegingen

* Er is een verwerkingsgrens van 5 minuten wanneer het omzetten van een kwestie in een project. Als er een groot aantal documenten aan de uitgave is gekoppeld en deze niet kan worden geconverteerd, moet u mogelijk enkele documenten verwijderen en het opnieuw proberen.

## Een uitgave converteren naar een project

U kunt een uitgave in een leeg project omzetten.

1. Ga naar een project en klik op **[!UICONTROL Issues]** in het linkerdeelvenster.
1. Voer een van de volgende handelingen uit in de lijst met weergegeven problemen:

   * Om een kwestie in een leeg project om te zetten, klik de naam van de kwestie, klik het **[!UICONTROL More]** menu ![&#x200B; Meer menu &#x200B;](assets/more-icon.png) rechts van de uitgevende naam, dan klik **[!UICONTROL Convert to a blank project]**.


     of

     Selecteer de kwestie in de lijst van kwestie, klik het **[!UICONTROL More]** menu ![&#x200B; Meer menu &#x200B;](assets/more-icon.png) bij de bovenkant van de lijst, dan klik **[!UICONTROL Convert to a blank project]**.

     >[!IMPORTANT]
     >
     >De optie Omzetten in een leeg project wordt alleen weergegeven wanneer uw systeem- of groepsbeheerder de voorkeur [!UICONTROL Allow users to create projects without using a template] heeft ingeschakeld in het [!UICONTROL Setup] -gebied. Voor meer informatie, zie [&#x200B; systeem-brede projectvoorkeur &#x200B;](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md) vormen.


     U moet taken aan het project manueel toevoegen of een malplaatje vastmaken aan het project nadat u de kwestie omzet.

     >[!TIP]
     >   
     >* Als de kwestie gebruikend een verzoekrij werd gecreeerd, erft het nieuwe project de Groep van de verzoekrij.
     >* Als de kwestie door het toe te voegen aan de sectie van Kwesties van het project werd gecreeerd, erft het nieuwe project de Groep van het project van de kwestie.

     >[!TIP]
     >
     >Als het probleem is gekoppeld aan een goedkeuringsproces of al is gekoppeld aan een oplossend object, geeft Workfront boven aan het vak Converteren naar project een waarschuwing weer om aan te geven dat de goedkeuring wordt verwijderd of dat het oplossende object tijdens de conversie wordt overschreven. Voor meer informatie, zie [&#x200B; Overzicht van het omzetten van kwesties in Adobe Workfront &#x200B;](../../../manage-work/issues/convert-issues/convert-issues.md).

1. (Facultatief en voorwaardelijk) klik [!UICONTROL **Opties**] in het linkerpaneel, dan selecteer van de opties die beschikbaar zijn:

   * [!UICONTROL **houd de originele kwestie en verbind zijn resolutie aan dit project**]

     Wanneer deze optie is uitgeschakeld, wordt de oorspronkelijke uitgave verwijderd.

     >[!NOTE]
     >
     >Gebruikers zonder toegang of machtigingen om problemen te verwijderen, kunnen de uitgave niet verwijderen omdat ze deze converteren, ongeacht de status van deze instelling. Voor informatie over toegang en toestemmingen tot kwesties, zie:
     >
     >* [&#x200B; de toegang van de Verlening tot kwesties &#x200B;](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-issues.md)
     > 
     >* [&#x200B; Deel een kwestie &#x200B;](../../../workfront-basics/grant-and-request-access-to-objects/share-an-issue.md)

   * [!UICONTROL **staat (de Naam van de Gebruiker) toe om toegang tot dit project te hebben**]

     Als deze optie niet is geselecteerd, heeft de uitgave [!UICONTROL Primary Contact] geen toegang tot de nieuwe taak.

     >[!NOTE]
     >
     >Welke opties hier beschikbaar zijn, is afhankelijk van de manier waarop de Workfront-beheerder deze voor iedereen in het systeem of voor uw groep heeft geconfigureerd. Voor meer informatie, zie [&#x200B; taak voor het hele systeem vormen en voorkeur uitgeven &#x200B;](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md).
     >
     >
     >Of, als de top-level groepen in uw organisatie hen afzonderlijk vormden, hangen de beschikbare opties hier af van welke groep u voor het nieuwe project in stap 6 selecteerde. Voor meer informatie, zie [&#x200B; taak vormen en uitgiftevoorkeur voor een groep &#x200B;](../../../administration-and-setup/manage-groups/create-and-manage-groups/configure-task-issue-preferences-group.md).

1. Klik [!UICONTROL **Forms van de Douane**] en doe om het even welke volgend:

   * Bekijk de aangepaste formulieren die aan de uitgave zijn gekoppeld. Zij zullen naar het nieuwe project, als zij ook projectdouaneformulieren zijn overbrengen.
   * Meer aangepaste formulieren toevoegen
   * Controleer of alle vereiste velden geldige gegevens bevatten.
   * Herschik de douanevormen door hen ![&#x200B; pictogram van de Belemmering &#x200B;](assets/drag-object-icon.png) te slepen waar u hen wilt.
   * Klik het **x** pictogram aan het recht van om het even welke vorm die u niet naar het project wilt overbrengen. Hiermee verwijdert u het formulier uit het project.
   * Indien nodig, breng de informatie van de douaneformulier van de kwestie aan het project over.

     >[!TIP]
     >
     >* Als een multi-objecten douaneformulier in bijlage aan de kwestie voor gebruik met zowel kwesties als projecten wordt gevormd, wordt alle informatie bewaard die in de vorm wordt opgeslagen wanneer u de omzetting maakt als de gebieden zowel op de kwestie als de douaneformulieren van het project bestaan.
     >* Als een aangepast formulier met meerdere objecten en een berekend veld is gekoppeld aan zowel de uitgave als het project, moeten de uitgave en het project compatibel zijn met alle velden waarnaar wordt verwezen in de berekende aangepaste velden van het formulier. Als er sprake is van incompatibiliteit, wordt u gewaarschuwd dat u aanpassingen moet aanbrengen. Voor meer informatie, zie de &quot;Berekende douanegebieden in multi-objecten douaneformulieren&quot;sectie in [&#x200B; berekende gebieden aan een vorm &#x200B;](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/add-a-calculated-field.md) toevoegen.

1. Klik [!UICONTROL **Bekeerling in project**].

   >[!TIP]
   >
   >Als u hebt besloten om de originele uitgave te verwijderen, is de kwestie nu een project.
   >   
   >of
   >  
   >Als u besloot om de oorspronkelijke uitgave te behouden, is de kwestie nu verbonden met het nieuwe project en het zal voltooien wanneer het project voltooit.
   >
   >De informatie in sommige gebieden van de uitgave gaat naar het project over, als u hen tijdens omzetting niet veranderde.

1. (Optioneel) Stel desgewenst verdere projectdetails &#x200B; (eigenaar van project, projectdatums) en taken in.
1. Klik [!UICONTROL **Bekeerling in project**].

   De uitgave wordt nu omgezet in een project. De vertoningen van de projectpagina.

## Een uitgave converteren naar een project met behulp van een sjabloon

U kunt een uitgave in een project omzetten gebruikend een malplaatje.

1. Ga naar een project en klik op **[!UICONTROL Issues]** in het linkerdeelvenster.
1. In de lijst van kwesties die toont, klik de naam van de kwestie, klik het **[!UICONTROL More]** menu ![&#x200B; Meer menu &#x200B;](assets/more-icon.png) rechts van de uitgevende naam, dan klik **Bekeerling aan project van Malplaatje** en begin de naam van een malplaatje in het **Sjabloon van het Onderzoek** vakje te typen, dan klik de naam van het malplaatje wanneer het in de lijst toont. Ga verder met stap 3.

   >[!TIP]
   >
   >Als u malplaatjes aan uw lijst van Favorieten toevoegde, kunt u muis over het [!UICONTROL **Favoriete malplaatjes**] menu en het malplaatje klikken u wilt gebruiken.

   Het vak Nieuw project van sjabloon wordt weergegeven.

   ![&#x200B; Nieuw project van malplaatje &#x200B;](assets/new-project-from-template-small-box-with-template-details-panel-nwe-350x279.png)

   >[!TIP]
   >
   >* Als het probleem is gekoppeld aan een goedkeuringsproces of al is gekoppeld aan een oplossend object, geeft Workfront boven aan het vak Converteren naar project een waarschuwing weer om aan te geven dat de goedkeuring wordt verwijderd of dat het oplossende object tijdens de conversie wordt overschreven. Voor meer informatie, zie [&#x200B; Overzicht van het omzetten van kwesties in Adobe Workfront &#x200B;](../../../manage-work/issues/convert-issues/convert-issues.md).
   >   
   >* Als de kwestie gebruikend een verzoekrij werd gecreeerd, erft het nieuwe project de Groep van de verzoekrij.
   >* Als de kwestie door het toe te voegen aan de sectie van Kwesties van het project werd gecreeerd, erft het nieuwe project de Groep van het project van de kwestie.

1. Bekijk de sjabloondetails rechts.

   De sjabloondetails bevatten onder meer de volgende informatie:

   * Sjabloonduur
   * Eigenaar van sjabloon
   * Het aantal taken op hoofdniveau dat de namen van de drie belangrijkste taken omvat
   * Het aantal taken in de sjabloon
   * De namen van de aangepaste sjabloonformulieren

1. (Facultatief) muis over de naam van een malplaatje en klik het **pictogram van Favorieten** ![&#x200B; om het als favoriet voor toekomstig gebruik te merken.](assets/favorites-icon-small.png)

   >[!TIP]
   >
   >Je kunt maximaal 40 Workfront-objecten als favorieten laten markeren. Dit omvat sjablonen en andere items.

1. Klik [!UICONTROL **malplaatje van het Gebruik**] om een malplaatje te selecteren.

   Het vak [!UICONTROL Convert to Project] wordt geopend.

   ![&#x200B; Bekeerling aan project &#x200B;](assets/convert-to-project-from-template-large-project-box-nwe-350x291.png)

1. Als een veld al in de sjabloon is ingevuld, wordt het veld vooraf ingevuld in het vak [!UICONTROL Convert to project] . U kunt de vooraf ingevulde waarden bewerken zodat deze beter overeenkomen met uw project. Voor meer informatie, zie [&#x200B; projecten &#x200B;](../../../manage-work/projects/manage-projects/edit-projects.md) uitgeven.

   >[!TIP]
   >
   >* Uw systeem- of groepsbeheerder kan velden toevoegen aan of verwijderen uit [!UICONTROL Convert to Project box] door de projectdetails in uw [!UICONTROL Layout Template] bij te werken.
   >
   >* Als u velden in de sectie [!UICONTROL Finance] in het vak [!UICONTROL Convert to Project] wilt bijwerken, moet u [!UICONTROL Edit] toegang hebben tot [!UICONTROL Financial Data] op toegangsniveau. Als u [!UICONTROL View] toegang tot [!UICONTROL Financial Data] in uw toegangsniveau hebt alle financiële informatie van de malplaatjeoverdrachten aan het nieuwe project en u kunt niet het uitgeven terwijl u de kwestie omzet. Voor informatie, zie [&#x200B; toegang van de Verlening tot financiële gegevens &#x200B;](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md) en [&#x200B; Deel een malplaatje &#x200B;](../../../workfront-basics/grant-and-request-access-to-objects/share-a-template.md).

1. (Facultatief en voorwaardelijk) klik [!UICONTROL **Opties**] in het linkerpaneel, dan selecteer van de opties die beschikbaar zijn:

   * [!UICONTROL **houd de originele kwestie en verbind zijn resolutie aan dit project**]

     Wanneer deze optie is uitgeschakeld, wordt de oorspronkelijke uitgave verwijderd.

     >[!NOTE]
     >
     >Gebruikers zonder toegang of machtigingen om problemen te verwijderen, kunnen de uitgave niet verwijderen omdat ze deze converteren, ongeacht de status van deze instelling. Voor informatie over toegang en toestemmingen tot kwesties, zie:
     >
     >* [&#x200B; de toegang van de Verlening tot kwesties &#x200B;](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-issues.md)
     > 
     >* [&#x200B; Deel een kwestie &#x200B;](../../../workfront-basics/grant-and-request-access-to-objects/share-an-issue.md)

   * [!UICONTROL **staat (de Naam van de Gebruiker) toe om toegang tot dit project te hebben**]

     Als deze optie niet is geselecteerd, heeft de uitgave [!UICONTROL Primary Contact] geen toegang tot de nieuwe taak.

     >[!NOTE]
     >
     >Welke opties hier beschikbaar zijn, is afhankelijk van de manier waarop de Workfront-beheerder deze voor iedereen in het systeem of voor uw groep heeft geconfigureerd. Voor meer informatie, zie [&#x200B; taak voor het hele systeem vormen en voorkeur uitgeven &#x200B;](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md).
     >
     >
     >Of, als de top-level groepen in uw organisatie hen afzonderlijk vormden, hangen de beschikbare opties hier af van welke groep u voor het nieuwe project in stap 6 selecteerde. Voor meer informatie, zie [&#x200B; taak vormen en uitgiftevoorkeur voor een groep &#x200B;](../../../administration-and-setup/manage-groups/create-and-manage-groups/configure-task-issue-preferences-group.md).

   1. Klik [!UICONTROL **Forms van de Douane**] en doe om het even welke volgend:

      * Bekijk de aangepaste formulieren die aan de sjabloon zijn gekoppeld. Zij zullen worden overgedragen naar het nieuwe project.
      * Bekijk de aangepaste formulieren die aan de uitgave zijn gekoppeld. Zij zullen naar het project worden overgedragen als het ook projectvormen zijn.
      * Controleer of alle vereiste velden geldige gegevens bevatten.
      * Herschik de douanevormen door hen ![&#x200B; pictogram van de Belemmering &#x200B;](assets/drag-object-icon.png) te slepen waar u hen wilt.
      * Klik het **x** pictogram aan het recht van om het even welke vorm die u niet naar het project wilt overbrengen.
      * Indien nodig, breng de informatie van de douaneformulier van de kwestie aan het project over.

        >[!TIP]
        >
        >* Als een multi-objecten douaneformulier in bijlage aan de kwestie voor gebruik met zowel kwesties als projecten wordt gevormd, wordt alle informatie bewaard die in de vorm wordt opgeslagen wanneer u de omzetting maakt als de gebieden zowel op de kwestie als de douaneformulieren van het project bestaan.
        >* Als een aangepast formulier met meerdere objecten en een berekend veld is gekoppeld aan zowel de uitgave als het project, moeten de uitgave en het project compatibel zijn met alle velden waarnaar wordt verwezen in de berekende aangepaste velden van het formulier. Als er sprake is van incompatibiliteit, wordt u gewaarschuwd dat u aanpassingen moet aanbrengen. Voor meer informatie, zie [&#x200B; berekende gebieden aan een vorm &#x200B;](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/add-a-calculated-field.md) toevoegen.
        >* Als een aangepast formulier dat aan de sjabloon is gekoppeld, een aangepast veld bevat dat ook wordt gevonden in een aangepast formulier dat aan de uitgave is gekoppeld, wordt de veldwaarde van de uitgave gebruikt voor het nieuwe project. Als het aangepaste veld echter leeg is in de uitgave, wordt de waarde uit de sjabloon gebruikt.

1. (Optioneel) Stel desgewenst verdere projectdetails &#x200B; (eigenaar van project, projectdatums) en taken in.

   1. Klik [!UICONTROL **Bekeerling in project**].

      >[!TIP]
      >
      >Als u hebt besloten om de originele uitgave te verwijderen, is de kwestie nu een project.
      >   
      >of
      >  
      >Als u besloot om de oorspronkelijke uitgave te behouden, is de kwestie nu verbonden met het nieuwe project en het zal voltooien wanneer het project voltooit.
      >
      >Sommige probleemgebieden worden overgedragen naar het project. De meeste die gebieden in het malplaatje worden bepaald brengen automatisch naar het nieuwe gecreeerde project over als u hen in vorige stappen niet veranderde. Voor informatie, zie [&#x200B; Overzicht van het omzetten van kwesties in Adobe Workfront &#x200B;](../../../manage-work/issues/convert-issues/convert-issues.md).

   De uitgave wordt nu omgezet in een project. De vertoningen van de projectpagina.
