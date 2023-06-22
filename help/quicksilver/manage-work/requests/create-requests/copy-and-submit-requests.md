---
title: Verzoeken kopiëren en verzenden
description: Verzoeken kopiëren en verzenden
author: Alina
draft: Probably
feature: Work Management
exl-id: 3d7581d0-e99c-4204-b1e5-04fde72251bb
source-git-commit: cd059c445d86ed5581e8b2cb01507f18b97954f3
workflow-type: tm+mt
source-wordcount: '1309'
ht-degree: 0%

---

# Verzoeken kopiëren en verzenden

<!--<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment.</span> -->

Wanneer u regelmatig vergelijkbare verzoeken verzendt, kunt u een bestaand verzonden verzoek kopiëren. In dit geval kunt u een bestaande aanvraag kopiëren, er minimale wijzigingen in aanbrengen en deze opnieuw verzenden als een nieuw verzoek.

## Toegangsvereisten

<!--drafted - replace table with P&P:

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
   <td><p>Current license: Contributor or higher</p> 
   Or
   <p>Legacy license: Request or higher</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>Edit access to Issues</p> <p><b>NOTE</b> 
   
   If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can modify your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>Access to add requests to a request queue</p> <p>View or higher permissions on the existing request</p> <p>For information on setting up a request queue, see <a href="../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md" class="MCXref xref">Create a Request Queue</a>. </p> </td> 
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
   <td role="rowheader">Adobe Workfront-abonnement*</td> 
   <td> <p>Alle</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-licentie*</td> 
   <td> <p>Aanvraag of hoger</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraties op toegangsniveau*</td> 
   <td> <p>Toegang tot problemen bewerken</p> <p><b>OPMERKING</b>

Als u nog steeds geen toegang hebt, vraagt u de Workfront-beheerder of deze aanvullende beperkingen op uw toegangsniveau instelt. Voor informatie over hoe een beheerder van Workfront uw toegangsniveau kan wijzigen, zie <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Aangepaste toegangsniveaus maken of wijzigen</a>.</p> </td>
</tr> 
  <tr> 
   <td role="rowheader">Objectmachtigingen</td> 
   <td> <p>Toegang tot het toevoegen van verzoeken aan een aanvraagwachtrij</p> <p>De toestemmingen van de mening of hoger op het bestaande verzoek</p> <p>Voor informatie over het instellen van een aanvraagwachtrij raadpleegt u <a href="../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md" class="MCXref xref">Een aanvraagwachtrij maken</a>. </p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Neem contact op met uw Workfront-beheerder om te weten te komen welk plan, licentietype of toegang u hebt.

## Vereisten

U moet een verzoek hebben dat u of iemand in uw organisatie eerder heeft ingediend om het te kunnen kopiëren en opnieuw verzenden. Als het verzoek van iemand anders is, moet u ten minste toegang hebben tot Beeld om het als nieuw te kunnen kopiëren en verzenden.

## Overwegingen bij het kopiëren en verzenden van verzoeken als nieuwe

* U kunt alleen ingediende aanvragen kopiëren en verzenden. U kunt geen opgestelde verzoeken kopiëren.
* U kunt verzoeken kopiëren en verzenden die u oorspronkelijk hebt verzonden, of verzoeken die anderen hebben verzonden en u hebt toegang tot minimaal Beeld.
* U hebt altijd toegang om een kopie van uw eigen verzoeken te kopiëren en te verzenden, tenzij iemand uw machtigingen heeft verwijderd.
* De toegang om verzoeken te kopiëren en voor te leggen die oorspronkelijk door anderen werden voorgelegd zou automatisch aan mensen in het zelfde bedrijf kunnen worden verleend wanneer de schepper van de verzoekrij toelaat **De mensen van het zelfde bedrijf zullen de zelfde toestemmingen voor alle verzoeken erven** in de Details van de Rij of geef de gebieden van het Project uit. Als u deze instelling uitschakelt, kan alleen de oorspronkelijke aanvrager zijn of haar eigen verzoeken weergeven.

  Raadpleeg de volgende artikelen voor meer informatie:

   * [Een aanvraagwachtrij maken](../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md)
   * [Projecten bewerken](../../../manage-work/projects/manage-projects/edit-projects.md)

* U kunt de kopie van de oorspronkelijke aanvraag bijwerken voordat u deze opnieuw indient als een nieuwe aanvraag.
* Als de volgende wijzigingen optreden nadat het oorspronkelijke verzoek is verzonden, kunt u het niet meer kopiëren en opnieuw verzenden:

   * De aanvraagwachtrij is verwijderd.
   * Het onderwerp van de wachtrij is verwijderd.

     >[!TIP]
     >
     >Als het rijonderwerp slechts in de verzoekrij was, kunt u nog het verzoek kopiëren en voorleggen en het zal onder de verzoekrij zelf worden bewaard.

   * De verzoekrij wordt niet meer gepubliceerd als Rij van het Verzoek van de Hulp. Zie voor meer informatie [Een aanvraagwachtrij maken](../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md).
   * Als de verzoekrij geen rijonderwerp heeft en het originele verzoek werd voorgelegd vóór Januari 2022.

   * De status van het project verbonden aan de verzoekrij is niet meer Huidig.

* U kunt een kopie van een omgezette aanvraag kopiëren en verzenden als de aanvraag tijdens het conversieproces is behouden. Zie voor meer informatie [Overzicht van conversie van problemen in Adobe Workfront](../../../manage-work/issues/convert-issues/convert-issues.md).

  >[!TIP]
  >
  >De gekopieerde aanvraag is niet gekoppeld aan een oplossend object.

## Verzoeken kopiëren en verzenden

1. Klik op de knop **Hoofdmenu** pictogram ![](assets/main-menu-icon.png) in de rechterbovenhoek van Adobe Workfront klikt u op **Verzoeken**.
1. (Voorwaardelijk) Als de sectie Verzonden niet standaard wordt weergegeven, klikt u op **Verzonden** in het linkerdeelvenster.
1. Zoek het verzoek dat u wilt kopiëren en verzenden als nieuw en voer een van de volgende handelingen uit:

   * Selecteer het, klik dan het **Kopiëren en verzenden als nieuw** pictogram ![](assets/copy-and-submit-as-new-requests-area-nwe.png) in de linkerbovenhoek van de lijst Ingediende aanvragen. <!--update this icon AND change its name to "Copy" with the 23.3 preview release, or shortly after-->

   <!-- reveal this tip for 23.3 preview release:
   >[!TIP]
   >
   > <span class="preview">If you did not select a request first, the Copy icon is dimmed.</span> 
   -->

   * Klik op de knop **Meer** menu ![](assets/more-icon.png) rechts van de naam van de aanvraag klikt u op **Kopiëren en verzenden als nieuw** <!--ensure this does not change with the Copy icon improvements with 23.3 preview-->

     of

     Klik met de rechtermuisknop op de geselecteerde aanvraag en klik vervolgens op **Kopiëren en verzenden als nieuw**.

     ![](assets/request-selected-more-menu-options-nwe-350x191.png)

     >[!TIP]
     >
     >Wanneer u geen toegang hebt om kwesties tot stand te brengen, ontvangt u een waarschuwing dat uw beheerder u van het creëren van verzoeken beperkte.

1. (Optioneel) Werk indien nodig de volgende gegevens bij:

   * **Type aanvraag**: de verzoekrij waar het gekopieerde verzoek wordt bewaard. Standaard wordt de gekopieerde aanvraag opgeslagen in de wachtrij met aanvragen van de oorspronkelijke aanvraag.
   * **Onderwerpgroepen** en **Onderwerpen van de Rij**, als deze zijn geselecteerd. De namen of onderwerpgroepen en rijonderwerpen worden aangepast voor uw milieu. Door gebrek, wordt het gekopieerde verzoek bewaard aan de onderwerpgroepen en de rijonderwerpen van het originele verzoek.

     >[!TIP]
     >
     >Als het pad verandert van het pad van het oorspronkelijke verzoek, heeft de maker van de aanvraagwachtrij de wachtrij gewijzigd.

1. (Optioneel) Werk de gegevens van de gekopieerde aanvraag bij. Afhankelijk van welke velden de maker van de aanvraagwachtrij in het dialoogvenster **Nieuwe probleemvelden** van de **Wachtrij** subtab op het project, zou u om het even welke volgende gebieden kunnen vinden:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>Onderwerp</strong> </td> 
      <td>Geeft de naam van de oorspronkelijke aanvraag weer. Werk deze indien nodig bij. Anders geeft Workfront de gekopieerde aanvraag een naam <b>Kopie van &lt;name of="" original="" request=""&gt;</b>. Dit is een verplicht veld.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Beschrijving</strong> </td> 
      <td>Geeft de beschrijving van de oorspronkelijke aanvraag weer. Werk deze indien nodig bij.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>URL</strong> </td> 
      <td> <p>Hiermee geeft u de URL van het oorspronkelijke verzoek weer. Werk deze indien nodig bij.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Prioriteit</strong> </td> 
      <td> <p>Geef de prioriteit van uw verzoek op. De prioriteit moet bepalen hoe snel u vindt dat dit verzoek moet worden opgelost. De standaardopties zijn:</p> 
       <ul> 
        <li>Geen</li> 
        <li>Laag</li> 
        <li>Normaal</li> 
        <li>Hoog</li> 
        <li>Dringend</li> 
       </ul> <p>Uw Workfront-beheerder kan de namen van prioriteiten wijzigen.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Ernst</strong> </td> 
      <td> <p>Geef de ernst van uw verzoek op. De ernst moet bepalen welke invloed dit verzoek op uw werk heeft als het niet op tijd wordt opgelost. De standaardopties zijn:</p> 
       <ul> 
        <li>Cosmetisch</li> 
        <li>Verwardheid</li> 
        <li>Fout met tijdelijke oplossing</li> 
        <li>Fout zonder tijdelijke oplossing</li> 
        <li>Fatale fout</li> 
       </ul> <p>Uw Workfront-beheerder kan de namen van de bestandscontroles wijzigen.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Primaire contactpersoon</strong> </td> 
      <td>De primaire contactpersoon van een verzoek blijft standaard bij u, aangezien u de puntpersoon bent die vragen met betrekking tot het verzoek behandelt. U kunt dit echter wijzigen in elke andere Workfront-gebruiker.</td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader"><span><strong>Toewijzingen</strong></span> </td> 
      <td> <p>Geef de naam op van een actieve gebruiker, taakrol of team waaraan de aanvraag moet worden toegewezen. </p> <p> U kunt meer dan één gebruiker, baanrol, of team specificeren. </p> <p>Afhankelijk van hoe de verzoekrij opstelling was, zou u het verzoek aan één of twee soorten middelen, in plaats van alle drie kunnen slechts toewijzen. </p> <p>Wij adviseren gebruikend het Verpletteren van Regels voor uw Opeenvolging van het Verzoek zodat zij automatisch aan de aangewezen middelen kunnen worden verpletterd. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader" colspan="2"> <p><p style="font-weight: normal;">Afhankelijk van hoe de verzoekrij opstelling was, zou u één type van middel aan het verzoek (bijvoorbeeld, gebruikers) kunnen slechts toewijzen. Als een verpletterende regel ook aan de verzoekrij wordt geassocieerd en het het verzoek aan een verschillend type van middel (bijvoorbeeld, een team) automatisch leidt, wordt uw verzoek toegewezen aan zowel de entiteit die u manueel wanneer het voorleggen van het verzoek (gebruikers) en het middel specificeert in de verpletterende regel (het team).</p> <p style="font-weight: normal;">Raadpleeg de volgende artikelen voor meer informatie:</p> 
        <ul> 
         <li> <p><a href="../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md" class="MCXref xref">Een aanvraagwachtrij maken</a> </p> </li> 
         <li> <p><a href="../../../manage-work/requests/create-and-manage-request-queues/create-routing-rules.md" class="MCXref xref">Verpletterende regels maken</a> <br> </p> </li> 
        </ul> </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Geplande uren</strong> </td> 
      <td> <p>Schatting hoeveel uren het voor dit verzoek om voltooien zou vergen.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Geplande begindatum</strong> </td> 
      <td> <p>De datum waarop de werkzaamheden aan dit verzoek moeten beginnen.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Geplande afsluitdatum</strong> </td> 
      <td>De datum waarop u dit verzoek wilt oplossen.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Status</strong> </td> 
      <td>De standaardstatus van een nieuw verzoek is "Nieuw." Mogelijk is de naam van deze status gewijzigd door uw Workfront-beheerder. U kunt de status ook wijzigen in iets anders vanuit dit keuzemenu.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Documenten</strong> </td> 
      <td> <p>Voeg documenten toe aan uw verzoek. De documenten die bij het oorspronkelijke verzoek zijn gevoegd, worden niet naar het gekopieerde verzoek overgedragen.</p> <p><b>TIP</b>

   Afhankelijk van hoe de verzoekrij opstelling was, zou de sectie van Documenten vóór of na de douanevelden kunnen tonen.</p> <p> </p> </td>
   </tr> 
    </tbody> 
   </table>

1. (Optioneel) Werk indien nodig alle gegevens in de bijgevoegde aangepaste formulieren bij.

   >[!TIP]
   >
   >* Alle aangepaste formulieren die bij de oorspronkelijke aanvraag horen en de waarden in de aangepaste velden worden naar de gekopieerde aanvraag overgebracht. Dit geldt ook voor velden die logica bevatten.
   >* U kunt geen aangepaste formulieren uit de gekopieerde aanvraag verwijderen.

1. Klikken **Verzenden**.

   Het gekopieerde verzoek wordt verzonden als een nieuw verzoek in de aanvraagwachtrij die u hebt opgegeven.
