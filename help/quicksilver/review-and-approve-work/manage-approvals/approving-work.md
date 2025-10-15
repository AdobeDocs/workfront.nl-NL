---
product-area: projects
navigation-topic: approvals
title: Goedkeuring van de werkzaamheden
description: Goedkeuring van de werkzaamheden
author: Courtney
feature: Work Management, Digital Content and Documents
exl-id: 6e43edbb-14dd-493d-a76b-84be6c3bef82
source-git-commit: 628f668f0c5df34eb967729224d91a28cebbb17c
workflow-type: tm+mt
source-wordcount: '843'
ht-degree: 0%

---

# Goedkeuring van de werkzaamheden

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE:&nbsp;From&nbsp;Courtney: Linked to Training sites/ articles , don't change title and link)</p>
-->

Als u als fiatteur wordt geplaatst, zou u regelmatig moeten herzien welk werk in afwachting van uw goedkeuring is.

Voor informatie over het creëren van goedkeuringsprocessen, zie [&#x200B; een goedkeuringsproces voor het werkpunten &#x200B;](../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-approval-processes.md) creëren.

Voor informatie over het associëren van goedkeuringen met het werk in Workfront, zie [&#x200B; een nieuw of bestaand goedkeuringsproces met het werk &#x200B;](../../review-and-approve-work/manage-approvals/associate-approval-with-work.md) associëren.

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
   <td role="rowheader">Adobe Workfront-licentie</td> 
   <td> 
   <p>Medewerker of hoger</p>
   <p>Controleren of hoger</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraties op toegangsniveau</td> 
   <td> <p>Toegang tot de objecten die aan goedkeuringen zijn gekoppeld weergeven of vergroten</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objectmachtigingen</td> 
   <td> <p>Machtigingen weergeven of hoger voor objecten die zijn gekoppeld aan goedkeuringen</p></td> 
  </tr> 
 </tbody> 
</table>

Voor informatie, zie [&#x200B; vereisten van de Toegang in de documentatie van Workfront &#x200B;](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Goedkeuringen zoeken in Adobe Workfront

U kunt goedkeuringen bekijken en beheren in verschillende gebieden van Workfront.

Voor meer informatie over het bekijken van punten die op goedkeuring wachten of punten die u voor goedkeuring zelf hebt voorgelegd, zie [&#x200B; goedkeuringen van de Mening &#x200B;](../../review-and-approve-work/manage-approvals/view-approvals.md).

## Werk goedkeuren vanuit het thuisgebied

1. Klik het **[!UICONTROL Main Menu]** ![&#x200B; Belangrijkste pictogram van het Menu &#x200B;](assets/main-menu-icon.png) in de hoger-juiste hoek, dan klik **[!UICONTROL Home]**.
1. (Voorwaardelijk) klik **aanpassen** om **Mijn goedkeurt** widget toe te voegen.
1. (Voorwaardelijk) klik het **drop-down menu van de Filter**, dan selecteer **allen** om goedkeuringen te zien die aan u worden toegewezen en worden gedelegeerd.

   >[!NOTE]
   >
   >Goedkeuringen die zijn toegewezen aan taakrollen of -groepen worden niet weergegeven in Home. De goedkeuringen die aan de vertoning van Teams in Mijn widget Goedkeuren voor elk teamlid worden toegewezen.


1. Selecteer het item waarop u een goedkeuringsbesluit wilt nemen.

   ![&#x200B; Mijn widget goedkeurt &#x200B;](assets/my-approvals-widget.png)

1. Klik op een van de beschikbare opties wanneer u een goedkeuringsbesluit neemt in het rechterdeelvenster. De volgende opties worden in de rechterbovenhoek van de pagina weergegeven, afhankelijk van het type item dat u goedkeurt:

   <table>
   <tr>
      <td>
      <p><strong>Toegang</strong></p>
      </td>
      <td>
      <p><strong>Werkitems</strong></p>
      </td>
      <td>
      <p><strong>Documenten</strong></p>
      </td>
      <td>
      <p><strong>Proefdrukken</strong></p>
      </td>
   </tr>
   <tr>
      <td>
       <ul>
      <li>Subsidie</li>
      <li>Negeren</li>
      </ul>
      U kunt het niveau van toegang in het <b> toegang van de Verandering </b> drop-down menu indien gewenst aanpassen.
      </td>
      <td>
         <ul>
         <li>Goedkeuren</li>
         <li>Afwijzen</li>
         </ul>
      U kunt een commentaar met uw besluit verlaten door het drop-down menu in de beslissingsknoop te klikken.
      </td>
      <td>
   Toegewezen als fiatteur
         <ul>
         <li>Goedkeuren</li>
         <li>Goedkeuren met wijzigingen</li>
         <li>Werking vereist</li>
         </ul>
   Toegewezen als revisor
         <ul>
         <li>Mijn revisie voltooien</li>
         </ul>
      De opties in deze kolom zijn slechts op Verenigde Goedkeuringen van toepassing. Goedkeuringen van oudere documenten zijn hetzelfde als goedkeuringen van werkitems. 
      </td>
      <td>
         <ul>
         <li>Ga naar proefdruk</li>
         </ul>
         U neemt uw besluit in de bewijsviewer. Voor informatie over het herzien van een proef, zie <a href="../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/review-proofs-in-wf.md"> proefdrukken van het Overzicht binnen Adobe Workfront </a>.
      </td>
   </tr>
   </table>

Nadat u een beslissing hebt genomen, wordt de goedkeuring verwijderd uit de Mijn widget Goedkeuring.


## Het werk rechtstreeks vanuit een project, taak of probleem goedkeuren

Wanneer een project, een taak, of een kwestie goedkeuring in afwachting zijn, kunt u de goedkeuring direct van het project goedkeuren of verwerpen, de taak, of de kwestie. U kunt ook details bekijken over het goedkeuringsproces.

Om het werk van een project, een taak, of een kwestie direct goed te keuren:

1. Ga naar het project, de taak, of de kwestie die uw goedkeuring vereist.

   De informatie van de goedkeuring betreffende het huidige goedkeuringsproces van een project, een taak, of een kwestie toont in de kopbal van het punt.

   ![&#x200B; Huidige goedkeuringsproces in projectkopbal &#x200B;](assets/current-approval-process-in-project-header-with-stages-nwe-350x92.png)

   De volgende goedkeuringsinformatie is beschikbaar:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Status</td> 
      <td>De huidige status van het project, de taak of de uitgave. Dit is de huidige status van het item dat in afwachting is van de goedkeuring. De status wordt goedgekeurd nadat elke fase van het goedkeuringsproces is goedgekeurd.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Goedkeuringsfasen</td> 
      <td>De fasen van het goedkeuringsproces. <br> het huidige stadium dat goedkeuring in afwachting is wordt getoond zoals In behandeling. De stadia die reeds zijn goedgekeurd worden getoond als Goedgekeurd; de stadia die nog niet zijn goedgekeurd worden getoond als niet Begonnen.</td> 
     </tr> 
    </tbody> 
   </table>

1. Klik **goedkeuren** of **Weigeren**, afhankelijk van of u het goedkeuringsproces wilt goedkeuren of verwerpen.\
   De goedkeuringsfase die in afwachting was van de goedkeuring wordt nu goedgekeurd en de goedkeuringsprocedure gaat naar de volgende fase. De status wordt goedgekeurd nadat alle fasen zijn goedgekeurd.

## Een document rechtstreeks vanuit een document goedkeuren

1. Ga naar het documentgebied dat het document bevat dat uw goedkeuring vereist.
1. Selecteer het document, dan klik **goedkeuren**, **Veranderingen**, of **verwerpen**.\
   ![&#x200B; keur document &#x200B;](assets/approval-approve-document-350x215.png) goed\
   ![&#x200B; de goedkeuring van het Document &#x200B;](assets/document-approval-350x199.png)

1. (Facultatief) als een proef voor het document is geproduceerd, kunt u het document binnen de het proeven interface goedkeuren, zoals die in [&#x200B; wordt beschreven een document van een proef &#x200B;](#approve-a-document-from-a-proof) goedkeuren.

## Een document goedkeuren via een e-mailbericht voor goedkeuring

Afhankelijk van uw berichtinstellingen ontvangt u mogelijk e-mailberichten waarin u op de hoogte wordt gesteld van documenten waarvoor andere gebruikers u nodig hebben om een goedkeuringsbesluit te nemen. Wanneer u een e-mail ontvangt die a **bevat maak de knoop van het Besluit van de Goedkeuring**, kunt u het goedkeuringsproces van e-mail direct beginnen:

1. Van e-mail, klik **maken het Besluit van de Goedkeuring** om de pagina van de Details van het Document voor de proef te openen.
1. Voer een van de volgende handelingen uit om het document te reviseren:

   * De metagegevens van het document weergeven.
   * Als een bewijs voor het herzien van het document met prijsverhoging en commentaren is gecreeerd, klik **Open proef** ![&#x200B; Open proef &#x200B;](assets/open-proof-icon-qs.png) dichtbij de hogere juiste hoek en herzie de proef.

     <!--   
     <span style="color: #ff1493;" data-mc-conditions="QuicksilverOrClassic.Draft mode">[Andrzej, does it make sense to leave this here if it's s document approval?&nbsp;Would there never be a proof in that situation?]</span>   
     -->

     Voor informatie over het herzien van proeven, zie [&#x200B; proefdrukken van het Overzicht binnen Adobe Workfront &#x200B;](../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/review-proofs-in-wf.md).

1. Klik de optie van het a **Besluit** in de hogere juiste hoek om, met veranderingen goed te keuren, goed te keuren of het document te verwerpen.

## Een document op basis van een bewijs goedkeuren {#approve-a-document-from-a-proof}

U kunt een document goedkeuren in de proefdrukviewer. Voor meer informatie, zie [&#x200B; een besluit over een bewijs in de het proeven kijker &#x200B;](../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/make-a-decision-on-a-proof/make-decisions-on-proof.md) in het artikel [&#x200B; nemen een besluit over een bewijs in de het proef kijker &#x200B;](../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/make-a-decision-on-a-proof/make-decisions-on-proof.md).
