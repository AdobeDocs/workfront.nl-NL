---
product-area: projects;templates
navigation-topic: create-projects
title: Een project maken met een sjabloon
description: U kunt sjablonen als een framework gebruiken om projecten te maken in Adobe Workfront. Als u projecten hebt die vaak herhalen, bewaart het gebruiken van malplaatjes voor het nieuwe project u van het moeten de zelfde projecten herhaaldelijk bouwen.
author: Alina
feature: Work Management
exl-id: 622cbfe0-b8c0-4045-bef2-9e21d45bfda0
source-git-commit: 5cb07cb42c3264c6629bc0a038c0e70ffc2cb509
workflow-type: tm+mt
source-wordcount: '1131'
ht-degree: 0%

---

# Een project maken met een sjabloon

<!-- Audited: 01/2024 -->

U kunt sjablonen als een framework gebruiken om projecten te maken in Adobe Workfront. Als u projecten hebt die vaak herhalen, bewaart het gebruiken van malplaatjes voor de algemene chronologie van het nieuwe project u van het moeten de zelfde projecten herhaaldelijk bouwen.

De malplaatjes voorzien u van een manier om herhaalbare processen, informatie, en montages te vangen verbonden aan uw projecten. De informatie verbonden aan een malplaatje wordt overgebracht naar het project. Dit omvat taken, taken, duur, documenten, financiële details, risico&#39;s, en douaneformulieren.

>[!TIP]
>
>Workfront definieert de groep en status van het nieuwe project als volgt:
>
>* De standaardstatus van een nieuw project dat van een malplaatje wordt gecreeerd beantwoordt aan de status die door uw beheerder van Workfront in het belangrijkste gebied van de Voorkeur van het Project wordt bepaald, of door een groepsbeheerder (of beheerder van Workfront) in het gebied van de Voorkeur van het Project voor een groep. Voor informatie over het vormen van projectvoorkeur, zie [Projectvoorkeuren voor het hele systeem configureren](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md) of [Projectvoorkeuren voor een groep configureren](../../../administration-and-setup/manage-groups/create-and-manage-groups/configure-project-preferences-group.md).
>
>* De Groep van het nieuwe project is de Groep van het malplaatje. Als het malplaatje niet met een Groep wordt geassocieerd, dan is de Groep van het project de Groep van het Huis van de gebruiker die tot het project leidt.
>
>* De statussen beschikbaar voor een nieuw project passen de statussen van de Groep van het project aan, die of de Groep van het malplaatje, of de Groep van het Huis van de gebruiker is die tot het project leidt.

U hebt de volgende opties voor het maken van een project op basis van een sjabloon:

* Creeer een project van een malplaatje in het gebied van Projecten
* Een project maken op basis van een sjabloon op sjabloonniveau
* Een sjabloon aan een bestaand project koppelen

  Zie voor meer informatie [Een sjabloon aan een project koppelen](../../../manage-work/projects/create-and-manage-templates/attach-template-to-project.md).

* Een project maken van een sjabloon in het gebied Groepen

## Toegangsvereisten

+++ Breid uit om de toegangseisen voor de functionaliteit in dit artikel weer te geven.

<!--drafted for P&P:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan*</td> 
   <td> <p>Any </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Workfront license*</td> 
   <td> <p>Current license: Standard </p>
   Or
   <p>Legacy license: Plan </p>
    </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>Edit access to Projects and to Templates</p> <p><b>NOTE</b>
   
   If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information about access to projects, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-projects.md" class="MCXref xref">Grant access to projects</a>. For information on how a Workfront administrator can change your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>View permissions to a template</p> <p>When you create a project you automatically receive Manage permissions to the project </p> <p> For information about project permissions, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/share-a-project.md" class="MCXref xref">Share a project in Adobe Workfront</a>.</p> <p>For information on requesting additional access, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>
-->

U moet de volgende toegang hebben om de stappen in dit artikel uit te voeren:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-plan</td> 
   <td> <p>Alle </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Workfront-licentie</td> 
   <td> <p>Nieuw: Standaard</p>
        <p>of</p>
        <p>Huidig: Plan </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraties op toegangsniveau</td> 
   <td> <p>Toegang tot projecten en sjablonen bewerken</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objectmachtigingen</td> 
   <td> <p>Machtigingen weergeven voor een sjabloon</p> <p>Wanneer u een project creeert, ontvangt u automatisch Manage toestemmingen aan het project.</p></td> 
  </tr> 
 </tbody> 
</table>

Zie voor meer informatie over de informatie in deze tabel [Toegangsvereisten in Workfront-documentatie](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Creeer een project van een malplaatje in het gebied van Projecten

U kunt een project van het gebied van Projecten in het Belangrijkste Menu, of van het gebied van Projecten van een portefeuille of een programma tot stand brengen.

>[!NOTE]
>
>Uw systeem of groepsbeheerder zou uw interface kunnen wijzigen gebruikend een lay-outmalplaatje. In dit geval kunnen sommige namen van de secties en gebieden waarnaar in de volgende stappen wordt verwezen, anders zijn in uw exemplaar van Workfront.

1. Voer een van de volgende handelingen uit:

   * Klik op de knop **[!UICONTROL Main Menu]** pictogram ![Hoofdmenu](/help/_includes/assets/main-menu-icon.png) in de rechterbovenhoek van Adobe Workfront of (indien beschikbaar) op de knop **[!UICONTROL Main Menu]** pictogram ![Hoofdmenu](/help/_includes/assets/main-menu-icon-left-nav.png) in de linkerbovenhoek Klikken **Projecten** vervolgens uitvouwen **Nieuw project**.
   * Naar een portfolio gaan en vervolgens uitvouwen **Nieuw project**.

     >[!TIP]
     >
     >Wanneer u een project gebruikend een malplaatje van een portefeuille creeert, werkt het gebied van het Portfolio van het nieuwe project bij om de portefeuille te tonen u verkoos om het project tot stand te brengen van. Hiermee wordt het veld Portfolio in de sjabloon overschreven, als dit is opgegeven.

   * Naar een programma gaan en vervolgens uitvouwen **Nieuw project**.

     >[!TIP]
     >
     >Wanneer u een project gebruikend een malplaatje van een programma creeert, werkt het gebied van het Programma van de nieuwe projecten bij om het Programma te tonen u verkoos om het project van tot stand te brengen. Het gebied van het Portfolio van het malplaatje werkt bij om de portefeuille van het programma te tonen u verkoos om het project van tot stand te brengen. Hiermee overschrijft u de velden Programma en Portfolio in de sjabloon, als deze zijn opgegeven.

   * Als u een groepsbeheerder bent, kunt u een project in de sectie van Projecten van een groep ook tot stand brengen u beheert. Zie voor meer informatie [Projecten van een groep maken en wijzigen](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-projects.md).

     >[!TIP]
     >
     >Wanneer u een project gebruikend een malplaatje van een groep creeert, de groep u het project van vertoningen op het gebied van de Groep van het nieuwe project creeert slechts wanneer het gebied van de Groep van het malplaatje niet wordt gespecificeerd. Als het gebied van de malplaatjegroep wordt gespecificeerd, is het gebied van de Groep van het nieuwe project dat van het malplaatje.

   <!--
   <p>(this, above, is hyperlinked to the classic version of this article; the Milestone View steps are similar to creating a project in Classic than to the way you do it in NWE)</p>
   -->

   ![Nieuwe projectopties](assets/new-project-dropdown.png)

1. Klik op de naam van een sjabloon in het dialoogvenster **Favoriete sjablonen** lijst.

   ![Een favoriete sjabloon selecteren](assets/new-project-from-template-dropdown-with-template-favorites.png)

   of

   Ga als volgt te werk:

   1. Selecteren **Nieuw project van sjabloon**.
   1. In de **Sjablonen zoeken** , typt u de naam van een sjabloon en klikt u erop wanneer de sjabloon in de lijst wordt weergegeven.
   1. Bekijk de sjabloondetails aan de rechterkant.

      De sjabloondetails bevatten onder meer de volgende informatie:

      * Sjabloonduur
      * Eigenaar van sjabloon
      * Het aantal taken op hoofdniveau, die de namen van de drie belangrijkste taken omvat
      * Het aantal taken in de sjabloon
      * De namen van de aangepaste sjabloonformulieren

   1. (Optioneel) Houd de muisaanwijzer boven de naam van een sjabloon in het linkervenster en klik op de knop **Favorieten** **pictogram** ![](assets/favorites-icon-small.png) om het als favoriet voor toekomstig gebruik te merken.

      of

      Breid uit **Favoriete sjablonen** en selecteer een sjabloon in de vervolgkeuzelijst.

      >[!TIP]
      >
      >Je kunt maximaal 40 Workfront-objecten als favorieten laten markeren. Dit omvat sjablonen en andere items.

   1. Klikken **Sjabloon gebruiken** als u een sjabloon hebt geselecteerd.

      ![Sjabloondetails](assets/new-project-from-template-small-box-with-template-details-panel.png)

      >[!NOTE]
      >
      >Als u de mening van de Mijlpaal hebt toegepast op de lijst van projecten, klik de naam van een malplaatje in **Nieuw vanuit gedeelte Sjabloon**.
      >
      >
      >![De mening van de mijlpaal van het creëren van een project van een malplaatje](assets/create-project-from-template-box-from-milestone-view-nwe-350x275.png)
      >

   De **Nieuw project** wordt geopend.

   ![Nieuw projectvak](assets/new-project-from-template-box.png)

1. Als een veld al in de sjabloon is ingevuld, wordt het veld vooraf ingevuld in het dialoogvenster **Nieuw project** doos. U kunt de vooraf ingevulde waarden bewerken zodat deze beter overeenkomen met uw project. Zie voor meer informatie [Projecten bewerken](../../../manage-work/projects/manage-projects/edit-projects.md).
1. Klikken **Project maken**.

   Alle details die in het malplaatje worden bepaald associëren automatisch met het pas gecreëerde project als u hen in de vorige stap niet veranderde.

## Een project maken van een sjabloon in het gebied Sjablonen

In plaats van in het gebied van Projecten te beginnen, kunt u een project van een malplaatje tot stand brengen door met het malplaatje te beginnen.

{{step1-to-templates}}

1. Klik op de naam van een sjabloon die u wilt gebruiken.
1. Klik op de knop **Meer** menu ![](assets/more-icon.png)en klik vervolgens op **Project maken**.

   ![Project maken van sjabloon](assets/project-sharing-on-template.png)

   De **Nieuw project** wordt geopend.

1. Ga een naam voor het project in, herzie dan elke sectie en breng om het even welke noodzakelijke veranderingen aan.

   ![Nieuw projectvak](assets/new-project-from-template-box.png)

   Als een veld al in de sjabloon is ingevuld, wordt het veld vooraf ingevuld in het dialoogvenster **Nieuw project** doos. U kunt de vooraf ingevulde waarden bewerken zodat deze beter overeenkomen met uw project. Zie voor meer informatie [Projecten bewerken](../../../manage-work/projects/manage-projects/edit-projects.md).

1. Klikken **Project maken**.

   Alle details die in het malplaatje worden bepaald associëren automatisch met het pas gecreëerde project als u hen in de vorige stap niet veranderde.
