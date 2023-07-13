---
product-area: requests
navigation-topic: create-and-manage-request-queues
title: Een aanvraagwachtrij maken
description: U kunt opstelling een Rij van het Verzoek waar de gebruikers occasionele verzoeken kunnen ingaan die niet gepland werk aan een project zijn.
author: Alina
feature: Work Management, Requests
topic: Collaboration
role: User
exl-id: 385420aa-0962-4b67-9d0d-b153dcf302cf
source-git-commit: ddb8f39e3ef400b02b443230f237b6a563d99d5f
workflow-type: tm+mt
source-wordcount: '2571'
ht-degree: 0%

---

# Een aanvraagwachtrij maken

<!--
<THIS IS CONNECTED TO THE PRODUCT IN BLUEPRINTS. DO NOT MOVE/ CHANGE URL>
-->

U kunt opstelling een Rij van het Verzoek waar de gebruikers occasionele verzoeken kunnen ingaan die niet gepland werk aan een project zijn. Bijvoorbeeld, kan een rij van het hulpdeskverzoek opstelling zijn om alle gebruikersverzoeken te vangen die aan een afdeling van IT komen.

## Toegangsvereisten

<!--drafted for P&P: replace the table below with this:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan*</td> 
   <td> <p>Any </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license*</td> 
   <td> 
   <p>Current license: Stadard </p>
   Or
   <p>Legacy license: Plan </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>Edit access to Projects</p> <p><b>NOTE</b> 
   
   If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can modify your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p> Manage permissions to the project</p> <p>For information on requesting additional access, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;To find out what plan, license type, or access you have, contact your Workfront administrator
-->

U moet de volgende toegang hebben om de stappen in dit artikel uit te voeren:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-abonnement*</td> 
   <td> <p>Alle </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-licentie*</td> 
   <td> <p>Plan </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraties op toegangsniveau*</td> 
   <td> <p>Toegang tot projecten bewerken</p> <p>Opmerking: Als u nog steeds geen toegang hebt, vraagt u de Workfront-beheerder of deze aanvullende beperkingen op uw toegangsniveau instelt. Voor informatie over hoe een beheerder van Workfront uw toegangsniveau kan wijzigen, zie <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Aangepaste toegangsniveaus maken of wijzigen</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objectmachtigingen</td> 
   <td> <p> Rechten voor het project beheren</p> <p>Voor informatie over het aanvragen van aanvullende toegang raadpleegt u <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Toegang tot objecten aanvragen </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Neem contact op met uw Workfront-beheerder als u wilt weten welk plan, licentietype of toegang u hebt

## Overzicht aanvraagrijen

U plaatst opstelling een verzoekrij als project. Wanneer u het project als Rij van het Verzoek aanwijst, wordt de rij toegankelijk van het gebied van Verzoeken van Adobe Workfront. Wanneer u de aanvraagwachtrij aanpast, past u ook de invulling van de formuliergebruikers aan wanneer ze de aanvragen verzenden.

Dit artikel beschrijft hoe te om een verzoekrij van een bestaand project tot stand te brengen. Nochtans, om consistentie voor uw proces van de verzoekinname te bouwen of veelvoudige lagen aan het voor rapporteringsdoeleinden en beter beheer toe te voegen, kunt u extra bouwstenen van een verzoekrij ook vormen die in de volgende lijst worden beschreven.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Wachtrij</td> 
   <td> <p>U moet opstelling een project als verzoekrij in het gebied van de Details van de Rij. Deze stap is verplicht. </p> <p>Zie voor meer informatie de <a href="#create-a-request-queue" class="MCXref xref">Een aanvraagwachtrij maken</a> in dit artikel.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Onderwerpgroepen</td> 
   <td> <p>Het zijn extra menu's die verzoeken classificeren die op gemeenschappelijke eigenschappen worden gebaseerd. Bijvoorbeeld, voor een Rij van het Verzoek van IT, zou u "On-site"en "Verre"onderwerpgroepen kunnen willen hebben. </p> <p>Zie voor meer informatie <a href="../../../manage-work/requests/create-and-manage-request-queues/create-topic-groups.md" class="MCXref xref">Onderwerpgroepen maken</a>. </p> <p>Dit is optioneel.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Onderwerpen van de Rij</td> 
   <td> <p>Zij zijn extra menu's die verzoeken classificeren die tot de zelfde Groep van het Onderwerp behoren die op gemeenschappelijke eigenschappen wordt gebaseerd. Een onderwerpgroep kan verscheidene rijonderwerpen bevatten. </p> <p>Bijvoorbeeld, kan de "On-site"onderwerpgroep voor de Rij van het Verzoek van IT de "Hardware", "Software"en "Netwerk"rijonderwerpen bevatten. </p> <p>Zie voor meer informatie <a href="../../../manage-work/requests/create-and-manage-request-queues/create-queue-topics.md" class="MCXref xref">Werkvoorraadonderwerpen maken</a>. </p> <p>Dit is optioneel.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Routeringsregels</td> 
   <td> <p>Zij staan u toe om elk verzoek aan een gebruiker, baanrol, team, of aan een project te leiden. </p> <p>Zie voor meer informatie <a href="../../../manage-work/requests/create-and-manage-request-queues/create-routing-rules.md" class="MCXref xref">Verpletterende regels maken</a>. </p> <p>Dit is optioneel.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Een aanvraagwachtrij maken

Wanneer u opstelling een project als Rij van het Verzoek, de projectstatus moet Actief zijn om op het gebied van Verzoeken van Workfront te tonen.

Een aanvraagwachtrij maken:

1. Ga naar het project dat u opstelling als Rij van het Verzoek wilt.
1. (Optioneel) Klik op **Projectdetails** in het linkerdeelvenster en voeg een **Beschrijving** aan het project in de **Overzicht** gebied. Deze informatie wordt weergegeven bij alle nieuwe aanvragen.
1. Klikken **Wachtrij** in het linkerdeelvenster. Mogelijk moet u op **Meer weergeven** vervolgens **Wachtrij**.

   Hiermee opent u de sectie Wachtrij details.

   ![](assets/classic-queue-setup-top-of-the-setup-form-350x248.png)

1. Geef de volgende informatie op:

   * **Publiceren als wachtrij voor Help-aanvragen:** Selecteer deze optie om dit project te identificeren als een aanvraagwachtrij. Alle inkomende kwesties worden beschouwd als Verzoeken.\
     Als deze optie niet is geselecteerd, gedraagt het project zich als een standaardproject in Workfront en zijn alle binnenkomende problemen van belang.

   * **Wie aanvragen kan toevoegen aan deze wachtrij:** Selecteer welke gebruikers toegang hebben om aanvragen aan deze wachtrij toe te voegen. U kunt de volgende groepen mensen toestaan om de Rij van het Verzoek in hun gebied van Verzoeken van de Globale Bar van de Navigatie te zien:

     | Wie aanvragen kan invoeren | Beschrijving |
     |---|---|
     | Iedereen | Elke Workfront-gebruiker met een actief account kan deze aanvraagwachtrij bekijken en er aanvragen aan toevoegen |
     | Personen met toegang tot dit project | Gebruikers met de machtiging Weergeven aan het project kunnen aanvragen weergeven en toevoegen aan deze wachtrij |
     | Personen in het bedrijf van dit project | De gebruikers die tot het bedrijf behoren verbonden aan dit project kunnen verzoeken aan deze rij bekijken en toevoegen. Als er een bedrijf verbonden aan het project is, is de naam van het bedrijf vermeld tussen haakjes na dit het plaatsen. |
     | Personen in de projectgroep | De gebruikers die tot de groep behoren verbonden aan dit project kunnen verzoeken aan deze rij bekijken en toevoegen. Als er een groep verbonden aan het project is, wordt de naam van de groep vermeld tussen haakjes na dit het plaatsen. |

     {style="table-layout:auto"}

   * **Delen met deze koppelingen:** Met de volgende opties kunt u gebruikers buiten Workfront of Workfront-gebruikers via een externe pagina rechtstreeks toegang geven tot de aanvraagwachtrij en de bijbehorende formulieren. Voor informatie over het insluiten van een verzoekrij in een dashboard als externe pagina, zie [Een aanvraagwachtrij insluiten in een dashboard](../../../reports-and-dashboards/dashboards/creating-and-managing-dashboards/embed-request-queue-dashboard.md).

     Gebruikers moeten al toegangsrechten tot de wachtrij hebben om directe toegang te krijgen. Het gebruik van een van de hier beschreven opties verleent niet automatisch toegang aan gebruikers.

     >[!TIP]
     >
     >Gebruikers moeten zich eerst aanmelden bij Workfront voordat ze toegang krijgen tot de wachtrij met aanvragen wanneer ze vanuit een andere toepassing toegang krijgen tot de pagina Wachtrij aanvragen.

      * **URL voor directe toegang:** Wanneer een gebruiker tot dit URL van browser toegang heeft, wordt de gebruiker genomen direct naar de Nieuwe sectie van het Verzoek in het gebied van Verzoeken en dit verzoek wordt geselecteerd door gebrek voor hen.

        ![](assets/share-request-queue-with-direct-url-embedded-in-dashboard-nwe-350x118.png)

        >[!NOTE]
        >
        >U kunt een verzoekwachtrij in een dashboard weergeven als een externe pagina. In dit geval is de wachtrij met aanvragen vooraf geselecteerd, maar u kunt een andere wachtrij met aanvragen selecteren in het veld Type verzoek. gebruikers kunnen het aanvraagtype wijzigen. Navigatiecomponenten van de Verzoeken worden ook weergegeven.

      * **Code insluiten:** Gebruik deze HTML-code om het formulier voor de aanvraagwachtrij in te sluiten als een iframe binnen een HTML-pagina.\
        Als gebruikers nog niet zijn geverifieerd bij Workfront wanneer ze de pagina bekijken waarop de code is ingesloten, wordt het Workfront-aanmeldingsvenster weergegeven. Nadat gebruikers zich hebben aangemeld, wordt het formulier Wachtrij aanvragen weergegeven.

        >[!NOTE]
        >
        Als een aanvraagwachtrij wordt weergegeven in een iframe, wordt alleen het aanvraagformulier weergegeven. De naam van de aanvraag wordt dan vooraf geselecteerd en grijs weergegeven. Gebruiker kan het aanvraagtype niet wijzigen. Navigatiecomponenten van het gebied Verzoeken worden niet weergegeven.

        Als u het formulier voor de aanvraagwachtrij wilt weergeven wanneer u deze insluitcode gebruikt, moet u de instelling Insluiten van Workfront in een iFrame toestaan inschakelen in de systeeminstellingen. Ga voor meer informatie over het inschakelen van insluiting van Workfront in een iframe naar [Beveiligingsvoorkeuren voor het systeem configureren](../../../administration-and-setup/manage-workfront/security/configure-security-preferences.md). Als deze instelling niet is ingeschakeld, wordt het iframe leeg weergegeven.

        U kunt als volgt verschillende aspecten van de weergave van het ingesloten formulier aanpassen:

        <table border="1" cellspacing="15"> 
         <col> 
         <col> 
         <thead> 
          <tr> 
           <th> <p><strong>Functionaliteit</strong> </p> </th> 
           <th> <p><strong>Oplossing</strong> </p> </th> 
          </tr> 
         </thead> 
         <tbody> 
          <tr> 
           <td> <p>De grootte van het frame aanpassen</p> </td> 
           <td> <p>Wijzig de kenmerken "width" en "height".</p> <p>De breedte is standaard "500" en de hoogte is "600"</p> </td> 
          </tr> 
          <tr> 
           <td> <p>Directe gebruikers aan een specifiek Onderwerp van de Rij of een Groep van het Onderwerp</p> </td> 
           <td> <p>Voeg de parameter "path" toe aan de URL van de bron. U kunt de wegparameter vinden door aan het gewenste Onderwerp of de Groep van het Onderwerp van de Rij in de niet ingebedde vorm te navigeren en URL te inspecteren.</p> </td> 
          </tr> 
          <tr> 
           <td> <p>Toon en sta gebruikers toe om de vooraf gevormde drop-down lijst van de Groep van het Onderwerp te veranderen</p> </td> 
           <td> <p>Gebruik de parameter "path" door de parameter "path" toe te voegen <code>showPreSelectedOptions=true</code> aan de <code>src URL</code>.</p> </td> 
          </tr> 
          <tr> 
           <td> <p>Detecteren wanneer het formulier is verzonden</p> </td> 
           <td> <p>Voeg een "message"-gebeurtenislistener toe aan het venster van uw webpagina en controleer of <code>event.data.type</code> is <code>requestSubmitted</code>. <code>event.data.newIssueID</code> wordt ingesteld op de id van het gemaakte probleem.</p> </td> 
          </tr> 
         </tbody> 
        </table>

   * **Typen aanvragen:** Maak een keuze uit de onderstaande standaardopties.

     De Workfront-beheerder kan de standaardaanvraagtypen een andere naam geven. Voor meer informatie over het anders noemen van de verzoektypes, zie [Standaardtypen voor problemen aanpassen](../../../administration-and-setup/set-up-workfront/configure-system-defaults/customize-default-issue-types.md).

      * Foutrapport
      * Volgorde wijzigen
      * Probleem
      * Verzoek

        Dit is een verplicht veld en u moet ten minste één optie selecteren.

     >[!NOTE]
     >
     De Types van verzoek tonen als selectie op het gebied van Verzoeken slechts als het Type van Verzoek in zowel de Details van de Rij als de pagina&#39;s van het Onderwerp van de Rij wordt geselecteerd. Voor informatie over vestiging het gebied van de Details van de Rij van een project, zie [Werkvoorraadonderwerpen maken](../../../manage-work/requests/create-and-manage-request-queues/create-queue-topics.md).

     Elk type dat u hier selecteert, is beschikbaar op het formulier (u kunt meerdere typen selecteren). Als u meerdere typen selecteert, kunt u meerdere aanvragen ordenen die binnenkomen.\
     Bijvoorbeeld, als u het formulier op een verzoekrij voor een project van IT gebruikt, kunnen de volgende verzoektypes in de rij komen: hardware, software, oplossingen voor problemen en problemen.

   * **Standaardduur:** De standaardduur is de tijd die nodig is om een uitgave te voltooien. Dit wordt de standaardinstelling voor alle binnenkomende uitgaven en kan handmatig worden gewijzigd. De duur wordt meestal ingesteld in uren, dagen of weken. De standaardduur van een uitgave is gelijk aan de geplande uren voor het probleem. De geplande afwerkingsdatum van de uitgave wordt berekend op basis van dit veld.\
     De standaardwaarde voor de duur van de uitgave is 1 dag of 8 uur. Als uw Workfront-beheerder de typische uren per werkdag instelt op minder dan 8 uur, is de standaardduur voor uitgaven nog steeds 8 uur. Als de typische uren per werkdag bijvoorbeeld op 7 uur zijn ingesteld, is de standaardduur voor uitgaven 1,14 dagen of 8 uur. Raadpleeg de sectie &#39;Tijdlijnberekeningen&#39; in het artikel voor meer informatie over het instellen van het systeem (normale uren per werkdag) [Projectvoorkeuren voor het hele systeem configureren](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).

   * **De mensen van het zelfde bedrijf zullen de zelfde toestemmingen voor alle verzoeken erven.:** Wanneer geselecteerd, zijn alle verzoeken die aan de rij worden voorgelegd zichtbaar voor gebruikers in het zelfde bedrijf. De gebruikers kunnen deze verzoeken in de Al sectie van Verzoeken bekijken, die binnen het gebied van Verzoeken wordt gevestigd. Op het moment dat deze instelling wordt in- of uitgeschakeld, heeft deze invloed op alle toekomstige aanvragen. de informatie heeft geen terugwerkende kracht .
   * **Wanneer iemand een verzoek indient, automatisch verlenen:** Wanneer een gebruiker een verzoek aan de verzoekrij indient, wordt de gebruiker automatisch verleend het niveau van toestemming dat u aan dat verzoek kiest. Selecteer een van de volgende machtigingsniveaus:

      * **Weergave**
      * **Contribute**. Dit is de standaardselectie.
      * **Beheren**

     Voor informatie over het Workfront machtigingenmodel raadpleegt u [Overzicht van het delen van machtigingen voor objecten](../../../workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md).\
     Het plaatsen van toestemmingen bewaart hier tijd, eerder dan het moeten toestemmingen voor elk individueel inkomend verzoek verlenen. Het kiezen van deze optie is van invloed op alle toekomstige verzoeken, maar heeft geen terugwerkende invloed op bestaande verzoeken.

   * **Standaardgoedkeuring**: Koppel een goedkeuringsproces aan deze verzoekrij. In dit keuzemenu worden alleen processen voor goedkeuring van uitgaven weergegeven. Alle kwesties die aan deze rij worden voorgelegd zullen met dit goedkeuringsproces worden geassocieerd. Uw Workfront-beheerder moet goedkeuringsprocessen op systeemniveau definiëren voordat u deze kunt koppelen aan aanvraagwachtrijen. Gebruikers met administratieve toegang tot goedkeuringsprocessen kunnen ook groepsspecifieke goedkeuringsprocessen maken.

     >[!IMPORTANT]
     >
     Als de groep van het project verandert, wordt het groep-specifieke goedkeuringsproces verbonden aan bestaande kwesties een enig-gebruiks goedkeuringsproces. Voor meer informatie over hoe de veranderingen in de groep van het project of de veranderingen in het goedkeuringsproces goedkeuringsmontages beïnvloeden, zie [De invloed van wijzigingen in groep- en goedkeuringsproces op toegewezen goedkeuringsprocessen](../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/how-changes-affect-group-approvals.md).

     Als u veelvoudige rijonderwerpen verbonden aan een verzoekrij hebt, adviseren wij dat u goedkeuringsprocessen met de rijonderwerpen in plaats daarvan associeert. Voor meer informatie over het creëren van rijonderwerpen, zie [Werkvoorraadonderwerpen maken](../../../manage-work/requests/create-and-manage-request-queues/create-queue-topics.md).

     Overweeg het volgende wanneer het toevoegen van goedkeuringsprocessen om rijen te verzoeken:

      * Alleen actieve goedkeuringsprocessen worden in de lijst weergegeven.
      * Systeemspecifieke en groepsspecifieke goedkeuringsprocessen worden in de lijst weergegeven. Een goedkeuringsproces verbonden aan een groep buiten die van het project toont niet in de lijst.

   * **Standaardroute**: Associeer een Verpletterende Regel met deze verzoekrij. Het gebruik dat Regels verplettert om nieuwe kwesties automatisch toe te wijzen die aan een Rij van het Verzoek aan het correcte middel (gebruiker, baanrol, of team) worden voorgelegd, en aan het correcte project. Alle kwesties die aan deze rij worden voorgelegd zullen met deze Verpletterende Regel worden geassocieerd. U moet het Verpletteren van Regels vormen alvorens u hen met verzoekrij kunt associëren.\
     Als u veelvoudige rijonderwerpen verbonden aan een verzoekrij hebt, adviseren wij dat u het verpletteren van regels met de rijonderwerpen in plaats daarvan associeert. Voor meer informatie over het creëren van het verpletteren van regels, zie [Verpletterende regels maken](../../../manage-work/requests/create-and-manage-request-queues/create-routing-rules.md).

   * **Nieuwe probleemvelden:** In toon de volgende geselecteerde gebieden aan alle gebruikerssectie, selecteer om het even welke gebieden die u zichtbaar aan alle gebruikers wilt zijn die een verzoek aan het project indienen of een kwestie toevoegen aan het project of de taken.

     >[!TIP]
     >
     De nieuwe die Gebieden van de Uitgave in de sectie van de Details van de Rij worden geselecteerd worden ook geassocieerd met om het even welke nieuwe kwestie aan het project of aan de taken in de sectie van Kwesties wordt toegevoegd.

     Wanneer u een van de velden Toegewezen aan, Functie of Team inschakelt, wordt de naam van de toewijzingen altijd gewijzigd in het aanvraagformulier, maar u kunt alleen het hier geselecteerde type toewijzing opgeven.

     >[!NOTE]
     >
     Als u Toegewezen aan in het gebied van de Details van de Rij selecteerde, kunt u slechts gebruikers op het gebied van Toewijzingen op het verzoekformulier ingaan. In dit geval kunt u geen taakrollen of een team invoeren.


   * **Documenten**: Als u de sectie Documenten wilt weergeven in het nieuwe aanvraagformulier, selecteert u waar de sectie voor het uploaden van documenten moet worden geplaatst. Selecteer een van de volgende opties:

     <table style="table-layout:auto"> 
      <col> 
      <col> 
      <tbody> 
       <tr> 
        <td role="rowheader">Na aangepaste formulieren</td> 
        <td><span>De sectie Documenten wordt onder aan het aanvraagformulier weergegeven.</span> </td> 
       </tr> 
       <tr> 
        <td role="rowheader">Voor aangepaste formulieren</td> 
        <td> <p><span>De sectie Documenten wordt weergegeven tussen de Workfront-velden en de aangepaste velden van het aanvraagformulier.</span> </p> </td> 
       </tr> 
      </tbody> 
     </table>

     ![](assets/nwe-new-issue-fields-area-with-documents-350x167.png)

   * **Alle geselecteerde en niet-geselecteerde velden weergeven in:** Selecteer welke gebruikers u alle velden op het formulier wilt weergeven. De volgende opties bepalen de toegang tot de velden op het formulier.

     | Welke gebruikers alle velden op het aanvraagformulier kunnen zien | Beschrijving |
     |---|---| 
     | Alle gebruikers (abonnementslicenties) | Alle gebruikers met een licentie voor abonnementen kunnen zowel de geselecteerde als de niet-geselecteerde velden zien. |
     | Personen met toegang tot dit project (licentie voor abonnementen) | Gebruikers met een licentie voor een abonnement die ook weergaverechten voor dit project hebben, kunnen zowel de geselecteerde als de niet-geselecteerde velden zien. De rest van de gebruikers die aanvragen kunnen indienen voor dit project, kunnen alleen de geselecteerde velden zien. |
     | Geen gebruikers | De niet-geselecteerde velden kunnen niet door gebruikers worden weergegeven. Alle gebruikers die aanvragen naar dit project kunnen verzenden, kunnen alleen de geselecteerde velden zien. |

   * **Aangepaste Forms**: Selecteer een aangepast formulier dat u wilt koppelen aan de aanvraagwachtrij. Alleen Issue Custom Forms is beschikbaar om te selecteren in dit keuzemenu. Aan alle problemen die worden voorgelegd aan de wachtrij met aanvragen worden de geselecteerde formulieren gekoppeld.\
     Als u de veelvoudige Onderwerpen van de Rij verbonden aan een Rij van het Verzoek hebt, adviseren wij dat u douaneformulieren met de Onderwerpen van de Rij in plaats daarvan associeert. Voor meer informatie over het creëren van subsecties voor de Rij van het Verzoek, zie [Werkvoorraadonderwerpen maken](../../../manage-work/requests/create-and-manage-request-queues/create-queue-topics.md).

     ![](assets/custom-forms-on-queue-details.png)

     Als er meerdere aangepaste formulieren zijn gekoppeld aan de aanvraagwachtrij, sleept u de formulieren naar de gewenste volgorde en zet u deze neer in de **Forms opnieuw ordenen** sectie.

     >[!TIP]
     >
     De vormen van de douane die aan de sectie van de Details van de Rij worden toegevoegd worden ook geassocieerd met om het even welke nieuwe kwestie die aan het project of de taken in de sectie van Kwesties wordt toegevoegd.

1. Doorgaan met het selecteren van gegevens voor de instellingen in het dialoogvenster **E-mailwachtrijinstellingen** om gebruikers toe te staan verzoeken te e-mailen naar het project van de verzoekrij.

   Zie voor meer informatie [Gebruikers toestaan een uitgave per e-mail te verzenden naar een aanvraagwachtrij-project](../../../manage-work/requests/create-requests/enable-email-issues-into-projects.md).

1. Klikken **Opslaan**.\
   Uw project is nu gevormd om een Rij van het Verzoek te zijn en de gebruikers kunnen verzoeken aan het nu toevoegen.

1. (Facultatief) om de functionaliteit van de Rij van het Verzoek te verbeteren, bouw extra ondersecties voor uw rij, evenals regels om de inkomende verzoeken aan het correcte team, de ontvanger of het project te leiden.

   * Raadpleeg de artikelen voor informatie over het maken van subsecties voor de aanvraagwachtrij [Werkvoorraadonderwerpen maken](../../../manage-work/requests/create-and-manage-request-queues/create-queue-topics.md) en [Onderwerpgroepen maken](../../../manage-work/requests/create-and-manage-request-queues/create-topic-groups.md).
   * Voor informatie over het verpletteren van de verzoeken aan de aangewezen ontvanger, het team, en aangewezen project, zie [Verpletterende regels maken](../../../manage-work/requests/create-and-manage-request-queues/create-routing-rules.md).
