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
source-git-commit: aec61210cf2c17775738db4975ae8d19223153cc
workflow-type: tm+mt
source-wordcount: '1433'
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

Zie voor meer informatie over de informatie in deze tabel [Toegangsvereisten in Workfront-documentatie](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

## Een aangepast toegangsniveau maken of bewerken

{{step-1-to-setup}}

1. Klikken **Toegangsniveaus** in het linkerdeelvenster.
1. Selecteer het toegangsniveau u wilt kopiëren en aanpassen, dan klik **Kopiëren**.

   of

   Als u een bestaand toegangsniveau (dat u eerder kopieerde) uitgeeft, klik zijn naam.

1. Voer in het vak dat wordt weergegeven een van de volgende handelingen uit om het aangepaste toegangsniveau te configureren:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Naam</td> 
      <td> <p>Typ een naam voor uw toegangsniveau. </p> <p>Als u enkel een toegangsniveau kopieerde om nieuwe tot stand te brengen, is de standaardnaam de Naam van het Niveau van de Toegang (Exemplaar), waar de Naam van het Niveau van de Toegang het toegangsniveau is u kopieerde.</p> <p><strong>Tip</strong>: Wij adviseren dat u de originele naam van het toegangsniveau in de naam van het exemplaar omvat. Bij ACME-bedrijven krijgt een kopie van het standaardtoegangsniveau bijvoorbeeld de naam ACME Standard.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Beschrijving </td> 
      <td>Typ een beschrijving voor het toegangsniveau. Het is handig om hier te vermelden waartoe een gebruiker met dit toegangsniveau toegang heeft.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Licentietype</td> 
      <td>Zorg ervoor dat de hier geselecteerde licentie de licentie is die het meest wordt gekoppeld aan het type toegangsniveau dat u maakt of bewerkt. De geselecteerde licentie bepaalt welke instellingen beschikbaar zijn voor het toegangsniveau. Zie voor meer informatie <a href="/help/quicksilver/administration-and-setup/add-users/how-access-levels-work/licenses-overview.md" class="MCXref xref">Overzicht van nieuwe licenties</a> of <a href="/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md">Overzicht van licenties</a>.</td> 
     </tr> 
    </tbody> 
   </table>

1. (Voorwaardelijk) Indien **Standaard** of **Plan** is geselecteerd in het dialoogvenster **Licentietype** vak, naar de sectie schuiven **Beheertoegang toestaan voor** en selecteer administratieve toegangstoestemmingen voor degenen die dit toegangsniveau zullen hebben.

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
       </ul><p><b>OPMERKING</b>: Hierdoor kan de gebruiker geen nieuwe kostentypen maken.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">Functies</td> 
      <td> Met deze toegang mag de gebruiker het volgende doen: 
       <ul> 
        <li>Bestaande taakrollen weergeven en bewerken</li> 
        <li>Nieuwe taakrollen toevoegen</li> 
        <li>Rolfacturering en kostentarieven bewerken</li> 
       </ul> 
       <p>Voor belangrijke informatie over toegang tot financiële gegevens die beschikbaar is voor een gebruiker van de Norm of van de Planner met administratieve toegang tot baanrollen, zie <a href="#standard-or-planner-users-with-administrative-access-to-job-roles">Standaard of Planner-gebruikers met beheerbare toegang tot functies</a>.</p>
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

1. Klikken **Aanvullende beperkingen instellen** stelt u vervolgens een van de volgende beperkingen voor het toegangsniveau in.

   >[!IMPORTANT]
   >
   >Voor externe gebruikers zoals verkopers (iedereen niet in uw organisatie), adviseren wij dat u toegang tot taken, projecten, updates, aankondigingen, andere bedrijven, teams en groepen beperkt.

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Nooit toegang geven tot het hele project wanneer het aan een taak of kwestie wordt toegewezen</td> 
      <td> Verhindert gebruikers die aan taken of kwesties worden toegewezen om toestemmingen aan het ouderproject ook te krijgen, zelfs als de projecttoestemmingen dat toestaan.<p>Voor meer informatie over het vormen van de toestemmingen op een project, zie de sectie <a href="../../../manage-work/projects/manage-projects/edit-projects.md#access" class="MCXref xref"></a> in het artikel <a href="../../../manage-work/projects/manage-projects/edit-projects.md" class="MCXref xref">Projecten bewerken</a>.</p></td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">Documenttoegang nooit overerven van projecten, taken, problemen, enz..</td> 
      <td>Voorkomt dat documenten de machtigingen overnemen die zijn ingesteld voor het bovenliggende object.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Alleen updates weergeven waarin ze zijn opgenomen in het gesprek</td> 
      <td> Laat gebruikers toe om slechts commentaren te zien waar hun naam of de naam van hun team is inbegrepen. <p> <p><b>OPMERKING</b>: Hiermee voorkomt u dat gebruikers zich abonneren op objecten in Workfront. Zie voor meer informatie over abonnementen op objecten <a href="../../../workfront-basics/using-notifications/subscribe-to-items-in-workfront.md" class="MCXref xref">Abonneren op objecten in Adobe Workfront</a>.</p> </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Gebruikers nooit toestaan opmerkingen te verwijderen </td> 
      <td> Hiermee voorkomt u dat gebruikers de opmerkingen die ze maken over items verwijderen.  <p><b>OPMERKING</b>: Niemand kan de opmerkingen van andere gebruikers verwijderen.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Alleen bedrijven, groepen en teams weergeven waartoe ze behoren</td> 
      <td>Staat gebruikers toe om punten slechts met bedrijven, groepen, en teams te bekijken en te delen zij tot behoren.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Zichtbaarheid van geplande uren of werkelijke uren nooit toestaan</td> 
      <td>Hiermee voorkomt u dat gebruikers de geplande en werkelijke uren van de door hen geopende werkitems kunnen zien. Zij kunnen, echter, Werkelijke Uren zien zij zich registreren, of uren die door iemand worden geregistreerd die aan hen rapporteert.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Gebruikers nooit toestaan om aankondigingen te verwijderen</td> 
      <td>Voorkomt dat gebruikers aankondigingen in het Aankondigingscentrum verwijderen. Zie voor meer informatie <a href="../../../administration-and-setup/get-started-wf-administration/view-send-announcements.md" class="MCXref xref">Aankondigingen verzenden</a>.</td> 
     </tr> 
    </tbody> 
   </table>

1. (Voorwaardelijk en optioneel) Als uw Workfront-systeem is ingesteld voor gebruikers die tot meerdere bedrijven behoren, beperkt u de zichtbaarheid tot andere gebruikers op basis van het bedrijf waartoe zij behoren in de sectie **Personen in andere bedrijven mogen alleen gebruikers van**.

   U kunt de gebruikers beperken om enkel gebruikers van hun eigen bedrijf of van het bedrijf te zien u als primair bedrijf aangewezen. Het primaire bedrijf vertegenwoordigt doorgaans uw Workfront-account waar de meeste gebruikers werken. Voor meer informatie over het primaire bedrijf raadpleegt u [Bedrijven maken en bewerken](../../../administration-and-setup/set-up-workfront/organizational-setup/create-and-edit-companies.md).

   >[!NOTE]
   >
   >Als twee gebruikers tot twee verschillende bedrijven behoren, maar zij kunnen allebei gebruikers van het primaire bedrijf zien, kunnen zij het gebied van Updates zien verbonden aan het primaire bedrijf.

1. (Optioneel) Als u de toegangsinstellingen wilt configureren voor andere objecten en gebieden in het toegangsniveau waaraan u werkt, gaat u verder met een van de artikelen in [Toegang tot Adobe Workfront configureren](../../../administration-and-setup/add-users/configure-and-grant-access/configure-access.md), zoals [Toegang verlenen tot taken](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-tasks.md) en [Toegang tot financiële gegevens verlenen](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md).
1. Klikken **Opslaan**.

   Nadat het toegangsniveau wordt gecreeerd, kunt u het aan een gebruiker toewijzen (tenzij het een toegangsniveau van de Beheerder van het Systeem is).

   Zie voor meer informatie [Gebruikersprofiel bewerken](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

   Voor informatie over hoe een beheerder van de Adobe een de toegangsniveau van de Beheerder van het Systeem aan een gebruikers toewijst, zie [Volledige administratieve toegang verlenen aan een gebruiker](../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md).

## Standaard of Planner-gebruikers met beheerbare toegang tot functies {#planner-users}

Als u een gebruiker van de Norm of van de Planner administratieve toegang tot baanrollen verleent, wordt de Edit het Factureren van de Rol &amp; het plaatsen van de Tarieven automatisch toegelaten voor de gebruiker.

Later, als u administratieve toegang tot baanrollen voor de gebruiker onbruikbaar maakt, zijn de baanrollen nog zichtbaar aan de gebruiker omdat de Edit het Factureren van de Rol &amp; het plaatsen van de Tarieven van Kosten nog wordt toegelaten.

Als dit gebeurt en u de toegang van de gebruiker tot de rollen van de meningsbaan moet verwijderen, moet u de het Edit van de Rol van de gebruiker het Factureren &amp; van de Tarieven van Kosten plaatsen van de Toestemming onbruikbaar maken. Zie voor instructies [Toegang tot financiële gegevens verlenen](grant-access-financial.md).
