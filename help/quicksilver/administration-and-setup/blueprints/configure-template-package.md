---
user-type: administrator
product-area: system-administration;workfront-integrations
navigation-topic: best-practices-catalog
title: Een blauwdruk configureren
description: U kunt details van het projectmalplaatje of de organisatorische structuur vormen alvorens u de blauwdruk installeert.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: df10bc8f-b980-4c61-ae6d-bcea03103738
source-git-commit: d46eb98c443a421f340b1021972ddb89eda1966b
workflow-type: tm+mt
source-wordcount: '1727'
ht-degree: 0%

---

# Een blauwdruk configureren

U kunt details van een blauwdruk vormen alvorens u het installeert. Voor de blauwdruktypen van projectsjablonen en organisatiestructuren moeten meestal enkele voorkeuren worden ingesteld en moeten bepaalde eigenschappen worden toegewezen. Voor andere typen blauwdrukken is mogelijk geen configuratie vereist en u installeert deze ongewijzigd. Voor meer informatie over installatie, zie [Een blauwdruk installeren](/help/quicksilver/administration-and-setup/blueprints/blueprints-install.md).

## Toegangsvereisten

U moet de volgende toegang hebben om de stappen in dit artikel uit te voeren:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] plan</strong></td>
   <td>Alle</td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Adobe [!DNL Workfront] licentie</strong></td>
   <td>[!UICONTROL Plan]</td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Configuraties op toegangsniveau</strong></td>
   <td> <p>[!UICONTROL System administrator]</p> </td> 
  </tr> 
 </tbody> 
</table>

## Een blauwdruk van een projectsjabloon configureren

1. Zoek de blauwdruk die u wilt gebruiken.
1. Klikken **[!UICONTROL Install]** kiest u vervolgens een omgeving:

   <table style="table-layout:auto">
        <tr>
        <td><strong>Productie</strong></td>
        <td>Productie is uw live omgeving.</td>
    </tr>
    <tr>
        <td><strong>Voorvertoning sandbox</strong></td>
        <td>De voorvertoning van de sandbox is een testomgeving die fungeert als replica van uw live omgeving en die elk weekend door Workfront wordt vernieuwd.</td>
    </tr>
    <tr>
        <td><strong>Sandbox 1 &amp; 2</strong></td>
        <td>De aangepaste vernieuwingssandbox is een aparte testomgeving die u handmatig kunt vernieuwen. Er zijn extra kosten voor het ophalen van de aangepaste vernieuwingssandbox.</td>
    </tr>
   </table>

1. Ga verder met de volgende secties:

   * [[!UICONTROL Template preferences]](#template-preferences)
   * [[!UICONTROL Role mapping]](#role-mapping)
   * [[!UICONTROL Team mapping]](#team-mapping)
   * [[!UICONTROL Company mappin]g](#company-mapping)
   * [[!UICONTROL Group mapping]](#group-mapping)

## [!UICONTROL Template preferences] {#template-preferences}

Kies hoe u de sjabloon wilt installeren.

U kunt sjablooneigendom ook toewijzen voordat u de blauwdruk installeert. U kunt deze velden wijzigen nadat de sjabloon is geïnstalleerd. Zie voor meer informatie [Projectsjablonen bewerken](../../manage-work/projects/create-and-manage-templates/edit-templates.md).

![[!UICONTROL Template Preferences] sectie](assets/Blueprints_TemplatePreferences.png)

1. In de [!UICONTROL Template Preferences] een nieuwe sjabloonnaam op.
1. Geef het volgende op:

   <table style="table-layout:auto">
    <tr>
        <td><strong>[!UICONTROL Template owner]<strong></td>
        <td>Deze persoon ontvangt [!UICONTROL Manage] toestemmingen op het malplaatje en zullen de eigenaar van het Project worden wanneer het malplaatje wordt gebruikt om een project tot stand te brengen.</td>
    </tr>
    <tr>
        <td><strong>[!UICONTROL Template sponsor]</strong></td>
        <td>Deze persoon is gewoonlijk een manager, uitvoerend, of belanghebbende die moet weten wat met het project gebeurt. De projectsponsor krijgt geen extra toegang tot het project, maar wordt toegevoegd aan de e-mailmeldingen voor het project.</td>
    </tr>
    <tr>
        <td><strong>[!UICONTROL Portfolio]</strong></td>
        <td>Dit is de portefeuille het project tot zal behoren wanneer het wordt gecreeerd.</td>
    </tr>
    <tr>
        <td><strong>[!UICONTROL Program]</strong></td>
        <td>Dit is het programma waar het project bij hoort wanneer het is gemaakt.</td>
    </tr>
   </table>

1. Selecteer of de sjabloon actief of inactief is geïnstalleerd.
1. Selecteer of u gedefinieerde voorkeuren voor nieuwe uitgaven wilt gebruiken als er voorkeuren beschikbaar zijn.

   Klikken **[!UICONTROL See issue preferences]** om de specifieke voorkeuren te bekijken die met de blauwdruk worden geïnstalleerd. Voor projecten die zijn gemaakt op basis van de geïmporteerde sjabloon worden deze voorkeuren gebruikt voor nieuwe uitgaven die zijn toegevoegd aan de [!UICONTROL Issues] sectie.

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>De het onderwerpgroepen van de Rij</strong></td> 
      <td> <p>De het onderwerpgroepen van de rij bepalen het hoogste niveau van categorieën voor de kwesties of de verzoeken. De gebruikers bekijken onderwerpgroepen als menuopties wanneer het selecteren waar te om verzoeken voor te leggen. Een onderwerpgroep kan veelvoudige rijonderwerpen bevatten. Zie voor meer informatie <a href="../../manage-work/requests/create-and-manage-request-queues/create-topic-groups.md" class="MCXref xref">Onderwerpgroepen maken</a>. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Werkvoorraadonderwerpen</strong></td> 
      <td> <p>De onderwerpen van de rij werken samen met het verpletteren van regels om kwesties of verzoeken toe te wijzen. Het zijn de menuopties die de gebruikers selecteren wanneer het ingaan van een kwestie of een verzoek, na het selecteren van een onderwerpgroep. Zie voor meer informatie <a href="../../manage-work/requests/create-and-manage-request-queues/create-queue-topics.md" class="MCXref xref">Werkvoorraadonderwerpen maken</a>. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Routeringsregels</strong></td> 
      <td>Het verpletteren van regels verzendt kwesties of verzoeken naar specifieke baanrollen, gebruikers, of teams. Zij kunnen de verzoeken aan specifieke projecten, buiten verbonden aan de verzoekrij ook verzenden. Zie voor meer informatie <a href="../../manage-work/requests/create-and-manage-request-queues/create-routing-rules.md" class="MCXref xref">Verpletterende regels maken</a>. </td> 
     </tr> 
    </tbody> 
   </table>

   >[!INFO]
   >
   >**Voorbeeld:** De nieuwe uitgiftevoorkeur in deze blauwdruk verstrekt vier rijonderwerpen. De gebruiker selecteert één van deze onderwerpen wanneer het creëren van een kwestie. (Omdat er slechts één onderwerpgroep bestaat, wordt deze automatisch toegepast en hoeft de gebruiker deze niet te selecteren.) Wanneer de gebruiker voltooit en de kwestie voorlegt, bepaalt het verpletteren van regels welke baanrol of team het aan wordt toegewezen.
   >![Voorkeuren voor nieuwe uitgave bekijken](assets/Blueprints_IssuePrefsDetails.png)
   >![De onderwerpen van de rij voor nieuwe kwestie](assets/blueprints-newissueqtopicsexample-350x204.png)
   >![Probleem gerouteerd naar taakrol](assets/Blueprints_ProjectShowsIssueAssignment.png)

   >[!TIP]
   >
   >* Met de voorkeuren voor uitgaven kunt u zorgen voor consistentie bij de manier waarop nieuwe problemen of verzoeken worden vastgelegd in uw projecten.
   >* Als u deze voorkeuren instelt, worden de projecten die met de sjabloon zijn gemaakt, niet automatisch omgezet in aanvraagwachtrijen. Voor informatie over het opzetten van een verzoekrij, zie [Een aanvraagwachtrij maken](../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md).
   >* Niet alle blauwdrukken bevatten nieuwe uitgiftevoorkeuren.



## [!UICONTROL Role mapping] {#role-mapping}

>[!NOTE]
>
>Deze sectie wordt mogelijk niet in alle blauwdrukken weergegeven.

Sommige sjablonen bevatten verplichte taakrollen. De rollen van de baan helpen u de juiste mensen toewijzen wanneer het malplaatje in een project wordt omgezet. U kunt aanpassen hoe rollen in kaart worden gebracht alvorens u de blauwdruk installeert. Klikken **[!UICONTROL See role descriptions]** voor meer informatie over de rollen die beschikbaar zijn in de blauwdruk.

De blauwdruk zoekt door de rolnaam om te zien of om het even welke bestaande rollen aanpassen. De zoekopdracht is hoofdlettergevoelig, dus namen moeten exact overeenkomen. Als er geen bestaande rollen overeenkomen, kunt u de blauwdruk deze voor u maken.

![[!UICONTROL Role Mapping] sectie](assets/Blueprints_RoleMapping.png)

1. Als een rol bestaat, kunt u één van de volgende opties kiezen:

   1. Maak een nieuwe rol met een andere naam en typ vervolgens de naam in het tekstvak.
   1. Gebruik een bestaande rol en selecteer vervolgens een rol in het selectievak.
   1. Gebruik geen toegewezen rol. Deze optie wordt niet aanbevolen omdat aan sommige taken geen rollen worden toegewezen.

1. Als een rol niet bestaat, kunt u één van de volgende opties kiezen:

   1. Maak een nieuwe rol. Met deze optie krijgt u de rol die de blauwdruk aanbeveelt.
   1. Maak een nieuwe rol met een andere naam en typ vervolgens de naam in het tekstvak.
   1. Gebruik een bestaande rol en selecteer vervolgens een rol in het selectievak.
   1. Gebruik geen toegewezen rol. Deze optie wordt niet aanbevolen omdat aan sommige taken geen rollen worden toegewezen.

>[!NOTE]
>
>Het installatieproces past geen rollen op specifieke mensen toe. U zou de mensen in die rollen na het installeren van de blauwdrukoplossing moeten verifiëren en mensen toewijzen indien nodig. Zie voor meer informatie [Handelingen die moeten worden uitgevoerd na de installatie van een blauwdruk](../../administration-and-setup/blueprints/best-next-actions-after-install.md).

Voor meer informatie over functies in [!DNL Workfront], zie [Taakrollen maken en beheren](../../administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md).

## [!UICONTROL Team mapping] {#team-mapping}

>[!NOTE]
>
>Deze sectie wordt mogelijk niet in alle blauwdrukken weergegeven.

Sommige sjablonen bevatten voorgeschreven teams. Het werk dat aan een team wordt toegewezen kan door om het even welk lid van het team worden voltooid. Voordat u de blauwdruk installeert, kunt u aanpassen hoe teams worden toegewezen. Klikken **[!UICONTROL See team descriptions]** voor meer informatie over de teams die beschikbaar zijn in de blauwdruk.

De blauwdruk zoekt door de teamnaam om te zien of om het even welke bestaande teams aanpassen. De zoekopdracht is hoofdlettergevoelig, dus namen moeten exact overeenkomen. Als er geen bestaande teams overeenkomen, kunt u de blauwdruk voor u maken.

![[!UICONTROL Team Mapping] sectie](assets/Blueprints_TeamMapping.png)

1. Als een team bestaat, kunt u één van de volgende opties kiezen:

   1. Maak een nieuw team met een andere naam en typ de naam in het tekstvak.
   1. Gebruiken [!UICONTROL existing team]selecteert u vervolgens een team in het selectievak.
   1. Gebruik geen toegewezen team. Deze optie wordt niet aanbevolen omdat voor sommige taken geen teams zijn toegewezen.

1. Als een team niet bestaat, kunt u een van de volgende opties kiezen:

   1. Maak een nieuw team. Met deze optie maakt u het team dat de blauwdruk aanbeveelt.
   1. Maak een nieuw team met een andere naam en typ de naam in het tekstvak.
   1. Gebruiken [!UICONTROL existing team]selecteert u vervolgens een team in het selectievak.
   1. Gebruik geen toegewezen team. Deze optie wordt niet aanbevolen omdat voor sommige taken geen teams zijn toegewezen.

>[!NOTE]
>
>Het installatieproces voegt geen mensen toe aan de teams. U zou de mensen op de teams na het installeren van de blauwdrukoplossing moeten verifiëren en mensen toewijzen indien nodig. Zie voor meer informatie [Handelingen die moeten worden uitgevoerd na de installatie van een blauwdruk](../../administration-and-setup/blueprints/best-next-actions-after-install.md).

Voor meer informatie over de werking van teams in [!DNL Workfront], zie [Teams maken en beheren](../../people-teams-and-groups/create-and-manage-teams/create-and-mange-teams.md).

## Bedrijfstoewijzing {#company-mapping}

>[!NOTE]
>
>Deze sectie wordt mogelijk niet in alle blauwdrukken weergegeven.

Sommige blauwdrukken omvatten voorgeschreven bedrijven. Een bedrijf is een organisatorische eenheid die uw organisatie, een afdeling binnen de organisatie, of een cliënt kan vertegenwoordigen u met werkt. U kunt aanpassen hoe bedrijven in kaart worden gebracht alvorens u de blauwdruk installeert. Klikken **[!UICONTROL See company descriptions]** voor meer informatie over de bedrijven in de blauwdruk .

De blauwdruk zoekt door de bedrijfsnaam om te zien of om het even welke bestaande bedrijven aanpassen. De zoekopdracht is hoofdlettergevoelig, dus namen moeten exact overeenkomen. Als er geen overeenkomende bestaande bedrijven zijn, kunt u de blauwdruk voor u maken. Het primaire bedrijf in de blauwdruk wordt in kaart gebracht aan het primaire bedrijf in uw milieu, zelfs als zij niet de zelfde naam hebben.

![[!UICONTROL Company Mapping] sectie](assets/Blueprints_CompanyMapping.png)

1. Als een bedrijf bestaat, kunt u één van de volgende opties kiezen:

   1. Maak een nieuw bedrijf met een andere naam en typ vervolgens de naam in het tekstvak.
   1. Gebruik het bestaande bedrijf en selecteer vervolgens een bedrijf in het selectievak.\

      Het primaire bedrijf in de blauwdruk wordt in kaart gebracht aan het primaire bedrijf in uw milieu, zelfs als zij niet de zelfde naam hebben.
   1. Gebruik geen toegewezen bedrijf. Deze optie wordt niet aanbevolen, omdat de bedrijfsverwijzingen in andere objecten leeg zijn.

1. Als een bedrijf niet bestaat, kunt u één van de volgende opties kiezen:

   1. Maak een nieuw bedrijf. Met deze optie maakt u het bedrijf dat door de blauwdruk wordt aanbevolen.
   1. Maak een nieuw bedrijf met een andere naam en typ vervolgens de naam in het tekstvak.
   1. Gebruik het bestaande bedrijf en selecteer vervolgens een bedrijf in het selectievak.
   1. Gebruik geen toegewezen bedrijf. Deze optie wordt niet aanbevolen, omdat de bedrijfsverwijzingen in andere objecten leeg zijn.

>[!NOTE]
>
>Om de bedrijven na het installeren van de blauwdruk te vormen, zie [Handelingen die moeten worden uitgevoerd na de installatie van een blauwdruk](../../administration-and-setup/blueprints/best-next-actions-after-install.md).

Voor informatie over het associëren van een malplaatje met een bedrijf, zie [Projectsjablonen bewerken](../../manage-work/projects/create-and-manage-templates/edit-templates.md).

Voor informatie over hoe bedrijven werken in [!DNL Workfront], zie [Bedrijven maken en bewerken](../../administration-and-setup/set-up-workfront/organizational-setup/create-and-edit-companies.md).

## [!UICONTROL Group mapping] {#group-mapping}

>[!NOTE]
>
>Deze sectie wordt mogelijk niet in alle blauwdrukken weergegeven.

Sommige blauwdrukken bevatten voorgeschreven groepen. Een groep is een groep gebruikers die samenvalt met de afdelingsstructuur. Groepen zijn vergelijkbaar met maar verschillen van teams en bedrijven in Workfront. Voordat u de blauwdruk installeert, kunt u aanpassen hoe groepen worden toegewezen. Klikken **[!UICONTROL See group descriptions]** voor meer informatie over de groepen die beschikbaar zijn in de blauwdruk.

De blauwdruk zoekt op de groepsnaam of er bestaande groepen overeenkomen. De zoekopdracht is hoofdlettergevoelig, dus namen moeten exact overeenkomen. Als er geen bestaande groepen overeenkomen, kunt u de blauwdruk voor u maken.

![[!UICONTROL Group Mapping] sectie](assets/Blueprints_GroupMapping.png)

1. Als er een groep bestaat, kunt u **[!UICONTROL Remap Group]** en kiest u een van de volgende opties:

   1. **[!UICONTROL Create a new group with a different name]** Typ vervolgens de naam die u aan deze groep wilt toewijzen. Verwijzingen naar de groep in de ontwerpdefinitie worden aan deze nieuwe groep gekoppeld.
   1. **[!UICONTROL Replace with an existing group]** en selecteert u vervolgens een groep in het selectievak.

      >[!NOTE]
      >
      >U kunt de naam van een bestaande groep niet wijzigen.

1. Als een groep niet bestaat, kunt u:

   1. Wijzig de voorgestelde groepsnaam door deze in het tekstvak te typen.
   1. Selecteren **[!UICONTROL Remap Group]** en kiest u [!UICONTROL Replace with an existing group]en selecteert u vervolgens een groep in het selectievak.
   1. Selecteren **[!UICONTROL Remap Group]** en kiest u **[!UICONTROL Insert under an existing group]** en selecteert u vervolgens een groep in het selectievak. Met deze optie maakt u een nieuwe subgroep onder de bestaande groep.

>[!NOTE]
>
>Om de groepen na het installeren van de blauwdruk te vormen, zie [Handelingen die moeten worden uitgevoerd na de installatie van een blauwdruk](../../administration-and-setup/blueprints/best-next-actions-after-install.md).

Voor informatie over het gebruik van groepen in [!DNL Workfront], zie [Overzicht van groepen](../../administration-and-setup/manage-groups/groups-overview/groups.md).
