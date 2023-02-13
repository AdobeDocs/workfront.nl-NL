---
product-area: documents
navigation-topic: review-proofs-within-workfront
title: Meldingen beheren voor proefopmerkingen en -beslissingen
description: Wanneer u aan een proefdruk werkt, of u een gebruiker van Adobe Workfront of een externe medewerker bent, kunt u specificeren welke e-mailberichten u over commentaren en besluiten over de proefdruk wilt ontvangen. Voor meer informatie, zie Berichten voor het proefdrukcommentaren en besluitoverzicht.
author: Courtney
feature: Digital Content and Documents
exl-id: c38e005c-8984-4e99-9527-94a0a6b1071d
source-git-commit: 49950895440fec8cebdf12ec81191c6e890383cf
workflow-type: tm+mt
source-wordcount: '983'
ht-degree: 0%

---

# Meldingen beheren voor proefopmerkingen en -beslissingen

Wanneer u aan een proefdruk werkt, of u een gebruiker van Adobe Workfront of een externe medewerker bent, kunt u specificeren welke e-mailberichten u over commentaren en besluiten over de proefdruk wilt ontvangen. Zie voor meer informatie [Kennisgevingen met betrekking tot opmerkingen ter staving en besluiten](../../../review-and-approve-work/proofing/proofing-overview/notifications-proof-comments-decisions.md).

>[!NOTE]
>
>Deze meldingen verschillen van de e-mailwaarschuwingen die u kunt ontvangen over de stroom van een proefdruk onder controleurs. Ze verschillen ook van de instellingen voor e-mailwaarschuwingen die u kunt configureren in Workfront. 

## Toegangsvereisten

U moet de volgende toegang hebben om de stappen in dit artikel uit te voeren:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-abonnement*</td> 
   <td> <p>Huidig plan: Pro of hoger</p> <p>of</p> <p>Ouder plan: Selecteren of Premium</p> <p>Voor meer informatie over het proefdrukken van toegang met de verschillende plannen, zie <a href="/help/quicksilver/administration-and-setup/manage-workfront/configure-proofing/access-to-proofing-functionality.md" class="MCXref xref">Toegang tot proefdrukfunctionaliteit in Workfront</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-licentie*</td> 
   <td> <p>Huidig plan: Werken of plannen</p> <p>Ouder plan: Willekeurig (proefdrukken moet zijn ingeschakeld voor de gebruiker)</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Bewijs van machtigingsprofiel </td> 
   <td>Manager of hoger</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraties op toegangsniveau*</td> 
   <td> <p>Toegang tot documenten bewerken</p> <p>Voor informatie over het aanvragen van aanvullende toegang raadpleegt u <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Toegang tot objecten aanvragen </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Neem contact op met de beheerder van de Workfront of Workfront-proefdrukken als u wilt weten welk plan, welke rol of welk proefdrukprofiel u hebt.

## Meldingen beheren voor proefopmerkingen en -beslissingen

1. Open de proefdruk waarvoor u berichten wilt vormen u zult ontvangen.
1. Als de linkerwerkbalk niet wordt weergegeven, klikt u op de knop **Menu** in de linkerbovenhoek van de Web Proofing Viewer.

   ![Menu_icon_in_Proofing_Viewer.png](assets/menu-icon-in-proofing-viewer-350x228.png)

1. Klik op de linkerwerkbalk op de knop **Instellingen** pictogram. ![Settings_icon.png](assets/settings-icon.png)

1. Onder **Stuur me e-mailberichten over** klikt u op de gewenste instelling voor de proefdruk.

   De instelling die u selecteert, blijft alleen van kracht voor de proefdruk die u hebt geopend.

   Het systeemgebrek is **Dagelijkse samenvatting**. Als u of uw controleurs geen andere wijzigingen aanbrengen, hebben al uw proefdrukken deze instelling.

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Alle activiteiten</td> 
      <td>Telkens wanneer er activiteiten aan het bewijs worden toegevoegd, zoals een nieuwe opmerking, een nieuw antwoord of een nieuw besluit, wordt er een e-mail naar de controleur verzonden.<br><p>Dit is een goede optie voor de persoon die het proefdrukproces beheert omdat het hen toestaat om de activiteit te zien aangezien het gebeurt. Gebruikers ontvangen geen e-mailwaarschuwing over hun eigen activiteiten (bijvoorbeeld opmerkingen, antwoorden en beslissingen).</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">Reacties op mijn opmerkingen</td> 
      <td>Een e-mail wordt alleen naar de controleur verzonden als iemand uitdrukkelijk op zijn opmerking reageert (dit sluit zijn eigen reacties op zijn eigen opmerkingen uit). Dit betekent dat als iemand op het bewijs een nieuwe opmerking maakt, de controleur niet op de hoogte wordt gesteld.<p>Deze instelling wordt aanbevolen voor uw klanten op de proefdruk, zodat zij geen andere opmerkingen over de proefdruk ontvangen en alleen op de hoogte worden gesteld van antwoorden op hun eigen opmerkingen.</p><p>Hoewel revisoren met deze instelling voor e-mailwaarschuwingen geen melding krijgen van andere nieuwe opmerkingen, kunnen ze alle opmerkingen over de proefdrukken wel bekijken in de proefdrukviewer.<br></p><p>Zie voor meer informatie <a href="../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/comment-on-a-proof/view-proof-comments.md" class="MCXref xref">Opmerkingen over proefdrukken weergeven en beantwoorden</a>.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">Besluiten</td> 
      <td>Een e-mail wordt alleen naar de controleur verzonden wanneer iemand een beslissing neemt.<br><p>Deze e-mailwaarschuwing kan nuttig zijn voor de persoon die het goedkeuringsproces beheert (zoals een projectmanager) omdat het de persoon die het goedkeuringsproces beheert toestaat de vooruitgang op het bewijs te controleren en te zien welke gebruikers hun besluit hebben genomen.<br></p><p>Je wordt pas op de hoogte gesteld van je eigen beslissing als je een bevestigingsoptie voor e-mail selecteert wanneer je je beslissing verzendt.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">Definitief besluit</td> 
      <td>Een e-mail wordt verzonden wanneer de definitieve beslissing op het bewijs wordt genomen (wanneer de laatste fiatteur op het bewijs zijn beslissing heeft genomen).<br><p>Deze waarschuwing wordt vaak gebruikt door de ontwerper omdat de ontwerper niet aan de daadwerkelijke overzichtsbespreking hoeft deel te nemen. Wanneer het definitieve besluit wordt genomen, wordt de ontwerper op de hoogte gebracht en kan dan actie ondernemen op om het even welke noodzakelijke veranderingen.<br></p><p>Deze waarschuwing kan ook nuttig zijn voor een afdelingsleider die slechts op de hoogte moet worden gebracht wanneer het overzichtsproces wordt gebeëindigd.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">Uuroverzicht</td> 
      <td>Elk uur wordt een e-mail naar de controleur verzonden met een overzicht van alle opmerkingen, antwoorden en beslissingen die in het afgelopen uur zijn genomen.<br><p>Het e-mailbericht wordt alleen verzonden wanneer er in het afgelopen uur andere activiteiten plaatsvinden dan die van uzelf. Als andere gebruikers geen activiteiten uitvoeren, wordt geen e-mail verzonden.<br></p><p>Deze waarschuwing is een goede manier om een overzicht van het project te zien.<br></p><p>Een voorbeeld van een gebruiksgeval voor deze samenvatting is een senior controleur die een overzicht van het project nodig heeft, maar niet onmiddellijk op de hoogte hoeft te worden gesteld van alle activiteiten op de proefdruk.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">Dagelijkse samenvatting</td> 
      <td>(Standaardinstelling): Elke dag wordt een e-mail verzonden met alle opmerkingen, antwoorden en beslissingen in de lijst. Er wordt alleen een e-mail verzonden op dagen dat er andere activiteiten zijn dan die van uzelf.<br><p>Deze waarschuwing is een goede manier om een samenvatting van het project te zien zonder overweldigd met veelvoudige updates door de dag te worden.<br></p><p>Een voorbeeld gebruikt geval voor deze samenvatting is een afdelingsleider die de algemene vooruitgang van het project wil controleren.<br></p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">Geen e-mail</td> 
      <td>Er worden geen e-mailwaarschuwingen verzonden.<br><p>Deze instelling is handig voor een persoon die alleen ter referentie aan een bewijs wordt toegevoegd en die niet op de hoogte hoeft te worden gesteld van wijzigingen.</p><p>Opmerking: <p>Met deze optie schakelt u alleen e-mailwaarschuwingen uit die u kunt ontvangen over proefdrukopmerkingen en -beslissingen. Hiermee schakelt u de e-mailwaarschuwingen die u kunt ontvangen over de stroom van een proefdruk, zoals de e-mail Nieuwe proef of Bewijs laat uit. Raadpleeg de volgende artikelen voor meer informatie over e-mailwaarschuwingen met betrekking tot de stroom van een bewijs: </p>
        <ul>
         <li><a href="../../../workfront-proof/wp-emailsntfctns/proof-notifications-and-reminders/new-proof-email.md" class="MCXref xref">Nieuwe proefe-mail</a></li>
         <li><a href="../../../workfront-proof/wp-emailsntfctns/proof-notifications-and-reminders/new-version-email.md" class="MCXref xref">Het e-mailbericht voor de nieuwe versie</a></li>
         <li><a href="../../../workfront-proof/wp-emailsntfctns/proof-notifications-and-reminders/late-proof-email.md" class="MCXref xref">E-mailadres voor proefdrukken</a></li>
         <li><a href="../../../workfront-proof/wp-emailsntfctns/proof-notifications-and-reminders/proof-made-email.md" class="MCXref xref">De e-mail met bewijs</a></li>
        </ul></p></td> 
     </tr> 
    </tbody> 
   </table>
