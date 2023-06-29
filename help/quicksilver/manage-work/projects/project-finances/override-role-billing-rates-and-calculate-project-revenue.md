---
product-area: projects
navigation-topic: financials
title: Overzicht van het overschrijven van de Billing Rates van de Rol en het berekenen van Inkomsten op een project
description: U kunt factureringstarieven gebruiken om opbrengst op uw projecten te berekenen wanneer u hen met de uren vermenigvuldigt die aan het project worden uitgegeven. Voor meer informatie over factureringstarieven en inkomsten, zie het artikel Overzicht van Facturering en Ontvangsten.
author: Alina, Lisa
feature: Work Management
exl-id: 63ba6758-ba62-48b4-89f4-d784e32a1bfa
source-git-commit: 1517e3e28fe536a8a72d2802919c8b8819e9ea1a
workflow-type: tm+mt
source-wordcount: '3852'
ht-degree: 0%

---

# Overzicht van het overschrijven van de Billing Rates van de Rol en het berekenen van Inkomsten op een project

{{highlighted-preview}}

U kunt factureringstarieven gebruiken om opbrengst op uw projecten te berekenen wanneer u hen met de uren vermenigvuldigt die aan het project worden uitgegeven. Zie het artikel voor meer informatie over factureringssnelheden en inkomsten [Overzicht van facturering en inkomsten](../../../manage-work/projects/project-finances/billing-and-revenue-overview.md).

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<p>(NOTE: drafted because the only procedure here was moved to a different article.&nbsp;This stays as an overview)</p>
<h2>Access requirements</h2>
<p>You must have the following access to perform the steps in this article:</p>
<table style="table-layout:auto">
<col>
<col>
<tbody>
<tr>
<td role="rowheader">Adobe Workfront plan*</td>
<td> <p>Any</p> </td>
</tr>
<tr>
<td role="rowheader">Adobe Workfront license*</td>
<td> <p>Plan </p> </td>
</tr>
<tr>
<td role="rowheader">Access level configurations*</td>
<td> <p>Edit access to Projects and Financial&nbsp;Data</p> <note type="note">
If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can modify your access level, see
<a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.
</note> </td>
</tr>
<tr>
<td role="rowheader">Object permissions</td>
<td> <p>Manage permissions to the project with permissions to Manage Finance</p> <p>For information on requesting additional access, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td>
</tr>
</tbody>
</table>
<p>*To find out what plan, license type, or access you have, contact your Workfront administrator.</p>
</div>
-->

## Overzicht van de factuurtarieven voor de rol en de inkomsten uit de rol van de werknemer

Als Adobe Workfront-beheerder kunt u factureringssnelheden koppelen aan zowel gebruikers als functies.\
Raadpleeg het artikel voor meer informatie over het maken van gebruikers en het koppelen van gebruikers aan factureringssnelheden [Gebruikers toevoegen](../../../administration-and-setup/add-users/create-and-manage-users/add-users.md). Raadpleeg het artikel voor meer informatie over het maken van taakrollen en het koppelen van rollen aan factureringssnelheden [Taakrollen maken en beheren](../../../administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md).

Factureringssnelheden voor gebruikers kunnen niet worden overschreven.

Factureringstarieven die aan baanrollen worden geassocieerd kunnen op het bedrijf of projectniveau worden met voeten getreden.

Om de opbrengsten van projecten te berekenen op basis van de factureringsgraad van de functies, **Type inkomsten** van de projecttaken moet een van de volgende zijn:

* Rol Uur
* Rol Uur met lampvoet
* Rol Uur plus Vast

Meer informatie over **Type inkomsten** en factureringssnelheden, zie [Overzicht van facturering en inkomsten](../../../manage-work/projects/project-finances/billing-and-revenue-overview.md).

## Hiërarchie van overschrijvingen van factureringssnelheden bij de berekening van inkomsten

Aan een taakrol kan op de volgende manieren een factureringsfrequentie zijn gekoppeld:

* Als Workfront-beheerder kunt u de factureringssnelheid op systeemniveau definiëren die aan een taakrol is gekoppeld wanneer u die taakrol maakt.\
  Zie voor meer informatie over het maken van taakrollen [Taakrollen maken en beheren](../../../administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md).

* Als beheerder van Workfront, kunt u het bedrijf-vlakke het factureren tarief voor de zelfde baanrol bepalen wanneer u een bedrijf creeert.\
  Wanneer Workfront inkomsten berekent voor de projecten verbonden aan dit bedrijf, wordt het bedrijf facturerend tarief gebruikt wanneer de rol aan taken wordt toegewezen, in plaats van het systeem-vlakke factureringspercentage voor deze baanrol.\
  De op het niveau van het bedrijf veranderde roltarieven zullen gevolgen hebben voor alle projecten verbonden aan dat bedrijf.

  >[!NOTE]
  >
  >Als u het het facturerings tarief van het Bedrijf moet bijwerken, zal het tarief op het project niet automatisch bijwerken. U moet het Bedrijf uit het project verwijderen, het tarief voor het Bedrijf bijwerken, dan het Bedrijf aan het project opnieuw vastmaken, alvorens het nieuwe tarief van het Bedrijf op het project van kracht wordt. Voor instructies bij het vastmaken van een Bedrijf aan een project, zie [Projecten bewerken](../../../manage-work/projects/manage-projects/edit-projects.md).

  Zie voor meer informatie over het maken van factureringssnelheden voor functies die specifiek voor een bedrijf gelden [Bedrijven maken en bewerken](../../../administration-and-setup/set-up-workfront/organizational-setup/create-and-edit-companies.md).

* Als beheerder van Workfront, kunt u een optie toelaten wanneer het uitgeven van een project om veranderingen in bedrijf-vlakke het factureren tarieven op het project toe te passen wanneer de gebruikers manueel projectfinanciën herberekenen.\
  Zie voor meer informatie [Override project-Level het Factureren Tarieven met het bedrijf-Vlakke FactureringsTarieven](../../../manage-work/projects/project-finances/override-project-level-with-company-level-billing-rates.md).

<div class="preview">

* Als beheerder van Workfront, kunt u tariefkaarten met veelvoudige het factureren tarieven per rol bepalen, die op plaats en datum wordt gebaseerd. Wanneer een tariefkaart aan een project in bijlage is, worden alle rollen (door plaats, als de plaatsen worden gebruikt) en hun bijbehorende het factureringspercentages toegevoegd aan de de factureringsrentesectie van het project. Het vastmaken van een tariefkaart treedt om het even welke bestaande het facturerings tarieven op het project met voeten.

  Zie voor meer informatie [Creditcards beheren](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/manage-rate-cards.md) en [Een tariefkaart aan een project koppelen](/help/quicksilver/manage-work/projects/project-finances/attach-rate-card-to-project.md).

</div>

* Als projectmanager, kunt u het het facturerings tarief voor de zelfde baanrol op het projectniveau bepalen.\
  Veranderde roltarieven op het project zullen slechts effect hebben op dat project.

  Voor informatie over het overschrijven van roltarieven voor het project, zie [De Factureringstarieven van de Rol van de Opheffing van de Taak op het projectniveau](../../../manage-work/projects/project-finances/override-job-role-billing-rates-at-the-project-level.md).

>[!IMPORTANT]
>
>Als een baanrol met een het factureringspercentage op het systeemniveau, het niveau van het Bedrijf, en het projectniveau wordt geassocieerd, berekent Workfront de opbrengst van de taken gebruikend het het facturerings tarief van de baanrol op het projectniveau, wanneer het de banen roltarieven gebruikt. De opbrengst van alle taken rolt tot de opbrengst van het project.

## De Factureringstarieven van de Rol van de Opheffing van de Taak op het projectniveau

Als projectmanager, kunt u specificeren wat het het facturerings tarief voor een baanrol op een specifiek project is. Dit factureringstarief op projectniveau treedt het factureringstarief op het systeemniveau voor deze baanrol met voeten. Workfront gebruikt het factureringstarief op projectniveau van de baanrol om opbrengst te berekenen, in plaats van het systeem-vlakke factureringstarief te gebruiken.

<span class="preview">U kunt een tariefkaart aan het project ook vastmaken, die de het factureringspercentages van de baanrol van de tariefkaart in het project zal invoeren.</span>

Voor informatie over hoe te om de het Facturerings Tarieven van de Rol van de Baan op het projectniveau met voeten te treden, zie [De Factureringstarieven van de Rol van de Opheffing van de Taak op het projectniveau](../../../manage-work/projects/project-finances/override-job-role-billing-rates-at-the-project-level.md).

Voor meer informatie over welke baanrol wordt gebruikt om opbrengst over het project te berekenen, zie de &quot;berekeningen van de Inkomsten voor taken die op gebruikers en van de Taken van de Rol worden gebaseerd&quot;sectie in [Overzicht van facturering en inkomsten](../../../manage-work/projects/project-finances/billing-and-revenue-overview.md). <span class="preview">Voor informatie over het vastmaken van een tariefkaart aan een project, zie [Een tariefkaart aan een project koppelen](/help/quicksilver/manage-work/projects/project-finances/attach-rate-card-to-project.md).</span>

>[!NOTE]
>
>In het geval van werkelijke inkomsten mogen de factureringstarieven die worden toegepast op uren die worden toegevoegd aan een factureringsrecord dat als facturering is gemarkeerd, niet worden beïnvloed door overschrijvingen van factureringstarieven die plaatsvinden nadat de factureringsrecord is gefactureerd.

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<p>(NOTE: drafted and linked above to the stand-alone article for overriding billing rates on projects.)</p>
<p>You can override the billing rate of a job role on a project in the following ways:</p>
<ul>
<li>One time, by selecting a new rate for the job role.<br>The new rate is used for the entire duration of the project, to calculate revenue. </li>
</ul>
<ul>
<li>Several times, by selecting several new rates for specific date ranges. <br>A different rate can be used during each specified date range.</li>
</ul>
<p>To override a billing rate for a project:</p>
<ol>
<li value="1">Go to the project you want to override billing rates for.</li>
<li value="2"> <p data-mc-conditions="QuicksilverOrClassic.Quicksilver">Click <strong>Billing Rates</strong> in the left panel. You might have to first click <strong>Show More</strong>. </p> </li>
<li value="3"> <p>Click <strong>Add Billing Rate</strong> > <strong>New Billing Rate</strong>.</p> <p>The New Billing Rate box opens</p> <p> <img src="assets/override-billing-rate-on-project-nwe-350x310.png" style="width: 350;height: 310;"> </p> <p> <br>The <strong>Default Billing Rate</strong> field displays the system-level rate for this job role.</p> </li>
<li value="4">In the <strong>Job Role</strong> field, select the job role you want to change the billing rate for.<br></li>
<li value="5">In the <strong>Billing Rates 1</strong> field, enter the one time billing rate override, then click <strong>Save</strong> to override the billing rate one time, <br>Or Click <strong>Add Rate</strong> to add more billing rate overrides.</li>
<li value="6">(Conditional) If you are adding more than one billing rate override, specify the following information:<br>- <strong>Billing Rates 1</strong>: the value of the Billing Rate from the beginning of the project to the first date of the first override. This is typically the same amount as the <strong>Default Rate</strong>.<br>- <strong>Start Date</strong>: this is the date when the Default Rate ends.<br>- <strong>End Date</strong>: the date when the new billing rate override ends. <br>Workfront applies the override job role rate to the hours that occur during the time frames specified when calculating revenue on the project.<br>There should be no gaps between the time frames of two override rates. The <strong>Start Date</strong> of an override rate should be the day immediately following the <strong>End Date</strong> of the previous override date.<br><note type="note">
You cannot specify a
<strong>Start Date</strong> for the first override rate, nor an
<strong>End Date</strong> for the last override rate. We recommend that you use the Default Rate for the first override rate.
<br>Workfront assumes that the first override rate is applied for all hours with a date older than the
<strong>End Date</strong> of the first override, and that the last override rate is applied for all hours with a date newer than the
<strong>Start Date</strong> of the last override.
<br>If an hour is logged before the Planned Start Date of the project the very first billing rate is used.
<br>If an hour is logged after the Planned Completion Date of the project the very last billing rate is used.
</note><br></li>
<li value="7">Click <strong>Save</strong>.</li>
</ol>
</div>
-->

## Overzicht van het gedeelte Factureringstarieven van een project

Nadat u de met voeten getreden factureringspercentages voor de baanrollen verbonden aan het project hebt gespecificeerd, kunt u alle baanrollen en hun met voeten treden in zien **Factureringstarieven** tabblad van het project.

Let op de volgende informatie in de lijst met **Factureringstarieven**:

* [Taakrolgroepering](#job-role-grouping)
* [Waarde van factureringssnelheid van project](#project-billing-rate-value)
* [Standaardfactuurwaarde](#default-billing-rate-value)
* [Factureringswaarde bedrijf](#company-billing-rate-value)
* [Meerdere waarden voor factureringssnelheid en tijdframes](#multiple-billing-rate-values-and-timeframes)

### Taakrolgroepering {#job-role-grouping}

Factureringstarieven worden gegroepeerd in de **Factureringstarieven** per werkplek. <span class="preview">Als een tariefkaart aan het project in bijlage is, dan worden de baanrollen ook gegroepeerd door tariefkaart. Als locaties worden toegepast op taakrollen, wordt de locatienaam opgenomen als onderdeel van de naam van de taakrol. U zou de zelfde baanrol kunnen hebben die voor veelvoudige plaatsen wordt vermeld.</span>

### Waarde van factureringssnelheid van project {#project-billing-rate-value}

In de groeperingslijn die aan een baanrol beantwoordt, merk het factureringspercentage voor die baanrol op het projectniveau in **Factureringsgraad van project** kolom. Als de taakrol meerdere overschrijvingssnelheden heeft, wordt de overschrijvingssnelheid die overeenkomt met de huidige datum weergegeven op de regel voor cijfergroepering in het dialoogvenster **Factureringsgraad van project** kolom.

### Standaardfactuurwaarde {#default-billing-rate-value}

In de groeperingslijn van een baanrol, merk het factureringspercentage voor die baanrol op het systeemniveau in **Standaardfactureringsfrequentie** kolom.

>[!NOTE]
>
>Als er tarieven voor projectfacturering voor een baanrol zijn, **Standaardfactureringsfrequentie** nooit wordt toegepast op de berekening van de inkomsten voor het project. Alleen de **Factureringstarieven voor projecten** worden toegepast voor de berekening van de opbrengsten.

### Factureringswaarde bedrijf {#company-billing-rate-value}

In de groeperingslijn van een baanrol, merk het factureringspercentage voor die baanrol op het bedrijfsniveau in **Factureringsgraad bedrijf** kolom. Dit betekent dat er een bedrijf is verbonden aan dit project, en deze baanrol heeft een verschillend factureringspercentage voor dat bedrijf. Het factureringstarief voor de bedrijfvertoningen, zelfs als het het zelfde als het projecttarief is.

>[!NOTE]
>
><span class="preview">Wanneer een tariefkaart aan het project in bijlage is, **Factureringstarieven voor bedrijven** niet worden ingevoerd in de factureringssnelheden. De berekeningen zijn gebaseerd op of tarief kaarttarieven of bedrijfstarieven voor de baanrollen.</span>
>
>Als er tarieven voor projectfacturering voor een baanrol zijn, **Factureringsgraad bedrijf** nooit wordt toegepast op de berekening van de inkomsten voor het project. Alleen de **Factureringstarieven voor projecten** worden toegepast om de opbrengsten te berekenen.

### Meerdere waarden voor factureringssnelheid en tijdframes {#multiple-billing-rate-values-and-timeframes}

Als u meerdere factureringssnelheden voor een specifieke taakrol hebt, worden deze vermeld onder de groepering voor die taakrol. Met inline bewerken kunt u de overschrijvingssnelheden en de **Start** **Datum** en **Einddatum** van de overschrijffactureringssnelheden op dit tabblad.

>[!NOTE]
>
>U kunt geen **Begindatum** voor de eerste overschrijvingsfrequentie en u kunt geen **Einddatum** voor de laatste overschrijvingstarief. Workfront gaat ervan uit dat de eerste overschrijvingsfrequentie wordt toegepast voor alle uren met een datum die ouder is dan de **Einddatum** van de eerste overschrijving, en dat de laatste overschrijvingstarief wordt toegepast op alle uren met een datum die jonger is dan **Begindatum** van de laatste overschrijving.\
>Als een uur vóór de Geplande Datum van het Begin van het project het programma wordt geopend wordt het eerste factureringstarief gebruikt.\
>Als een uur na de Geplande Datum van Voltooiing van het project het programma wordt geopend wordt het laatste factureringstarief gebruikt.

## Geplande inkomsten berekenen

* [Geplande inkomsten berekenen op basis van een eenmalige overschrijving](#calculate-planned-revenue-based-on-a-one-time-billing-rate-override)
* [Geplande inkomsten berekenen op basis van meervoudige overschrijvingen van factureringssnelheden](#calculate-planned-revenue-based-on-multiple-billing-rate-overrides)
* [Verdeling van geplande uren over de duur van een taak](#distribution-of-planned-hours-across-the-duration-of-a-task)

### Geplande inkomsten berekenen op basis van een eenmalige overschrijving {#calculate-planned-revenue-based-on-a-one-time-billing-rate-override}

Houd rekening met het volgende wanneer u geplande inkomsten berekent op basis van een eenmalige overschrijving:

* Wanneer de **Type inkomsten** van een taak **Rol Uur**, vermenigvuldigt Workfront de geplande uren van een taak met de factureringsgraad van de baanrol verbonden aan de taak om Geplande Inkomsten op de taak te berekenen.

* Wanneer het factureringspercentage van de functie op projectniveau is overschreven, gebruikt Workfront het overschrijvingspercentage van het project om de geplande inkomsten te berekenen.
* Wanneer een taak meerdere taken heeft, wordt de geplande opbrengst berekend door het factureringspercentage van elke taak en hun respectieve geplande uurtoewijzing te vermenigvuldigen.

>[!NOTE]
>
>De geplande uren per toewijzing zijn niet gelijk aan de geplande uren voor de taak, in het geval van meerdere toewijzingen.

Voor meer informatie over welke baanrol wordt gebruikt om Geplande Inkomsten te berekenen, zie de &quot;Begrip sectie van de Berekeningen van de Inkomsten voor Taken die op Gebruiker en de Taken van de Rol&quot;in het artikel worden gebaseerd [Overzicht van facturering en inkomsten](../../../manage-work/projects/project-finances/billing-and-revenue-overview.md).

### Geplande inkomsten berekenen op basis van meervoudige overschrijvingen van factureringssnelheden {#calculate-planned-revenue-based-on-multiple-billing-rate-overrides}

Houd rekening met het volgende bij het berekenen van geplande inkomsten op basis van meervoudige overschrijvingen van factureringssnelheden:

* Wanneer de **Type inkomsten** van een taak **Rol Uur**, vermenigvuldigt Workfront de geplande uren van een taak met de factureringsgraad van de baanrol verbonden aan de taak om Geplande Inkomsten op de taak te berekenen.

  Voor meer informatie over welke baanrol wordt gebruikt om Geplande Inkomsten te berekenen, zie de &quot;Begrip sectie van de Berekeningen van de Inkomsten voor Taken die op Gebruiker en de Taken van de Rol&quot;in het artikel worden gebaseerd [Overzicht van facturering en inkomsten](../../../manage-work/projects/project-finances/billing-and-revenue-overview.md).

* In het geval van veelvoudige het facturerings tarief treedt met voeten, verandert het tarief waardoor de Geplande Uren tijdens de duur van een taak worden vermenigvuldigd. Standaard verdeelt Workfront de geplande uren gelijkmatig over de duur van een taak, waarbij een gelijk aantal uren voor elke dag van de taak wordt toegewezen. Bij het berekenen **Geplande inkomsten** voor een taak vermenigvuldigt Workfront de geplande uren per dag met de factureringssnelheid van die dag. In het geval van meerdere factureringssnelheden kan dat tarief elke dag verschillend zijn.

  Bijvoorbeeld, hebt u een taak met een Uur van de Rol **Type inkomsten**. De taak duurt 5 dagen en de waarde voor het geplande uur is 40 uur. De geplande uren per dag is 8 uur. Wijs een de baanrol van de Projectleider van aan de taak toe, en ga het factureringspercentage van deze baanrol voor de laatste drie dagen van de taak met voeten, zodat zult u een tarief 1 facturerings voor de eerste twee dagen, en tarief 2 facturerings tarief voor de resterende drie dagen van de taak voor deze baanrol hebben.

  De formule die de **Geplande inkomsten** deze taak is :

  ```
  Planned Revenue = (Rate 1) * (Planned Hours for Day 1) + (Rate 1) * (Planned hours for Day 2) + (Rate 2) * (Planned hours for Day 3) + (Rate 2) * (Planned hours for Day 4) + (Rate 2) * (Planned hours for Day 5)
  ```

Zie de sectie voor meer informatie over het vinden van de geplande uren per dag in Workfront [Verdeling van geplande uren over de duur van een taak](#distribution-of-planned-hours-across-the-duration-of-a-task) in dit artikel.

>[!NOTE]
>
>Als u veelvoudige wijzers op de taak hebt, wordt de hoeveelheid Geplande Uren eerst verdeeld aan elke toegewezen persoon, en dan aan elke dag tijdens de duur van de taak. In dit geval wordt bij de berekening van de geplande ontvangsten rekening gehouden met het bedrag van de daguren voor elke toegewezen werknemer en het factureringspercentage van elke functie die tijdens de duur van de taak kan veranderen, in het geval van meervoudige factureringstarieven.

### Verdeling van geplande uren over de duur van een taak {#distribution-of-planned-hours-across-the-duration-of-a-task}

Overweeg het volgende wanneer het begrip van de verdeling van Geplande Uren over de Duur van een taak:

* Door gebrek, verdeelt Workfront de Geplande Uren gelijkmatig over de Duur van een taak, die een gelijk aantal Geplande Uren voor elke dag van de taak, op de beschikbaarheid van het projectprogramma toewijst.

  Voor meer informatie over het begrip van de verdeling van Geplande Uren over de Duur van een taak, zie de &quot;Begrip van de Distributie van Geplande Uren over de Duur van een Taak&quot;sectie in het artikel [Overzicht van geplande uren](../../../manage-work/tasks/task-information/planned-hours.md).

  >[!NOTE]
  >
  >De geplande uren per dag is de verdeling van de geplande uren voor elke dag tijdens de duur van de taak. Als de taak één taak heeft, dan vertegenwoordigt dit aantal ook de Geplande Uren per Dag per taak. Als de taak meerdere taken heeft, verschilt de geplande uren per dag per toewijzing van de taken van de geplande uren per dag. Er is geen visuele weergave in Workfront voor de geplande uren per dag per toewijzing, voor taken met meerdere toewijzingen.
  >
  >
  >De geplande uren per dag worden vermenigvuldigd met de factureringsgraad voor de functie die voor die dag aan de taak is toegewezen om de geplande inkomsten per dag voor die taak te berekenen. De som van alle op deze wijze berekende dagelijkse geraamde inkomsten is gelijk aan de voor die taak geplande inkomsten.

## Werkelijke inkomsten berekenen

* [Berekenen van de werkelijke inkomsten op basis van een eenmalige overschrijving](#calculate-actual-revenue-based-on-a-one-time-billing-rate-override)
* [Ware inkomsten berekenen op basis van meervoudige overschrijvingen van factureringssnelheden](#calculate-actual-revenue-based-on-multiple-billing-rate-overrides)

### Berekenen van de werkelijke inkomsten op basis van een eenmalige overschrijving {#calculate-actual-revenue-based-on-a-one-time-billing-rate-override}

Houd rekening met het volgende wanneer u de werkelijke inkomsten berekent op basis van een eenmalige overschrijving:

* Wanneer de **Type inkomsten** van een taak **Rol Uur**, Workfront vermenigvuldigt de **Werkelijke uren** van een taak door het factureringstarief van de baanrol verbonden aan de te berekenen taak **Werkelijke ontvangsten** over de taak. Werkelijke uren zijn uren die rechtstreeks bij de taak zijn geregistreerd.

  Voor meer informatie over welke functie wordt gebruikt om te berekenen **Werkelijke ontvangsten**, zie de &quot;Begrijpende sectie van de Berekeningen van de Ontvangsten voor Taken die op Gebruiker en de Toewijzingen van de Rol&quot;in het artikel worden gebaseerd [Overzicht van facturering en inkomsten](../../../manage-work/projects/project-finances/billing-and-revenue-overview.md).

* Als het factureringspercentage van de functie op projectniveau is overschreven, gebruikt Workfront het overschrijvingspercentage van het project om de werkelijke inkomsten te berekenen. Wanneer u het factureringstarief van de baanrol op het project met voeten treedt, **Werkelijke ontvangsten** van het project automatisch wordt herberekend aan de hand van het nieuwe aangepaste tarief.

  Voor informatie over het overschrijven van roltarieven voor het project, zie [De Factureringstarieven van de Rol van de Opheffing van de Taak op het projectniveau](../../../manage-work/projects/project-finances/override-job-role-billing-rates-at-the-project-level.md).

>[!NOTE]
>
>Als u de uren wilt houden die u reeds het project hebt het programma geopend alvorens u het originele factureringstarief dat tegen het originele tarief wordt gefactureerd, moet u hen in omvatten **Factureringsrecord** en u moet de **Factureringsrecord** als **Gefactureerd**. Anders wordt **Werkelijke ontvangsten** vanaf de uren die zijn geregistreerd voordat de factureringsgraad voor het project werd overschreven , wordt het nieuwe tarief opnieuw berekend wanneer de financiën van de projecten opnieuw worden berekend .\
>Meer informatie over het opnemen van uren in een factureringsrecord en het markeren als **Gefactureerd**, zie het artikel [Factureringsrecords maken](../../../manage-work/projects/project-finances/create-billing-records.md).

### Ware inkomsten berekenen op basis van meervoudige overschrijvingen van factureringssnelheden {#calculate-actual-revenue-based-on-multiple-billing-rate-overrides}

Houd rekening met het volgende wanneer u de werkelijke inkomsten berekent op basis van meervoudige overschrijvingen van de factureringssnelheid:

* Wanneer de **Type inkomsten** van een taak **Rol Uur**, Workfront vermenigvuldigt de **Werkelijke uren** op de taak met het factureringspercentage van de aan de taak toegewezen taakrollen om te berekenen **Werkelijke ontvangsten** over de taak. Werkelijke uren zijn uren die rechtstreeks bij de taak zijn geregistreerd.

* In geval van meervoudige factureringssnelheden, de snelheid waarmee de **Werkelijke uren** worden vermenigvuldigd om de **Werkelijke ontvangsten** kan tijdens de duur van een taak veranderen. Workfront gebruikt de factureringssnelheid van de taakrol waarvan het tijdframe overeenkomt met het **Invoerdatum** van de uren die voor de taak worden geregistreerd om te berekenen **Werkelijke ontvangsten.**

  Een taak heeft bijvoorbeeld de opdracht **Type inkomsten** van **Rol Uur** en wordt toegewezen aan de taakrol van Projectmanager. Overschrijf de factureringsgraad van deze baanrol met Tarief 1 voor de data tussen 19 en 25 juni. Vanaf 26 juni, treedt het facturerings tarief met Tarief 2 met voeten. Log 2 uur voor 20 juni en 3 uur voor 28 juni.

  Workfront berekent de **Werkelijke ontvangsten** voor deze taak met behulp van de volgende formule:

  ```
  Actual Revenue = 2 * Rate 1 + 3 * Rate 2
  ```

  Voor meer informatie over welke functie wordt gebruikt om te berekenen **Werkelijke ontvangsten**, zie de &quot;Begrijpende sectie van de Berekeningen van de Ontvangsten voor Taken die op Gebruiker en de Toewijzingen van de Rol&quot;in het artikel worden gebaseerd [Overzicht van facturering en inkomsten](../../../manage-work/projects/project-finances/billing-and-revenue-overview.md).

## Het effect van tijdzones bij de berekening van inkomsten op basis van meervoudige factureringstarieven

Gebruikers kunnen verschillende geplande uren per dag zien dan andere gebruikers als er verschillen in de tijdzone tussen hen en andere entiteiten in Workfront optreden. De volgende scenario&#39;s kunnen de Geplande Uren per Daginformatie voor een gebruiker van scheeftrekken wat een andere gebruiker ziet:

* De twee gebruikers zouden hun computers kunnen hebben die voor twee verschillende tijdzones worden geplaatst
* De twee gebruikersprofielen in Workfront kunnen op twee verschillende tijdzones worden ingesteld
* De tijdzone die aan het gebruikersprofiel is gekoppeld, kan anders zijn dan de systeemtijdzone in Workfront
* De tijdzone verbonden aan het gebruikersprofiel zou dan de Zone van de Tijd van de planning van het project kunnen verschillend zijn.

In deze gevallen kan het aantal geplande uren per dag verschillen tussen twee gebruikers die niet dezelfde instellingen voor tijdzones delen. Ze zullen ook verschillende geplande inkomstennummers zien wanneer meerdere overschrijvingen van factureringssnelheden voor een project worden gebruikt.

* [Geplande inkomsten berekenen voor gebruikers in verschillende tijdzones](#calculate-planned-revenue-for-users-in-different-time-zones)
* [Ware inkomsten berekenen voor gebruikers in verschillende tijdzones](#calculate-actual-revenue-for-users-in-different-time-zones)

### Geplande inkomsten berekenen voor gebruikers in verschillende tijdzones {#calculate-planned-revenue-for-users-in-different-time-zones}

>[!NOTE]
>
>Als u gebruikers in verschillende tijdzones hebt die aan de zelfde projecten werken, adviseren wij dat u niet de het facturerings tarief met voeten treedt voor uw projecten tijdens de week. Dit kan een onjuiste hoeveelheid Geplande Inkomsten voor uw project tonen, als resultaat van uurverschillen tussen de tijdzones in de lijst van de gebruikers en de het systeemtijdzone van Workfront. De meeste programma&#39;s staan toe dat weekends van de Geplande berekeningen van Uren worden uitgesloten. Als een verandering in het facturerings tarief opheffing van een baanrol gebeurt, is het beter voor het voorkomen tijdens een weekend dan in het midden van een week wanneer het met het midden van de Duur van een taak zou kunnen samenvallen.

Houd rekening met het volgende bij het berekenen van de geplande inkomsten voor gebruikers in verschillende tijdzones:

* Voor taken die een **Type inkomsten** van **Rol Uur** en worden toegewezen aan functies, **Geplande inkomsten** wordt berekend door vermenigvuldiging van **Geplande uren** van een taak door het factureringstarief van de baanrol.

* De **Geplande uren** gelijkmatig over de **Duur** van de taak.

* De **Duur** is de periode tussen de **Geplande start** **Datum** en de **Geplande afsluitdatum** van de taak. Omdat **Geplande begindatum** en **Geplande afsluitdatum** Als de taken kunnen verschillen, afhankelijk van de tijdzones van de gebruikers die de taak bekijken, kan de hoeveelheid geplande uren per dag verschillen voor twee gebruikers in twee verschillende tijdzones.

* De hoeveelheid geplande uren per dag verandert niets aan de geplande inkomsten van een project als de factureringsgraad van de rol van de baan niet wordt gewijzigd of als er slechts één factureringstarief is. Zelfs als twee gebruikers uit twee verschillende tijdzones verschillende geplande uren per dag zien, is de totale geplande opbrengst van het project gelijk voor beide gebruikers.

  In het geval van meervoudige overschrijvingen van de factureringsgraad, echter, de **Geplande inkomsten** van het project voor twee gebruikers in twee verschillende tijdzones mogelijk verschillend lijken, omdat het afhankelijk is van de hoeveelheid geplande uren per dag (die voor de twee gebruikers verschillend kunnen zijn) en de tariefoverschrijving (die voor dezelfde dag verschillend zou kunnen zijn, wanneer elke gebruiker de taak in hun eigen tijdzone bekijkt).

* De nauwkeurigheid **Geplande inkomsten** Deze hoeveelheid wordt gezien door de gebruiker die dezelfde tijdzone heeft als de tijdzone van uw Workfront-instantie. Uw Workfront-beheerder definieert de Workfront-tijdzone in het gedeelte System Customer Info.\
  Raadpleeg het artikel voor meer informatie over het definiëren van de tijdzone voor uw systeem [Basisinformatie voor uw systeem configureren](../../../administration-and-setup/get-started-wf-administration/configure-basic-info.md).

### Ware inkomsten berekenen voor gebruikers in verschillende tijdzones {#calculate-actual-revenue-for-users-in-different-time-zones}

Houd rekening met het volgende bij het berekenen van de werkelijke inkomsten voor gebruikers in verschillende tijdzones:

* Wanneer de **Type inkomsten** van een taak **Rol Uur**, Workfront vermenigvuldigt de **Werkelijke uren** op de taak met de factureringssnelheid van de aan de taak toegewezen taakrollen om de **Werkelijke ontvangsten**. Werkelijke uren zijn uren die rechtstreeks bij de taak zijn geregistreerd.

* In het geval van meerdere overschrijvingen van factureringssnelheden, gebruikt Workfront de factureringssnelheid van de taakrol waarvan het tijdkader overeenkomt met de **Invoerdatum** van de uren die voor de taak worden geregistreerd om te berekenen **Werkelijke ontvangsten**.

* Omdat er geen tijdstempel aanwezig is op het tabblad **Invoerdatum** van geregistreerde uren en er is geen tijdstempel op de datumwaaiers van veelvoudige het facturerings tarief met voeten treedt; **Werkelijke ontvangsten** de tijdzone die aan gebruikers is gekoppeld, heeft geen invloed op de berekeningen.

Voor meer informatie over welke functie wordt gebruikt om te berekenen **Werkelijke ontvangsten**, zie de &quot;Begrijpende sectie van de Berekeningen van de Ontvangsten voor Taken die op Gebruiker en de Toewijzingen van de Rol&quot;in het artikel worden gebaseerd [Overzicht van facturering en inkomsten](../../../manage-work/projects/project-finances/billing-and-revenue-overview.md).

## Projectfinanciën opnieuw berekenen

De financiën worden berekend op een project aangezien de veranderingen in de uren voorkomen die voor het project worden geregistreerd.

Als de tarieven tijdens de duur van een project worden veranderd, kunt u kosten en opbrengsten op het project manueel herberekenen, door de optie van de Financiën van de Herberekening op een project te gebruiken. Daarnaast wordt door sommige handelingen een automatische herberekening gestart.

Zie het artikel voor meer informatie over het opnieuw berekenen van projectfinanciën [Projectfinanciën opnieuw berekenen](../../../manage-work/projects/project-finances/recalculate-project-finances.md).

## Een nieuwe factureringssnelheid toevoegen met behulp van de API

Als u een nieuwe factureringssnelheid voor een taakrol wilt toevoegen met de API, voert u een *setRatesForRole* actie voor de **Snelheid** object gebruiken *Methode PUT*.
De handeling en de datumvelden op het tabblad **Snelheid** -object beschikbaar in API-versie 8.0. Als u reeds verscheidene het factureren tarieven voor een baanrol op een project hebt bepaald en u een nieuw het facturerings tarief voor het met een nieuwe datumwaaier wilt toevoegen, moet u zowel het bestaande tarief als het tarief omvatten dat in de zelfde API vraag moet worden toegevoegd. Dit is vergelijkbaar met de manier waarop u verzamelingen voor objecten bijwerkt.

De volgende API-aanroep is een voorbeeld van **attachableID** is de **Project-id** van het project waar u het tarief toevoegt en **RoleID** is de **Functie-id** waarvoor u het nieuwe factureringstarief toevoegt.<pre>{</pre><pre>&quot;attachableID&quot;:&quot;593f01500000557d75fdd4fdfcc624f2&quot;,</pre><pre>&quot;attachableObjCode&quot;:&quot;PROJ&quot;,</pre><pre>&quot;roleID&quot;:&quot;544820df00014148cda5136d4b79d09&quot;, </pre><pre>&quot;tarieven&quot;:[</pre><pre>         {&quot;rateValue&quot;:&quot;0.00&quot;,&quot;startDate&quot;:null,&quot;endDate&quot;:&quot;2017-06-11&quot;},</pre><pre>         {&quot;rateValue&quot;:&quot;45.00&quot;,&quot;startDate&quot;:&quot;2017-06-12&quot;,&quot;endDate&quot;:&quot;2017-06-17&quot;},</pre><pre>         {&quot;rateValue&quot;:&quot;95.00&quot;,&quot;startDate&quot;:&quot;2017-06-21&quot;,&quot;endDate&quot;:null}</pre><pre>]</pre><pre>}</pre>Zie het artikel voor meer informatie over het gebruik van de Workfront API [API-basisbeginselen](https://experience.workfront.com/s/article/API-Basics-638808549).
