---
title: Verzoeken kopiëren en verzenden
description: Wanneer u regelmatig vergelijkbare verzoeken indient, kunt u een bestaand verzonden verzoek kopiëren. In dit geval kunt u een bestaande aanvraag kopiëren, er minimale wijzigingen in aanbrengen en deze opnieuw verzenden als een nieuw verzoek.
author: Becky
feature: Work Management
role: User
topic: Collaboration
exl-id: 3d7581d0-e99c-4204-b1e5-04fde72251bb
source-git-commit: b58814d68d582a08457d1d4685d110c2bdd2087c
workflow-type: tm+mt
source-wordcount: '1517'
ht-degree: 0%

---

# Verzoeken kopiëren en verzenden


Wanneer u regelmatig vergelijkbare verzoeken indient, kunt u een bestaand verzonden verzoek kopiëren. In dit geval kunt u een bestaande aanvraag kopiëren, er minimale wijzigingen in aanbrengen en deze opnieuw verzenden als een nieuw verzoek.

## Toegangsvereisten

+++ Breid uit om de toegangseisen voor de functionaliteit in dit artikel weer te geven.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-pakket</td> 
   <td> <p>Alle </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-licentie</td> 
   <td> <p>Medewerker of hoger</p>
   <p>Aanvraag of hoger</p>
    </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraties op toegangsniveau</td> 
   <td> <p>Toegang tot problemen bewerken</p>  </td> 
  </tr> 
  <tr>
   <td role="rowheader">Objectmachtigingen</td> 
   <td><p>Toegang tot het toevoegen van verzoeken aan een aanvraagwachtrij</p> <p>De toestemmingen van de mening of hoger op het bestaande verzoek</p> <p>Voor informatie bij vestiging ziet een verzoekrij, <a href="../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md" class="MCXref xref"> een Rij van het Verzoek </a> creëren. </p> </td> 
  </tr>
  <tr> 
   <td role="rowheader"> Product</td> 
   <td> <ul><li>Adobe Workfront</li><li>U moet Adobe Workfront Planning hebben om de verzoeken van de Planning te bekijken of om formulieren te verzoeken</td> 
  </tr> 
 </tbody> 
</table>

Voor informatie, zie [&#x200B; vereisten van de Toegang in de documentatie van Workfront &#x200B;](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Vereisten

U moet een verzoek hebben dat u of iemand in uw organisatie eerder heeft ingediend om het te kunnen kopiëren en opnieuw verzenden. Als het verzoek van iemand anders is, moet u ten minste toegang hebben tot Beeld om het als nieuw te kunnen kopiëren en verzenden.

## Overwegingen bij het kopiëren en verzenden van verzoeken als nieuwe

* U kunt alleen ingediende aanvragen kopiëren en verzenden. U kunt geen opgestelde verzoeken kopiëren.
* U kunt verzoeken kopiëren en verzenden die u oorspronkelijk hebt verzonden, of verzoeken die anderen hebben verzonden en u hebt toegang tot minimaal Beeld.
* U hebt altijd toegang om een kopie van uw eigen verzoeken te kopiëren en te verzenden, tenzij iemand uw machtigingen heeft verwijderd.
* De toegang om verzoeken te kopiëren en voor te leggen die oorspronkelijk door anderen worden voorgelegd zou automatisch aan mensen in het zelfde bedrijf kunnen worden verleend wanneer de schepper van de verzoekrij de **Mensen van het zelfde bedrijf toelaat zal de zelfde toestemmingen voor alle verzoeken** in de Details van de Rij of zal de gebieden van het Project uitgeven. Als u deze instelling uitschakelt, kan alleen de oorspronkelijke aanvrager zijn of haar eigen verzoeken weergeven.

  Raadpleeg de volgende artikelen voor meer informatie:

   * [&#x200B; creeer een Rij van het Verzoek &#x200B;](../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md)
   * [Projecten bewerken](../../../manage-work/projects/manage-projects/edit-projects.md)

* U kunt de kopie van de oorspronkelijke aanvraag bijwerken voordat u deze opnieuw indient als een nieuwe aanvraag.
* Als de volgende wijzigingen optreden nadat het oorspronkelijke verzoek is verzonden, kunt u het niet meer kopiëren en opnieuw verzenden:

   * De aanvraagwachtrij is verwijderd.
   * Het onderwerp van de wachtrij is verwijderd.

     >[!TIP]
     >
     >Als het rijonderwerp slechts in de verzoekrij was, kunt u nog het verzoek kopiëren en voorleggen en het zal onder de verzoekrij zelf worden bewaard.

   * De verzoekrij wordt niet meer gepubliceerd als Rij van het Verzoek van de Hulp. Voor informatie, zie [&#x200B; een Rij van het Verzoek &#x200B;](../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md) creëren.
   * Als de verzoekrij geen rijonderwerp heeft en het originele verzoek werd voorgelegd vóór Januari 2022.

   * De status van het project verbonden aan de verzoekrij is niet meer Huidig.

* U kunt een kopie van een omgezette aanvraag kopiëren en verzenden als de aanvraag tijdens het conversieproces is behouden. Voor meer informatie, zie [&#x200B; Overzicht van het omzetten van kwesties in Adobe Workfront &#x200B;](../../../manage-work/issues/convert-issues/convert-issues.md).

  >[!TIP]
  >
  >De gekopieerde aanvraag is niet gekoppeld aan een oplossend object.

## Verzoeken in de oudere aanvraagervaring kopiëren en verzenden

{{step1-to-requests}}

1. (Voorwaardelijk) als de Voorgelegde sectie niet door gebrek toont, klik **Voorgelegd** in het linkerpaneel.

   >[!TIP]
   >
   >   Uw Workfront- of groepsbeheerder kan uw lay-outsjabloon aanpassen en gebieden uit het hoofdmenu of uit het linkerdeelvenster in uw omgeving verwijderen. In dit geval zijn ze mogelijk niet beschikbaar voor u.

1. Zoek het verzoek dat u wilt kopiëren en verzenden als nieuw en voer een van de volgende handelingen uit:

   * Selecteer het, dan klik **Exemplaar** ![](assets/copy-and-submit-as-new-requests-area-nwe.png) in de upper-left hoek van de Voorgelegde lijst van verzoeken.

   >[!TIP]
   >
   > Als u niet eerst een aanvraag hebt geselecteerd, wordt het pictogram Kopiëren grijs weergegeven.

   * Klik **Meer** menu ![](assets/more-icon.png) aan het recht van de verzoeknaam, dan klik **Exemplaar en voorlegt als nieuw**

     of

     Klik op het geselecteerde verzoek met de rechtermuisknop aan, dan klik **Exemplaar en verzend als nieuw**.

     ![](assets/request-selected-more-menu-options-nwe-350x191.png)

     >[!TIP]
     >
     >Wanneer u geen toegang hebt om kwesties tot stand te brengen, ontvangt u een waarschuwing dat uw beheerder u van het creëren van verzoeken beperkte.

1. (Optioneel) Werk indien nodig de volgende gegevens bij:

   * **Type van Verzoek**: de verzoekrij waar het gekopieerde verzoek wordt bewaard. Standaard wordt de gekopieerde aanvraag opgeslagen in de wachtrij met aanvragen van de oorspronkelijke aanvraag.
   * **de Groepen van het Onderwerp** en **Onderwerpen van de Rij**, als zij worden geselecteerd. De namen of onderwerpgroepen en rijonderwerpen worden aangepast voor uw milieu. Door gebrek, wordt het gekopieerde verzoek bewaard aan de onderwerpgroepen en de rijonderwerpen van het originele verzoek.

     >[!TIP]
     >
     >Als de weg van de weg van het originele verzoek verandert, dan wijzigde de maker van de verzoekrij de rij.

1. (Optioneel) Werk de gegevens van de gekopieerde aanvraag bij. Afhankelijk van welke gebieden de schepper van de verzoekrij in de **Nieuwe Uitgevende Gebieden** sectie van de Rij **&#x200B;**&#x200B;subtab van de Details van de Rij op het project werd toegelaten, zou u om het even welke volgende gebieden kunnen vinden:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong> Onderwerp </strong> </td> 
      <td>Geeft de naam van de oorspronkelijke aanvraag weer. Werk deze indien nodig bij. Anders, noemt Workfront het gekopieerde verzoek <b> Exemplaar van &lt;Naam van oorspronkelijk verzoek&gt; </b>. Dit is een verplicht veld.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong> Beschrijving </strong> </td> 
      <td>Geeft de beschrijving van de oorspronkelijke aanvraag weer. Werk deze indien nodig bij.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong> URL </strong> </td> 
      <td> <p>Hiermee geeft u de URL van het oorspronkelijke verzoek weer. Werk deze indien nodig bij.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong> Prioriteit </strong> </td> 
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
      <td role="rowheader"><strong> Ernst </strong> </td> 
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
      <td role="rowheader"><strong> Primair Contact </strong> </td> 
      <td>De primaire contactpersoon van een verzoek blijft standaard bij u, aangezien u de puntpersoon bent die vragen met betrekking tot het verzoek behandelt. U kunt dit echter wijzigen in elke andere Workfront-gebruiker.</td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader"><span><strong> Taken </strong></span> </td> 
      <td> <p>Geef de naam op van een actieve gebruiker, taakrol of team waaraan de aanvraag moet worden toegewezen. </p> <p> U kunt meer dan één gebruiker, baanrol, of team specificeren. </p> <p>Afhankelijk van hoe de verzoekrij opstelling was, zou u het verzoek aan één of twee soorten middelen, in plaats van alle drie kunnen slechts toewijzen. </p> <p>Wij adviseren gebruikend het Verpletteren van Regels voor uw Opeenvolging van het Verzoek zodat zij automatisch aan de aangewezen middelen kunnen worden verpletterd. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader" colspan="2"> <p><p style="font-weight: normal;">Afhankelijk van hoe de verzoekrij opstelling was, zou u één type van middel aan het verzoek (bijvoorbeeld, gebruikers) kunnen slechts toewijzen. Als een verpletterende regel ook aan de verzoekrij wordt geassocieerd en het het verzoek aan een verschillend type van middel (bijvoorbeeld, een team) automatisch leidt, wordt uw verzoek toegewezen aan zowel de entiteit die u manueel wanneer het voorleggen van het verzoek (gebruikers) en het middel specificeert in de verpletterende regel (het team).</p> <p style="font-weight: normal;">Raadpleeg de volgende artikelen voor meer informatie:</p> 
        <ul> 
         <li> <p><a href="../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md" class="MCXref xref"> creeer een Rij van het Verzoek </a> </p> </li> 
         <li> <p><a href="../../../manage-work/requests/create-and-manage-request-queues/create-routing-rules.md" class="MCXref xref"> creeer Verpletterend Regels </a> <br> </p> </li> 
        </ul> </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong> Geplande Uren </strong> </td> 
      <td> <p>Schatting hoeveel uren het voor dit verzoek om voltooien zou vergen.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong> Geplande Datum van het Begin </strong> </td> 
      <td> <p>De datum waarop de werkzaamheden aan dit verzoek moeten beginnen.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong> Geplande de Datum van de Voltooiing </strong> </td> 
      <td>De datum waarop u dit verzoek wilt oplossen.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong> Status </strong> </td> 
      <td>De standaardstatus van een nieuw verzoek is "Nieuw." Mogelijk is de naam van deze status gewijzigd door uw Workfront-beheerder. U kunt de status ook wijzigen in iets anders vanuit dit keuzemenu.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong> Documenten </strong> </td> 
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

1. Klik **voorleggen**.

   Het gekopieerde verzoek wordt verzonden als een nieuw verzoek in de aanvraagwachtrij die u hebt opgegeven.

## Verzoeken kopiëren en verzenden met de nieuwe ervaring die u opvraagt

U kunt aanvragen kopiëren en verzenden in het gebied Verzoeken van Workfront of vanuit de widget Mijn verzoeken in Home.

{{step1-to-requests}}

1. Ga als volgt te werk om de widget Mijn verzoeken te openen:

   {{step1-to-home}}

   1. Zoek de widget Mijn verzoeken.

      Voor meer informatie over Mijn widget van Verzoeken, zie [&#x200B; Gebruik Mijn widget van Verzoeken &#x200B;](/help/quicksilver/workfront-basics/using-home/using-the-home-area/my-requests-widget.md).

1. Houd de muisaanwijzer boven de aanvraag die u wilt kopiëren in de lijst Verzoeken of de widget Mijn verzoeken.

   Er verschijnt een menu Meer met drie punten.
   ![](assets/more-menu.png)

1. Klik het **Meer** menu rechts van de verzoeknaam, dan klik **Exemplaar**.

   of

   Klik op het geselecteerde verzoek met de rechtermuisknop aan, dan klik **Exemplaar**.

   >[!TIP]
   >
   >Wanneer u geen toegang hebt om kwesties tot stand te brengen, ontvangt u een waarschuwing dat uw beheerder u van het creëren van verzoeken beperkte.

1. (Optioneel) Werk de gegevens van de gekopieerde aanvraag bij. Welke velden beschikbaar zijn, is afhankelijk van de aanvraagwachtrij of het aanvraagformulier dat voor de aanvraag wordt gebruikt.

   Wanneer u veldwaarden in de gekopieerde aanvraag invoert of wijzigt, wordt deze opgeslagen als concept.

1. Klik **voorleggen**.

   Het gekopieerde verzoek wordt als een nieuw verzoek ingediend.


