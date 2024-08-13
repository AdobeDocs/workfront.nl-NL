---
title: Aangepaste toegangsniveaus maken en wijzigen
user-type: administrator
product-area: system-administration;user-management
navigation-topic: configure-access-to-workfront
description: Als Adobe Workfront-beheerder kunt u aangepaste toegangsniveaus maken en deze op gebruikers toepassen.
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: d2a73d24-51d3-42e2-9c09-7f4bc30b2caa
source-git-commit: c887569d59c7751210671cab97c492ee1752fffc
workflow-type: tm+mt
source-wordcount: '1463'
ht-degree: 0%

---

# Aangepaste toegangsniveaus maken en wijzigen

<!--Audited: 12/2023-->

<!--Don't delete, draft, or change the title of this article. The UI links to it via context-sensitive help. -->

Als Adobe Workfront-beheerder kunt u aangepaste toegangsniveaus maken en deze op gebruikers toepassen. Als u met toegangsniveaus werkt, is het belangrijk dat u begrijpt hoe ze samenwerken met de objectmachtigingen die gebruikers verlenen wanneer ze objecten met elkaar delen. Voor meer informatie over toegangsniveaus, zie:

* [Overzicht van nieuwe toegangsniveaus](/help/quicksilver/administration-and-setup/add-users/how-access-levels-work/access-level-overview.md)
* [Overzicht van toegangsniveaus](../../../administration-and-setup/add-users/access-levels-and-object-permissions/access-levels-overview.md)

>[!IMPORTANT]
>
>Wij adviseren sterk dat u de ingebouwde toegangsniveaus onveranderd laat zodat u naar hen kunt verwijzen nadat u opstelling uw gebruikers. Als u een toegangsniveau wilt aanpassen, kopieert u het standaardtoegangsniveau en wijzigt u de kopie. U kunt dit voor elk toegangsniveau behalve de Beheerder van het Systeem en Externe Gebruiker doen.

## Toegangsvereisten

+++ Breid uit om de toegangseisen voor de functionaliteit in dit artikel weer te geven.

U moet de volgende toegang hebben om de stappen in dit artikel uit te voeren:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-plan</td> 
   <td>Alle</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-licentie</td> 
   <td>Nieuw: Standaard
   <p>of</p>
   <p>Huidig: Plan</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraties op toegangsniveau</td> 
   <td> <p>U moet een Workfront-beheerder zijn.</p></td> 
  </tr> 
 </tbody> 
</table>

Voor meer detail over de informatie in deze lijst, zie [ vereisten van de Toegang in de documentatie van Workfront ](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Een aangepast toegangsniveau maken of bewerken

{{step-1-to-setup}}

1. Klik **Niveaus van de Toegang** in het linkerpaneel.
1. Selecteer het toegangsniveau u wilt kopiëren en aanpassen, dan **Exemplaar** klikken.

   of

   Als u een bestaand toegangsniveau (dat u eerder kopieerde) uitgeeft, klik zijn naam.

1. Voer in het vak dat wordt weergegeven een van de volgende handelingen uit om het aangepaste toegangsniveau te configureren:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Naam</td> 
      <td> <p>Typ een naam voor uw toegangsniveau. </p> <p>Als u enkel een toegangsniveau kopieerde om nieuwe tot stand te brengen, is de standaardnaam de Naam van het Niveau van de Toegang (Exemplaar), waar de Naam van het Niveau van de Toegang het toegangsniveau is u kopieerde.</p> <p><strong> Uiteinde </strong>: Wij adviseren dat u de originele naam van het toegangsniveau in de naam van het exemplaar omvat. Bij ACME-bedrijven krijgt een kopie van het standaardtoegangsniveau bijvoorbeeld de naam ACME Standard.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Beschrijving </td> 
      <td>Typ een beschrijving voor het toegangsniveau. Het is handig om hier te vermelden waartoe een gebruiker met dit toegangsniveau toegang heeft.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Licentietype</td> 
      <td>Zorg ervoor dat de hier geselecteerde licentie de licentie is die het meest wordt gekoppeld aan het type toegangsniveau dat u maakt of bewerkt. De geselecteerde licentie bepaalt welke instellingen beschikbaar zijn voor het toegangsniveau. Voor meer informatie, zie <a href="/help/quicksilver/administration-and-setup/add-users/how-access-levels-work/licenses-overview.md" class="MCXref xref"> Nieuw vergunningsoverzicht </a> of <a href="/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md"> overzicht van Vergunningen </a>.</td> 
     </tr> 
    </tbody> 
   </table>

1. (Voorwaardelijk) als **Standaard** of **Plan** in de **doos van het Type van Vergunning** wordt geselecteerd, scrol aan de sectie **administratieve toegang voor** verlenen en administratieve toegangstoestemmingen voor die selecteren die dit toegangsniveau zullen hebben.

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Goedkeuringsprocessen</td> 
      <td>Goedkeuringsprocessen voor gebruik in het hele systeem en voor specifieke groepen maken en beheren.<p>Zonder deze toegang kunnen gebruikers alleen ad-hocgoedkeuringsprocessen maken voor items die ze kunnen beheren.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">Bedrijven</td> 
      <td>Voeg nieuwe bedrijven toe en bewerk bestaande bedrijven in Workfront.<br><p>Zonder deze toegang kunnen gebruikers alleen bestaande bedrijven bekijken.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">Aangepaste formulieren</td> 
      <td>Alle aangepaste formulieren in hun groep maken en beheren. <br><p>Zonder deze toegang kunnen gebruikers alleen bestaande formulieren koppelen aan de objecten die ze kunnen bijdragen of beheren.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">Wisselkoersen</td> 
      <td> Voeg nieuwe valuta toe in Workfront. <p>Zonder deze toegang kan de gebruiker alleen een bestaande valuta toevoegen aan een project dat hij of zij maakt.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Uitgaven</td> 
      <td>Alle uitgaven weergeven voor objecten in Workfront.<p>Zonder deze toegang kan de gebruiker alleen het volgende weergeven:</p>
       <ul>
        <li>Uitgaven voor projecten, taken of kwesties die zij beheren</li>
        <li>Hun eigen kosten</li>
        <li>De kosten van hun ondergeschikten</li>
       </ul><p><b> NOTA </b>: Dit staat de gebruiker niet toe om nieuwe Types van Uitgaven tot stand te brengen.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">Functies</td> 
      <td> Met deze toegang mag de gebruiker het volgende doen: 
       <ul> 
        <li>Bestaande taakrollen weergeven en bewerken</li> 
        <li>Nieuwe taakrollen toevoegen</li> 
        <li>Rolfacturering en kostentarieven bewerken</li> 
       </ul> 
       <p>Voor belangrijke informatie over toegang tot financiële gegevens die aan een Standaard of gebruiker van de Planner met administratieve toegang tot baanrollen beschikbaar is, zie <a href="#standard-or-planner-users-with-administrative-access-to-job-roles"> Norm of de gebruikers van de Planner met administratieve toegang tot baanrollen </a>.</p>
      </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Mijlpalen in mijn fractie</td> 
      <td>Bekijk alle milestone-paden in het systeem onder het menu Paden van mijlpaal in Setup. De gebruikers kunnen om het even welke milestone wegen ook uitgeven of schrappen die tot om het even welk van hun groepen behoren. Gebruikers kunnen geen milestone-paden beheren (bewerken of verwijderen) die niet aan hun groep zijn toegewezen.<p>Zonder deze toegang, kunnen de gebruikers bestaande milestone wegen slechts bekijken en hen toepassen op projecten zij toegang hebben te beheren.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">Herinneringsmeldingen</td> 
      <td>Herinneringsberichten maken en beheren in Workfront.<p>Zonder deze toegang zijn gebruikers beperkt tot het ontvangen en weergeven van meldingen.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">Timesheets en uren</td> 
      <td> De beheerders van de groep kunnen timesheet profielen aan gebruikers in de groepen en subgroepen toewijzen zij leiden. <p>Als deze optie niet is ingeschakeld, kunnen groepsbeheerders geen timesheet-profielen toewijzen aan andere gebruikers in de groepen en subgroepen die zij beheren, hoewel zij deze wel kunnen maken.</p> <p>Alle andere gebruikers met een Standard- of Plan-licentie kunnen alle uren en tijdbladen in Workfront bekijken.</p> <p>Als deze optie niet is ingeschakeld, kunnen gebruikers alleen uren weergeven op:</p> 
       <ul> 
        <li>Projecten, taken of problemen die zij beheren</li> 
        <li>Hun eigen tijdschema</li> 
        <li>Een tijdspad van iemand die een melding ontvangt</li> 
        <li>Een overzicht van de goedgekeurde tijdschriften</li> 
       </ul> </td> 
     </tr> 
    </tbody> 
   </table>

1. Klik **Reeks extra beperkingen**, dan plaats om het even welke volgende beperkingen voor het toegangsniveau.

   >[!IMPORTANT]
   >
   >Voor externe gebruikers zoals verkopers (iedereen niet in uw organisatie), adviseren wij dat u toegang tot taken, projecten, updates, aankondigingen, andere bedrijven, teams en groepen beperkt.

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Nooit toegang geven tot het hele project wanneer het aan een taak of kwestie wordt toegewezen</td> 
      <td> Verhindert gebruikers die aan taken of kwesties worden toegewezen om toestemmingen aan het ouderproject ook te krijgen, zelfs als de projecttoestemmingen dat toestaan.<p>Voor meer informatie over het vormen van de toestemmingen op een project, zie de sectie <a href="../../../manage-work/projects/manage-projects/edit-projects.md#access" class="MCXref xref"></a> in het artikel <a href="../../../manage-work/projects/manage-projects/edit-projects.md" class="MCXref xref"> projecten </a> uitgeven.</p></td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">Documenttoegang nooit overerven van projecten, taken, problemen, enz..</td> 
      <td>Voorkomt dat documenten de machtigingen overnemen die zijn ingesteld voor het bovenliggende object.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Alleen updates weergeven waarin ze zijn opgenomen in het gesprek</td> 
      <td> Laat gebruikers toe om slechts commentaren te zien waar hun naam of de naam van hun team is inbegrepen. <p> <p><b> NOTA </b>: Dit verhindert gebruikers aan punten in Workfront in te tekenen. Voor meer informatie over het intekenen op punten, zie <a href="../../../workfront-basics/using-notifications/subscribe-to-items-in-workfront.md" class="MCXref xref"> aan punten in Adobe Workfront </a> intekenen.</p> </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Gebruikers nooit toestaan opmerkingen te verwijderen </td> 
      <td> Hiermee voorkomt u dat gebruikers de opmerkingen die ze maken over items verwijderen.  <p><b> NOTA </b>: Niemand kan de commentaren van andere gebruikers schrappen.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Alleen bedrijven, groepen en teams weergeven waartoe ze behoren</td> 
      <td>Staat gebruikers toe om punten slechts met bedrijven, groepen, en teams te bekijken en te delen zij tot behoren.<p><strong> NOTA </strong>: De gebruikers met de vergunningen van de Aanvrager kunnen geen bedrijven bekijken zij niet tot behoren, zelfs als deze optie wordt geselecteerd.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Zichtbaarheid van geplande uren of werkelijke uren nooit toestaan</td> 
      <td>Hiermee voorkomt u dat gebruikers de geplande en werkelijke uren van de door hen geopende werkitems kunnen zien. Zij kunnen, echter, Werkelijke Uren zien zij zich registreren, of uren die door iemand worden geregistreerd die aan hen rapporteert.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Gebruikers nooit toestaan om aankondigingen te verwijderen</td> 
      <td>Voorkomt dat gebruikers aankondigingen in het Aankondigingscentrum verwijderen. Voor meer informatie, zie <a href="../../../administration-and-setup/get-started-wf-administration/view-send-announcements.md" class="MCXref xref"> aankondigingen </a> verzenden.</td> 
     </tr> 
    </tbody> 
   </table>

1. (Voorwaardelijk en facultatief) als uw systeem van Workfront opstelling voor gebruikers is die tot veelvoudige bedrijven behoren, beperk het zicht tot andere gebruikers die op welk bedrijf worden gebaseerd zij tot in de sectie **Mensen in andere bedrijven zouden slechts gebruikers van** moeten bekijken.

   U kunt de gebruikers beperken om enkel gebruikers van hun eigen bedrijf of van het bedrijf te zien u als primair bedrijf aangewezen. Het primaire bedrijf vertegenwoordigt doorgaans uw Workfront-account waar de meeste gebruikers werken. Voor meer informatie over het primaire bedrijf, zie [ bedrijven ](../../../administration-and-setup/set-up-workfront/organizational-setup/create-and-edit-companies.md) creëren en uitgeven.

   >[!NOTE]
   >
   >Als twee gebruikers tot twee verschillende bedrijven behoren, maar zij kunnen allebei gebruikers van het primaire bedrijf zien, kunnen zij het gebied van Updates zien verbonden aan het primaire bedrijf.

1. (Facultatief) om toegangsmontages voor andere voorwerpen en gebieden in het toegangsniveau te vormen u aan werkt, ga met één van de artikelen voort die in [ worden vermeld toegang tot Adobe Workfront ](../../../administration-and-setup/add-users/configure-and-grant-access/configure-access.md), zoals [ toegang van de Verlening tot taken ](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-tasks.md) en [ toegang van de Verlening tot financiële gegevens ](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md).
1. Klik **sparen**.

   Nadat het toegangsniveau wordt gecreeerd, kunt u het aan een gebruiker toewijzen (tenzij het een toegangsniveau van de Beheerder van het Systeem is).

   Voor meer informatie, zie [ het profiel van een gebruiker ](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md) uitgeven.

   Voor informatie over hoe een beheerder van de Adobe een de toegangsniveau van de Beheerder van het Systeem aan gebruikers toewijst, zie [ een gebruiker volledige administratieve toegang verlenen ](../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md).

## Standaard of Planner-gebruikers met beheerbare toegang tot functies {#planner-users}

Als u een gebruiker van de Norm of van de Planner administratieve toegang tot baanrollen verleent, wordt de Edit het Factureren van de Rol &amp; het plaatsen van de Tarieven automatisch toegelaten voor de gebruiker.

Later, als u administratieve toegang tot baanrollen voor de gebruiker onbruikbaar maakt, zijn de baanrollen nog zichtbaar aan de gebruiker omdat de Edit het Factureren van de Rol &amp; het plaatsen van de Tarieven van Kosten nog wordt toegelaten.

Als dit gebeurt en u de toegang van de gebruiker tot de rollen van de meningsbaan moet verwijderen, moet u de het Edit van de Rol van de gebruiker het Factureren &amp; van de Tarieven van Kosten plaatsen van de Toestemming onbruikbaar maken. Voor instructies, zie [ toegang van de Verlening tot financiële gegevens ](grant-access-financial.md).
