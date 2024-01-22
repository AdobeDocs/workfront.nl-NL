---
product-area: projects
navigation-topic: convert-issues
title: Een uitgave converteren naar een project in Adobe Workfront
description: Een uitgave converteren naar een project in Adobe Workfront
author: Alina
feature: Work Management
exl-id: e3ba15a3-6169-466c-9912-32a8afdcc68d
source-git-commit: 71d5e15c38b26b9a833ac2418d5782afd249a24c
workflow-type: tm+mt
source-wordcount: '1927'
ht-degree: 0%

---

# Een uitgave converteren naar een project in Adobe Workfront

<!--Audited: 01/2024-->

Als meer werk moet worden gedaan om een kwestie te voltooien nadat de kwestie wordt voorgelegd, kunt u de kwestie in een project omzetten.

U kunt een uitgave in een nieuw project omzetten of u kunt het in een project omzetten gebruikend een malplaatje. Dit artikel beschrijft beide manieren om kwesties in projecten om te zetten.

>[!IMPORTANT]
>
>Voor algemene informatie over conversieproblemen raden we u aan ook het artikel te lezen [Overzicht van conversie van problemen in Adobe Workfront](../../../manage-work/issues/convert-issues/convert-issues.md).

Wanneer het creëren van een project van een kwestie, bevolken sommige gebieden op het project van andere voorwerpen. Voor meer informatie, zie de &quot;Nieuwe project standaardmontages&quot;sectie in het artikel [Een project maken](../../../manage-work/projects/create-projects/create-project.md).

## Toegangsvereisten

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
   <td role="rowheader">Adobe Workfront-licentie*</td> 
   <td> <p>Nieuw: Standaard </p>
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

*Neem contact op met uw Workfront-beheerder om te weten te komen welk abonnement, licentietype of toegang u hebt. Zie voor meer informatie [Toegangsvereisten in Workfront-documentatie](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

## Een uitgave converteren naar een project

U kunt een uitgave in een leeg project omzetten.

1. Ga naar een project en klik op **[!UICONTROL Issues]** in het linkerdeelvenster.
1. Voer een van de volgende handelingen uit in de lijst met weergegeven problemen:

   * Als u een uitgave wilt omzetten in een leeg project, klikt u op de naam van de uitgave en klikt u op de knop **[!UICONTROL More]** menu ![](assets/more-icon.png) rechts van de naam van de uitgave klikt u op **[!UICONTROL Convert to a blank project]**.


     of

     Selecteer de uitgave in de lijst met uitgaven en klik op de knop **[!UICONTROL More]** menu ![](assets/more-icon.png) boven aan de lijst klikt u op **[!UICONTROL Convert to a blank project]**.

     >[!IMPORTANT]
     >
     >De Omzetten in een lege projectoptie toont slechts wanneer uw systeem of groepsbeheerder toeliet [!UICONTROL Allow users to create projects without using a template] voorkeur in [!UICONTROL Setup] gebied. Zie voor meer informatie [Projectvoorkeuren voor het hele systeem configureren](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).


     U moet taken aan het project manueel toevoegen of een malplaatje vastmaken aan het project nadat u de kwestie omzet.

     >[!TIP]
     >   
     >* Als de kwestie gebruikend een verzoekrij werd gecreeerd, erft het nieuwe project de Groep van de verzoekrij.
     >* Als de kwestie door het toe te voegen aan de sectie van Kwesties van het project werd gecreeerd, erft het nieuwe project de Groep van het project van de kwestie.

     >[!TIP]
     >
     >Als het probleem is gekoppeld aan een goedkeuringsproces of al is gekoppeld aan een oplossend object, geeft Workfront boven aan het vak Converteren naar project een waarschuwing weer om aan te geven dat de goedkeuring wordt verwijderd of dat het oplossende object tijdens de conversie wordt overschreven. Zie voor meer informatie [Overzicht van conversie van problemen in Adobe Workfront](../../../manage-work/issues/convert-issues/convert-issues.md).

1. (Optioneel en voorwaardelijk) Klik op [!UICONTROL **Opties**] in het linkerdeelvenster selecteert u een van de beschikbare opties:

   * [!UICONTROL **Behoud de oorspronkelijke kwestie en koppel zijn resolutie aan dit project**]

     Wanneer deze optie is uitgeschakeld, wordt de oorspronkelijke uitgave verwijderd.

     >[!NOTE]
     >
     >Gebruikers zonder toegang of machtigingen om problemen te verwijderen, kunnen de uitgave niet verwijderen omdat ze deze converteren, ongeacht de status van deze instelling. Voor informatie over toegang en toestemmingen tot kwesties, zie:
     >
     >* [Toegang verlenen tot kwesties](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-issues.md)
     > 
     >* [Een uitgave delen](../../../workfront-basics/grant-and-request-access-to-objects/share-an-issue.md)

   * [!UICONTROL **(Gebruikersnaam) toegang verlenen tot dit project**]

     Als deze optie niet is geselecteerd, wordt de uitgave [!UICONTROL Primary Contact] heeft geen toegang tot de nieuwe taak.

     >[!NOTE]
     >
     >Welke opties hier beschikbaar zijn, is afhankelijk van de manier waarop de Workfront-beheerder deze voor iedereen in het systeem of voor uw groep heeft geconfigureerd. Zie voor meer informatie [Taak- en probleemvoorkeuren voor het hele systeem configureren](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md).
     >
     >
     >Of, als de top-level groepen in uw organisatie hen afzonderlijk vormden, hangen de beschikbare opties hier af van welke groep u voor het nieuwe project in stap 6 selecteerde. Zie voor meer informatie [Taak- en uitgavevoorkeuren voor een groep configureren](../../../administration-and-setup/manage-groups/create-and-manage-groups/configure-task-issue-preferences-group.md).

1. Klikken [!UICONTROL **Aangepaste Forms**] en voer een van de volgende handelingen uit:

   * Bekijk de aangepaste formulieren die aan de uitgave zijn gekoppeld. Zij zullen naar het nieuwe project, als zij ook projectdouaneformulieren zijn overbrengen.
   * Meer aangepaste formulieren toevoegen
   * Controleer of alle vereiste velden geldige gegevens bevatten.
   * De aangepaste formulieren opnieuw rangschikken door deze te slepen ![](assets/drag-object-icon.png) waar je ze wilt.
   * Klik op de knop **x** rechts van een formulier dat u niet naar het project wilt overbrengen. Hiermee verwijdert u het formulier uit het project.
   * Indien nodig, breng de informatie van de douaneformulier van de kwestie aan het project over.

     >[!TIP]
     >
     >* Als een multi-objecten douaneformulier in bijlage aan de kwestie voor gebruik met zowel kwesties als projecten wordt gevormd, wordt alle informatie bewaard die in de vorm wordt opgeslagen wanneer u de omzetting maakt als de gebieden zowel op de kwestie als de douaneformulieren van het project bestaan.
     >* Als een aangepast formulier met meerdere objecten en een berekend veld is gekoppeld aan zowel de uitgave als het project, moeten de uitgave en het project compatibel zijn met alle velden waarnaar wordt verwezen in de berekende aangepaste velden van het formulier. Als er sprake is van incompatibiliteit, wordt u gewaarschuwd dat u aanpassingen moet aanbrengen. Zie de sectie &quot;Berekende aangepaste velden in aangepaste formulieren voor meerdere objecten&quot; in het dialoogvenster [Berekende gegevens toevoegen aan een aangepast formulier met de oudere formulierbuilder](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-calculated-data-to-custom-form.md).

1. Klikken [!UICONTROL **Omzetten in project**].

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
1. Klikken [!UICONTROL **Omzetten in project**].

   De uitgave wordt nu omgezet in een project. De vertoningen van de projectpagina.

## Een uitgave converteren naar een project met behulp van een sjabloon

U kunt een uitgave in een project omzetten gebruikend een malplaatje.

1. Ga naar een project en klik op **[!UICONTROL Issues]** in het linkerdeelvenster.
1. Klik in de lijst met weergegeven uitgaven op de naam van de uitgave, klik op de knop **[!UICONTROL More]** menu ![](assets/more-icon.png) rechts van de naam van de uitgave klikt u op **Converteren naar project vanuit sjabloon** en typ de naam van een sjabloon in het dialoogvenster **Zoeksjabloon** klikt u vervolgens op de naam van de sjabloon wanneer deze in de lijst wordt weergegeven. Ga verder met stap 3.

   >[!TIP]
   >
   >Als u sjablonen hebt toegevoegd aan de lijst Favorieten, kunt u de muis boven de knop [!UICONTROL **Favoriete sjablonen**] en klik op de sjabloon die u wilt gebruiken.

   Het vak Nieuw project van sjabloon wordt weergegeven.

   ![](assets/new-project-from-template-small-box-with-template-details-panel-nwe-350x279.png)

   >[!TIP]
   >
   >* Als het probleem is gekoppeld aan een goedkeuringsproces of al is gekoppeld aan een oplossend object, geeft Workfront boven aan het vak Converteren naar project een waarschuwing weer om aan te geven dat de goedkeuring wordt verwijderd of dat het oplossende object tijdens de conversie wordt overschreven. Zie voor meer informatie [Overzicht van conversie van problemen in Adobe Workfront](../../../manage-work/issues/convert-issues/convert-issues.md).
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

1. (Optioneel) Plaats de muisaanwijzer op de naam van een sjabloon en klik op de knop **Favorieten** pictogram ![](assets/favorites-icon-small.png) om het als favoriet voor toekomstig gebruik te merken.

   >[!TIP]
   >
   >Je kunt maximaal 40 Workfront-objecten als favorieten laten markeren. Dit omvat sjablonen en andere items.

1. Klikken [!UICONTROL **Sjabloon gebruiken**] om een sjabloon te selecteren.

   De [!UICONTROL Convert to Project] wordt geopend.

   ![](assets/convert-to-project-from-template-large-project-box-nwe-350x291.png)

1. Als een veld al in de sjabloon is ingevuld, wordt het veld vooraf ingevuld in het dialoogvenster [!UICONTROL Convert to project] doos. U kunt de vooraf ingevulde waarden bewerken zodat deze beter overeenkomen met uw project. Zie voor meer informatie [Projecten bewerken](../../../manage-work/projects/manage-projects/edit-projects.md).

   >[!TIP]
   >
   >* Uw systeem- of groepsbeheerder kan velden toevoegen aan of verwijderen uit de [!UICONTROL Convert to Project box] door de projectdetails in uw [!UICONTROL Layout Template].
   >
   >* Als u velden wilt bijwerken in het dialoogvenster [!UICONTROL Finance] in de [!UICONTROL Convert to Project] vak moet u hebben [!UICONTROL Edit] toegang tot [!UICONTROL Financial Data] in uw toegangsniveau. Als u [!UICONTROL View] toegang tot [!UICONTROL Financial Data] in uw toegangsniveau alle financiële informatie van de malplaatjeoverdrachten aan het nieuwe project en u kunt niet het uitgeven terwijl u de kwestie omzet. Zie voor meer informatie [Toegang tot financiële gegevens verlenen](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md) en [Een sjabloon delen](../../../workfront-basics/grant-and-request-access-to-objects/share-a-template.md).

1. (Optioneel en voorwaardelijk) Klik op [!UICONTROL **Opties**] in het linkerdeelvenster selecteert u een van de beschikbare opties:

   * [!UICONTROL **Behoud de oorspronkelijke kwestie en koppel zijn resolutie aan dit project**]

     Wanneer deze optie is uitgeschakeld, wordt de oorspronkelijke uitgave verwijderd.

     >[!NOTE]
     >
     >Gebruikers zonder toegang of machtigingen om problemen te verwijderen, kunnen de uitgave niet verwijderen omdat ze deze converteren, ongeacht de status van deze instelling. Voor informatie over toegang en toestemmingen tot kwesties, zie:
     >
     >* [Toegang verlenen tot kwesties](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-issues.md)
     > 
     >* [Een uitgave delen](../../../workfront-basics/grant-and-request-access-to-objects/share-an-issue.md)

   * [!UICONTROL **(Gebruikersnaam) toegang verlenen tot dit project**]

     Als deze optie niet is geselecteerd, wordt de uitgave [!UICONTROL Primary Contact] heeft geen toegang tot de nieuwe taak.

     >[!NOTE]
     >
     >Welke opties hier beschikbaar zijn, is afhankelijk van de manier waarop de Workfront-beheerder deze voor iedereen in het systeem of voor uw groep heeft geconfigureerd. Zie voor meer informatie [Taak- en probleemvoorkeuren voor het hele systeem configureren](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md).
     >
     >
     >Of, als de top-level groepen in uw organisatie hen afzonderlijk vormden, hangen de beschikbare opties hier af van welke groep u voor het nieuwe project in stap 6 selecteerde. Zie voor meer informatie [Taak- en uitgavevoorkeuren voor een groep configureren](../../../administration-and-setup/manage-groups/create-and-manage-groups/configure-task-issue-preferences-group.md).

   1. Klikken [!UICONTROL **Aangepaste Forms**] en voer een van de volgende handelingen uit:

      * Bekijk de aangepaste formulieren die aan de sjabloon zijn gekoppeld. Zij zullen worden overgedragen naar het nieuwe project.
      * Bekijk de aangepaste formulieren die aan de uitgave zijn gekoppeld. Zij zullen naar het project worden overgedragen als het ook projectvormen zijn.
      * Controleer of alle vereiste velden geldige gegevens bevatten.
      * De aangepaste formulieren opnieuw rangschikken door deze te slepen ![](assets/drag-object-icon.png) waar je ze wilt.
      * Klik op de knop **x** rechts van een formulier dat u niet naar het project wilt overbrengen.
      * Indien nodig, breng de informatie van de douaneformulier van de kwestie aan het project over.

        >[!TIP]
        >
        >* Als een multi-objecten douaneformulier in bijlage aan de kwestie voor gebruik met zowel kwesties als projecten wordt gevormd, wordt alle informatie bewaard die in de vorm wordt opgeslagen wanneer u de omzetting maakt als de gebieden zowel op de kwestie als de douaneformulieren van het project bestaan.
        >* Als een aangepast formulier met meerdere objecten en een berekend veld is gekoppeld aan zowel de uitgave als het project, moeten de uitgave en het project compatibel zijn met alle velden waarnaar wordt verwezen in de berekende aangepaste velden van het formulier. Als er sprake is van incompatibiliteit, wordt u gewaarschuwd dat u aanpassingen moet aanbrengen. Zie de sectie &quot;Berekende aangepaste velden in aangepaste formulieren voor meerdere objecten&quot; in het dialoogvenster [Berekende gegevens toevoegen aan een aangepast formulier met de oudere formulierbuilder](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-calculated-data-to-custom-form.md).
        >* Als een aangepast formulier dat aan de sjabloon is gekoppeld, een aangepast veld bevat dat ook wordt gevonden in een aangepast formulier dat aan de uitgave is gekoppeld, wordt de veldwaarde van de uitgave gebruikt voor het nieuwe project. Als het aangepaste veld echter leeg is in de uitgave, wordt de waarde uit de sjabloon gebruikt.

1. (Optioneel) Stel desgewenst verdere projectdetails &#x200B; (eigenaar van project, projectdatums) en taken in.

   1. Klikken [!UICONTROL **Omzetten in project**].

      >[!TIP]
      >
      >Als u hebt besloten om de originele uitgave te verwijderen, is de kwestie nu een project.
      >   
      >of
      >  
      >Als u besloot om de oorspronkelijke uitgave te behouden, is de kwestie nu verbonden met het nieuwe project en het zal voltooien wanneer het project voltooit.
      >
      >Sommige probleemgebieden worden overgedragen naar het project. De meeste die gebieden in het malplaatje worden bepaald brengen automatisch naar het nieuwe gecreeerde project over als u hen in vorige stappen niet veranderde. Zie voor meer informatie [Overzicht van conversie van problemen in Adobe Workfront](../../../manage-work/issues/convert-issues/convert-issues.md).

   De uitgave wordt nu omgezet in een project. De vertoningen van de projectpagina.