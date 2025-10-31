---
product-area: projects;templates
navigation-topic: create-projects
title: Een project maken met een sjabloon
description: U kunt sjablonen als een framework gebruiken om projecten te maken in Adobe Workfront. Als u projecten hebt die vaak herhalen, bewaart het gebruiken van malplaatjes voor het nieuwe project u van het moeten de zelfde projecten herhaaldelijk bouwen.
author: Alina
feature: Work Management
exl-id: 622cbfe0-b8c0-4045-bef2-9e21d45bfda0
source-git-commit: 76379d5433cc13ee412c8c1045316ef253b3ee7d
workflow-type: tm+mt
source-wordcount: '1146'
ht-degree: 0%

---

# Een project maken met een sjabloon

<!-- Audited: 10/2025 -->

U kunt sjablonen als een framework gebruiken om projecten te maken in Adobe Workfront. Als u projecten hebt die vaak herhalen, bewaart het gebruiken van malplaatjes voor de algemene chronologie van het nieuwe project u van het moeten de zelfde projecten herhaaldelijk bouwen.

De malplaatjes voorzien u van een manier om herhaalbare processen, informatie, en montages te vangen verbonden aan uw projecten. De informatie verbonden aan een malplaatje wordt overgebracht naar het project. Dit omvat taken, taken, duur, documenten, financiële details, risico&#39;s, en douaneformulieren.

>[!TIP]
>
>Workfront definieert de groep en status van het nieuwe project als volgt:
>
>* De standaardstatus van een nieuw project dat van een malplaatje wordt gecreeerd beantwoordt aan de status die door uw beheerder van Workfront in het belangrijkste gebied van de Voorkeur van het Project wordt bepaald, of door een groepsbeheerder (of beheerder van Workfront) in het gebied van de Voorkeur van het Project voor een groep. Voor informatie over het vormen van projectvoorkeur, zie [&#x200B; systeem-brede projectvoorkeur &#x200B;](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md) vormen of [&#x200B; projectvoorkeur voor een groep &#x200B;](../../../administration-and-setup/manage-groups/create-and-manage-groups/configure-project-preferences-group.md) vormen.
>
>* De Groep van het nieuwe project is de Groep van het malplaatje. Als het malplaatje niet met een Groep wordt geassocieerd, dan is de Groep van het project de Groep van het Huis van de gebruiker die tot het project leidt.
>
>* De statussen beschikbaar voor een nieuw project passen de statussen van de Groep van het project aan, die of de Groep van het malplaatje, of de Groep van het Huis van de gebruiker is die tot het project leidt.

U hebt de volgende opties voor het maken van een project op basis van een sjabloon:

* Creeer een project van een malplaatje in het gebied van Projecten
* Een project maken op basis van een sjabloon op sjabloonniveau
* Een sjabloon aan een bestaand project koppelen

  Voor informatie, zie [&#x200B; een malplaatje aan een project &#x200B;](../../../manage-work/projects/create-and-manage-templates/attach-template-to-project.md) vastmaken.

* Een project maken van een sjabloon in het gebied Groepen

## Toegangsvereisten

+++ Breid uit om de toegangseisen voor de functionaliteit in dit artikel weer te geven.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-pakket</td> 
   <td> <p>Alle</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Workfront-licentie</td> 
   <td> <p>Standard</p>
        <p>Plan</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuratie op toegangsniveau</td> 
   <td> <p>Toegang tot projecten en sjablonen bewerken</p>
   <p>Toegang tot portfolio's en programma's bewerken als de sjabloon die u gebruikt een Portfolio en een programma bevat</p>  
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objectmachtigingen</td> 
   <td> <p>Machtigingen weergeven voor een sjabloon</p> 
  <p>Als de sjabloon die u gebruikt een Portfolio en een programma bevat, moet u beheerdersmachtigingen voor het portfolio en programma hebben om het project te maken </p> 
   <p>Wanneer u een project creeert, ontvangt u automatisch Manage toestemmingen aan het project.</p></td> 
  </tr> 
 </tbody> 
</table>

Voor meer informatie, zie [&#x200B; vereisten van de Toegang in de documentatie van Workfront &#x200B;](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

<!--Old:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan</td> 
   <td> <p>Any </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Workfront license*</td> 
   <td> <p>New: Standard</p>
        <p>or</p>
        <p>Current: Plan </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level</td> 
   <td> <p>Edit access to Projects and to Templates</p>
   
   <p>edit access to Portfolios and Programs, if the template you use contains a Portfolio and a Program</p>
   
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>View permissions to a template</p> 
  <p>If the template you use contains a Portfolio and a Program, you must have Manage permissions to the portfolio and program to create the project </p> 
   <p>When you create a project, you automatically receive Manage permissions to the project.</p></td> 
  </tr> 
 </tbody> 
</table>-->

## Creeer een project van een malplaatje in het gebied van Projecten

U kunt een project van het gebied van Projecten in het Belangrijkste Menu, of van het gebied van Projecten van een portefeuille of een programma tot stand brengen.

>[!NOTE]
>
>Uw systeem of groepsbeheerder zou uw interface kunnen wijzigen gebruikend een lay-outmalplaatje. In dit geval kunnen sommige namen van de secties en gebieden waarnaar in de volgende stappen wordt verwezen, anders zijn in uw exemplaar van Workfront.

1. Voer een van de volgende handelingen uit:

   * Klik het **[!UICONTROL Main Menu]** pictogram ![&#x200B; Belangrijkste Menu &#x200B;](/help/_includes/assets/main-menu-icon-left-nav.png) in de upper-left hoek, of het **[!UICONTROL Main Menu]** pictogram ![&#x200B; Belangrijkste Menu &#x200B;](/help/_includes/assets/main-menu-icon.png) in de hoger-juiste hoek van Adobe Workfront, als beschikbaar, dan klik **Projecten** en breid **Nieuw Project** uit.
   * Ga naar een portefeuille, dan breid **Nieuw Project** uit.

     >[!TIP]
     >
     >Wanneer u een project gebruikend een malplaatje van een portefeuille creeert, werkt het gebied van Portfolio van het nieuwe project bij om de portefeuille te tonen u verkoos om het project van tot stand te brengen. Hiermee wordt het Portfolio-veld op de sjabloon overschreven, als dit is opgegeven.

   * Ga naar een programma, dan breid **Nieuw Project** uit.

     >[!TIP]
     >
     >Wanneer u een project gebruikend een malplaatje van een programma creeert, werkt het gebied van het Programma van de nieuwe projecten bij om het Programma te tonen u verkoos om het project van tot stand te brengen. Het Portfolio-veld van de sjabloon wordt bijgewerkt en geeft het portfolio weer van het programma waarmee u het project hebt gemaakt. Hiermee worden de velden Programma en Portfolio in de sjabloon overschreven, als deze zijn opgegeven.

   * Als u een groepsbeheerder bent, kunt u een project in de sectie van Projecten van een groep ook tot stand brengen u beheert. Voor meer informatie, zie [&#x200B; tot stand brengen en wijzigen de projecten van een groep &#x200B;](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-projects.md).

     >[!TIP]
     >
     >Wanneer u een project gebruikend een malplaatje van een groep creeert, de groep u het project van vertoningen op het gebied van de Groep van het nieuwe project creeert slechts wanneer het gebied van de Groep van het malplaatje niet wordt gespecificeerd. Als het gebied van de malplaatjegroep wordt gespecificeerd, is het gebied van de Groep van het nieuwe project dat van het malplaatje.

   <!--
   <p>(this, above, is hyperlinked to the classic version of this article; the Milestone View steps are similar to creating a project in Classic than to the way you do it in NWE)</p>
   -->

   ![&#x200B; Nieuwe opties van het Project &#x200B;](assets/new-project-dropdown.png)

1. Klik de naam van een malplaatje in de **Favoriete malplaatjes** lijst.

   ![&#x200B; selecteer een favoriet malplaatje &#x200B;](assets/new-project-from-template-dropdown-with-template-favorites.png)

   of

   Ga als volgt te werk:

   1. Klik **Nieuw Project van Malplaatje**.
   1. Op het **gebied van de Malplaatjes van het Onderzoek**, begin de naam van een malplaatje te typen en het te klikken wanneer het in de lijst toont.
   1. Bekijk de sjabloondetails aan de rechterkant.

      De sjabloondetails bevatten onder meer de volgende informatie:

      * Sjabloonduur
      * Eigenaar van sjabloon
      * Het aantal taken op hoofdniveau, die de namen van de drie belangrijkste taken omvat
      * Het aantal taken in de sjabloon
      * De namen van de aangepaste sjabloonformulieren

   1. (Facultatief) Beweeg over de naam van een malplaatjenaam in de linkerruit en klik de **Favorieten** **pictogram** ![&#x200B; pictogram van Favorieten &#x200B;](assets/favorites-icon-small.png) om het als favoriet voor toekomstig gebruik te merken.

      of

      Breid de **Favoriete malplaatjes** lijst uit en selecteer een malplaatje van de drop-down lijst.

      >[!TIP]
      >
      >Je kunt maximaal 40 Workfront-objecten als favorieten laten markeren. Dit omvat sjablonen en andere items.

   1. Klik **malplaatje van het Gebruik** wanneer u een malplaatje hebt geselecteerd.

      ![&#x200B; de details van het Malplaatje &#x200B;](assets/new-project-from-template-small-box-with-template-details-panel.png)

      <!--no longer available, after unshimming - Oct 2025:
      >[!NOTE]
      >
      >If you have the Milestone View applied to the list of projects, click the name of a template in the **New from Template section**.
      >
      >
      >![Milestone view of creating a project from a template](assets/create-project-from-template-box-from-milestone-view-nwe-350x275.png)
      >
      -->

   Het **Nieuwe vakje van het Project** opent.

   ![&#x200B; Nieuwe doos van het Project &#x200B;](assets/new-project-from-template-box.png)

1. (Voorwaardelijk) als een gebied reeds in het malplaatje bevolkt is, is het gebied pre-bevolkt in de **Nieuwe doos van het Project**.

   Bewerk de vooraf ingevulde waarden om deze beter aan te passen aan uw project.

   Voor meer informatie, zie [&#x200B; projecten &#x200B;](../../../manage-work/projects/manage-projects/edit-projects.md) uitgeven.
1. Klik **tot project** leiden.

   Alle details die in het malplaatje worden bepaald associëren automatisch met het pas gecreëerde project als u hen in de vorige stap niet veranderde.

## Een project maken van een sjabloon in het gebied Sjablonen

In plaats van in het gebied van Projecten te beginnen, kunt u een project van een malplaatje tot stand brengen door met het malplaatje te beginnen.

{{step1-to-templates}}

1. Klik op de naam van een sjabloon die u wilt gebruiken.
1. Klik het **Meer** menu ![&#x200B; Meer pictogram &#x200B;](assets/more-icon.png) aan het recht van de malplaatjenaam in de kopbal, dan klik **leidt tot Project**.

   ![&#x200B; creeer project van malplaatje &#x200B;](assets/project-sharing-on-template.png)

   Het **Nieuwe vakje van het Project** opent.

1. Voer een naam in voor het project. Workfront gebruikt de naam van de sjabloon om het nieuwe project een naam te geven.

1. Herzie elke sectie in het **Nieuwe vakje van het Project** en breng om het even welke noodzakelijke veranderingen aan.

   ![&#x200B; Nieuwe doos van het Project &#x200B;](assets/new-project-from-template-box.png)

   Als een gebied reeds in het malplaatje bevolkt is, is het gebied pre-bevolkt in het **Nieuwe vakje van het Project**. U kunt de vooraf ingevulde waarden bewerken zodat deze beter overeenkomen met uw project.

   Voor informatie, zie [&#x200B; projecten &#x200B;](../../../manage-work/projects/manage-projects/edit-projects.md) uitgeven.

1. Klik **tot project** leiden.

   Alle details die in het malplaatje worden bepaald associëren automatisch met het pas gecreëerde project als u hen in de vorige stap niet veranderde.
