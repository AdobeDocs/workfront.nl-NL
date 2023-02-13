---
product-area: projects
navigation-topic: approvals
title: Goedkeuring van de werkzaamheden
description: Goedkeuring van de werkzaamheden
author: Courtney
feature: Work Management
exl-id: 6e43edbb-14dd-493d-a76b-84be6c3bef82
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '1134'
ht-degree: 0%

---

# Goedkeuring van de werkzaamheden

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE:&nbsp;From&nbsp;Courtney: Linked to Training sites/ articles , don't change title and link)</p>
-->

Als u als fiatteur wordt geplaatst, zou u regelmatig moeten herzien welk werk in afwachting van uw goedkeuring is.

Voor informatie over het maken van goedkeuringsprocessen raadpleegt u [Een goedkeuringsproces voor werkitems maken](../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-approval-processes.md).

Voor informatie over het koppelen van goedkeuringen aan werk in Workfront raadpleegt u [Een nieuw of bestaand goedkeuringsproces koppelen aan werk](../../review-and-approve-work/manage-approvals/associate-approval-with-work.md).

## Toegangsvereisten

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
   <td> <p>Controleren of hoger</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraties op toegangsniveau*</td> 
   <td> <p>Toegang tot de objecten die aan goedkeuringen zijn gekoppeld weergeven of vergroten</p> <p>Opmerking: Als u nog steeds geen toegang hebt, vraagt u de Workfront-beheerder of deze aanvullende beperkingen op uw toegangsniveau instelt. Voor informatie over hoe een beheerder van Workfront uw toegangsniveau kan wijzigen, zie <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Aangepaste toegangsniveaus maken of wijzigen</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objectmachtigingen</td> 
   <td> <p>Machtigingen weergeven of hoger voor objecten die zijn gekoppeld aan goedkeuringen</p> <p>Voor informatie over het aanvragen van aanvullende toegang raadpleegt u <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Toegang tot objecten aanvragen </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Neem contact op met uw Workfront-beheerder om te weten te komen welk plan, licentietype of toegang u hebt.

## Goedkeuringen zoeken in Adobe Workfront

U kunt goedkeuringen bekijken en beheren in verschillende gebieden van Workfront.

Voor meer informatie over het bekijken van objecten die wachten op goedkeuring of onderdelen die u zelf ter goedkeuring hebt ingediend, raadpleegt u [Goedkeuringen weergeven](../../review-and-approve-work/manage-approvals/view-approvals.md).

## Werk goedkeuren vanuit het thuisgebied

1. Klik op de knop **Home** pictogram ![](assets/home-icon-30x29.png) in de linkerbovenhoek van Adobe Workfront.

   >[!NOTE]
   >
   >Uw Workfront-beheerder kan de volgende wijzigingen aanbrengen in het pictogram Home in uw omgeving:
   >
   >   
   >* Vervang deze door een afbeelding die is aangepast om uw organisatie te illustreren. In dit geval ziet het pictogram er anders uit dan in dit artikel.
   >* De gekoppelde pagina vervangen door een andere pagina. Klik in dit geval op de knop **Hoofdmenu** ![](assets/main-menu-icon.png) in de rechterbovenhoek van de pagina klikt u op **Home**.


1. Klik op de knop **Filter** vervolgkeuzemenu.

   ![](assets/displaying-work-items-filters-nwe-350x401.png)

1. Selecteren **Goedkeuringen**.\
   Alle werkitems waarvoor goedkeuring is vereist, worden weergegeven. 

   >[!NOTE]
   >
   >Goedkeuringen die zijn toegewezen aan taakrollen of -groepen worden niet weergegeven in Home. De goedkeuringen die aan Teams worden toegewezen tonen in de Groep van het Verzoek van het Team in de Lijst van het Werk.

1. (Optioneel) Wijzig de volgorde waarin goedkeuringen worden weergegeven, zoals wordt beschreven in de sectie &#39;Groep en sorteren op datum, project of prioriteit&#39; in het artikel [Items weergeven in de werklijst in het gebied Home](../../workfront-basics/using-home/using-the-home-area/display-items-in-home-work-list.md).
1. Selecteer het item waarop u een goedkeuringsbesluit wilt nemen.

   ![](assets/task-approval-home-350x127.png)

1. Klik op een van de beschikbare opties wanneer u een goedkeuringsbesluit neemt in het rechterdeelvenster. De volgende opties worden in de rechterbovenhoek van de pagina weergegeven, afhankelijk van het type item dat u goedkeurt:

   * **Projecten:** Klikken **Goedkeuren** of **Afwijzen**.

   * **Taken:** Klikken **Goedkeuren** of **Afwijzen** .

   * **Problemen:** Klikken **Goedkeuren** of **Afwijzen** .

   * **Timesheets:** Klikken **Goedkeuren** of **Afwijzen** .

   * **Documenten:** Klikken **Goedkeuren**, **Afwijzen**, of **Wijzigingen**.\
       Houd rekening met het volgende wanneer u goedkeuringen weergeeft:

      * Hier worden proefdrukken van goedkeuringen weergegeven wanneer een gebruiker een proefdruk met u deelt, zoals wordt beschreven in de sectie &quot;Een proefdrukkoppeling delen&quot; in het artikel [Een proefdruk delen in Adobe Workfront](../../review-and-approve-work/proofing/managing-proofs-within-workfront/share-a-proof-in-workfront.md).
      * Goedkeuringen voor proefdrukken worden alleen weergegeven in het gedeelte Home als uw Workfront-omgeving is geïntegreerd met een Workfront Proof Premium-account. Neem contact op met de Workfront-beheerder als u geen gebruik kunt maken van de hier beschreven proefdrukken.
      * U ontvangt een melding in de app waarin u op de hoogte wordt gebracht van de goedkeuring voor proefdrukken.\
         Voor meer informatie over meldingen in de app raadpleegt u [Meldingen in apps weergeven en beheren](../../workfront-basics/using-notifications/view-and-manage-in-app-notifications.md).

      * De naam van de gebruiker die goedkeuring heeft aangevraagd, wordt weergegeven naast de miniatuurafbeelding in het gebied Home, met de volgende tekst:\
         &quot;*Gebruiker A* graag uw goedkeuring op...&quot;

         <!--      
        <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">      
        (NOTE:&nbsp;From&nbsp;Courtney: Is this true?)      
        </MadCap:conditionalText>      
        -->

         Als de gebruikersnaam niet beschikbaar is, wordt de volgende tekst weergegeven:\
         &quot;Een nieuwe versie van een proefdruk kan worden weergegeven&quot;
      * Als u een goedkeuringsbesluit wilt nemen over het bewijs, klikt u op **Ga naar proefafdruk**, klikt u op **Revisie voltooien** en klikt u op een van de beschikbare opties. De beschikbare opties voor het goedkeuren van een proefdruk zijn: **Goedgekeurd**, **Goedgekeurd met wijzigingen**, **Vereiste wijzigingen**, en **Niet relevant**.

      * Nadat een besluit is genomen op het bewijs, blijft het bewijs op het tabblad Mijn goedkeuringen staan met de tekst &quot;Beslissing gemaakt&quot; totdat u klikt op het tabblad **Vernieuwen** of totdat u de browserpagina vernieuwt.

         Voor informatie over het bekijken van een bewijs raadpleegt u [Proefversies bekijken in Adobe Workfront](../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/review-proofs-in-wf.md).
   * **Toegang:** Selecteer in het dialoogvenster **Toegang wijzigen** vervolgkeuzemenu en vervolgens op **Toegang verlenen**. Of klik op **Negeren**.


## Het werk rechtstreeks vanuit een project, taak of probleem goedkeuren

Wanneer een project, een taak, of een kwestie goedkeuring in afwachting zijn, kunt u de goedkeuring direct van het project goedkeuren of verwerpen, de taak, of de kwestie. U kunt ook details bekijken over het goedkeuringsproces.

Om het werk van een project, een taak, of een kwestie direct goed te keuren:

1. Ga naar het project, de taak, of de kwestie die uw goedkeuring vereist.

   De informatie van de goedkeuring betreffende het huidige goedkeuringsproces van een project, een taak, of een kwestie toont in de kopbal van het punt.

   ![](assets/current-approval-process-in-project-header-with-stages-nwe-350x92.png)

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
      <td>De fasen van het goedkeuringsproces. <br>Het huidige stadium dat goedkeuring in afwachting is wordt getoond zoals In behandeling. De stadia die reeds zijn goedgekeurd worden getoond zoals Goedgekeurd; als Niet gestart worden weergegeven, worden stappen weergegeven die nog niet zijn goedgekeurd.</td> 
     </tr> 
    </tbody> 
   </table>

1. Klikken **Goedkeuren** of **Afwijzen**, afhankelijk van de vraag of u het goedkeuringsproces wilt goedkeuren of afwijzen.\
   De goedkeuringsfase die in afwachting was van de goedkeuring wordt nu goedgekeurd en de goedkeuringsprocedure gaat naar de volgende fase. De status wordt goedgekeurd nadat alle fasen zijn goedgekeurd.

## Een document rechtstreeks vanuit een document goedkeuren 

1. Ga naar het documentgebied dat het document bevat dat uw goedkeuring vereist.
1. Selecteer het document en klik op **Goedkeuren**, **Wijzigingen**, of **Afwijzen**.\
   ![](assets/approval-approve-document-350x215.png)\
   ![](assets/document-approval-350x199.png)

1. (Optioneel) Als een proefdruk voor het document is gegenereerd, kunt u het document goedkeuren in de interface voor proefdrukken, zoals beschreven in [Een document op basis van een bewijs goedkeuren](#approve-a-document-from-a-proof).

## Een document goedkeuren via een e-mailbericht voor goedkeuring

Afhankelijk van uw berichtinstellingen ontvangt u mogelijk e-mailberichten waarin u op de hoogte wordt gesteld van documenten waarvoor andere gebruikers u nodig hebben om een goedkeuringsbesluit te nemen. Wanneer u een e-mail ontvangt met een **Goedkeuringsbesluit maken** kunt u het goedkeuringsproces rechtstreeks starten via e-mail:

1. Klik in het e-mailbericht op **Goedkeuringsbesluit maken** om de pagina Documentdetails voor de proefdruk te openen.
1. Voer een van de volgende handelingen uit om het document te reviseren:

   * De metagegevens van het document weergeven.
   * Als er een proefdruk is gemaakt voor het reviseren van het document met opmaakcodes en opmerkingen, klikt u op **Proef openen** ![](assets/open-proof-icon-qs.png) in de rechterbovenhoek en bekijk de proefdruk.

      <!--   
     <span style="color: #ff1493;" data-mc-conditions="QuicksilverOrClassic.Draft mode">[Andrzej, does it make sense to leave this here if it's s document approval?&nbsp;Would there never be a proof in that situation?]</span>   
     -->

      Voor informatie over het controleren van proefdrukken raadpleegt u [Proefversies bekijken in Adobe Workfront](../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/review-proofs-in-wf.md).

1. Klik op een **Besluit** in de rechterbovenhoek om het document goed te keuren, goed te keuren met wijzigingen of af te wijzen.

## Een document op basis van een bewijs goedkeuren {#approve-a-document-from-a-proof}

U kunt een document goedkeuren in de proefdrukviewer. Zie voor meer informatie [Beslissen op een bewijs in de professionele drukker](../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/make-a-decision-on-a-proof/make-decisions-on-proof.md) in het artikel [Beslissen op een bewijs in de professionele drukker](../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/make-a-decision-on-a-proof/make-decisions-on-proof.md).
