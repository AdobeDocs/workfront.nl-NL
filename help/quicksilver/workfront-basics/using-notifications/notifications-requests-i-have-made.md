---
content-type: reference
navigation-topic: notifications
title: "Meldingen: verzoeken die ik heb gedaan"
description: In de volgende berichten wordt u op de hoogte gebracht van verzoeken die u in Adobe Workfront hebt gedaan.
author: Lisa
feature: Get Started with Workfront
exl-id: 42771f71-dbf8-4e73-9a0e-8efea612af4a
source-git-commit: 9f351a16c2a741b922e8ee51efb3ea3d7d2d18e1
workflow-type: tm+mt
source-wordcount: '1299'
ht-degree: 0%

---

# Meldingen: verzoeken die ik heb ingediend

In de volgende berichten wordt melding gemaakt van verzoeken die u hebt gedaan in [!DNL Adobe Workfront] .

Voor informatie over het vormen van welke berichten u ontvangt, zie [ uw eigen e-mailberichten wijzigen ](../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md).

Zie ook [ de berichten van de Gebeurtenis ](../../workfront-basics/using-notifications/event-notifications.md).

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td colspan="3"><strong> verzoeken ik heb gemaakt </strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong> het verzoek van de documentgoedkeuring van A wordt voltooid </strong> </p> <p>De gebruiker die een goedkeuring voor een document heeft aangevraagd, ontvangt een e-mailbericht wanneer het verzoek om documentgoedkeuring is voltooid.</p> <p>Het onderwerp van de direct-mailmelding is: {<em>} &lt;Naam van goedkeurder&gt; heeft &lt;Goedkeuringsbesluit ([!UICONTROL Approved], [!UICONTROL Approved with Changes], [!UICONTROL Rejected])&gt; dit document.</em></p> <p>Opmerking: u kunt dit bericht niet configureren voor een e-mailbericht met dagelijkse samenvatting.</p> </td> 
   <td> Naam van het document <br> Approver Name </td> 
   <td><strong> Onmiddellijk </strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong> het document van A wordt veranderd of op een kwestie geupload waarvoor ik het primaire contact </strong> ben </p> <p>De primaire contactpersoon van de uitgave ontvangt een e-mailbericht wanneer een document wordt geüpload of gewijzigd tijdens de uitgave, tenzij de gebruiker die het document heeft geüpload of gewijzigd ook de primaire contactpersoon is.</p> <p>Er wordt alleen een melding verzonden als het project is ingesteld als een [!UICONTROL Help Request Queue] (zoals beschreven in <a href="../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md" class="MCXref xref">[!UICONTROL Create a Request Queue]</a> ).</p> <p>Het onderwerp van het onmiddellijke bericht e-mail is: <em> Document dat aan &lt;Naam van de Uitgave&gt; </em> wordt toegevoegd</p> <p>Het onderwerp van het dagelijkse samenvattingsbericht is: <em> Samenvatting van Uw Verzoeken &lt;Datum van de dagelijkse samenvatting&gt; </em></p> </td> 
   <td> Objectnaam van het document dat is geüpload <br>Naam van het bovenliggende object <br>Referentienummer van het document<br>Naam van de gebruiker die het document heeft geüpload<br>Naam van het document<br>Toegevoegd op datum<br>Documentdetails (formaat, grootte, versienummer)<br>Documentminiatuur<br><strong>[!UICONTROL Preview]</strong> en <strong>[!UICONTROL Download]</strong> knoppen<br>*Projectnaam <br>*Projectreferentienummer<br>*Totaal aantal geüploade documenten<br>*Naam van het document<br>*Naam van het bovenliggende object<br>*Naam van de gebruiker Het document <br>*Datum van het dagelijks overzicht toegevoegd </td> 
   <td><strong> Dagelijks </strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong> het verzoek van het document uploadt wordt voldaan aan </strong> </p> <p>De aanvrager van het document ontvangt een e-mailbericht wanneer aan een aanvraag voor het uploaden van een document is voldaan.</p> <p>Het onderwerp van de e-mail met de onmiddellijke melding is: <em>[!UICONTROL Your document request from] &lt;Gebruikersnaam&gt; is uitgevoerd </em></p> <p>Opmerking: u kunt dit bericht niet configureren voor een e-mailbericht met dagelijkse samenvatting.</p> </td> 
   <td> <p>Naam van de gebruiker die het document <br> Naam van Objecten uploadde waar het document <br> Naam van het Document werd geupload<br><br></p> </td> 
   <td><strong> Onmiddellijk </strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong> Een persoonlijke taak ik aan iemand anders heb toegewezen wordt voltooid </strong> </p> <p>Een bericht wordt verzonden naar de gebruiker die een ad-hoctaak aan iemand anders toewees wanneer die taak wordt voltooid. </p> <p>Voor meer informatie over ad hoc taken, zie <a href="../../workfront-basics/using-home/using-the-home-area/create-work-items-in-home.md" class="MCXref xref"> het werkpunten en projecten van het [!UICONTROL Home] gebied </a> creëren.</p> <p>Het onderwerp van het onmiddellijke bericht e-mail is: <em> Voltooiing van de Taak: &lt;Naam van de Taak&gt; </em></p> <p> <p>Opmerking: u kunt dit bericht niet configureren voor een e-mailbericht met dagelijkse samenvatting.</p> </p> </td> 
   <td> Taaknaam<br>Standaardprojectnaam (persoonlijk project van de gebruiker die de persoonlijke taak heeft ontvangen)<br>Taakreferentienummer<br>Naam van taakeigenaar<br>Nieuwe taakstatus<br>Datum en tijd waarop de taak is voltooid<br>Knop Vorige taakstatus<br><strong>[!UICONTROL See More Details]</strong><br><br><br></td> 
   <td><strong> Onmiddellijk </strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong> Een kwestie waarvoor ik het primaire contact ben wordt voltooid </strong> </p> <p>De primaire contactpersoon voor een uitgave ontvangt een melding wanneer de uitgave is voltooid.</p> <p>Er wordt alleen een melding verzonden als de projectstatus [!UICONTROL Current] of [!UICONTROL Planning] is.</p> <p>Het onderwerp van de e-mail met onmiddellijke kennisgeving is: <em>[!UICONTROL Issue Completion]: &lt;Naam van Uitgave&gt; </em></p> <p>Het onderwerp van het dagelijkse samenvattingsbericht is:<em> Samenvatting van uw Verzoeken &lt;Datum van de dagelijkse samenvatting&gt; </em></p> <p> </p> </td> 
   <td> Probleemnaam<br>Projectnaam<br>Uitgavenummer<br>Naam van de gebruiker die het probleem heeft opgelost<br>Nieuwe status<br> Datum en tijd waarop het probleem is opgelost<br> Vorige uitgiftestatus<br><strong>[!UICONTROL See More Details]</strong> knop <br>*Projectnaam<br>*Projectreferentienummer<br>*Totaal aantal voltooide problemen<br>*Uitgavenaam<br>*Naam van de gebruiker die het probleem heeft opgelost<br>*Datum van dagelijkse samenvatting </td> 
   <td><strong> Onmiddellijk </strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong> ik voeg een kwestie aan een project toe </strong> </p> <p>Het primaire contact op een kwestie ontvangt een bericht wanneer hij of zij een kwestie in een project toevoegt.</p> <p>Er wordt alleen een melding verzonden als de projectstatus [!UICONTROL Current] of [!UICONTROL Planning] is.</p> <p>Het onderwerp van de directe melding-e-mail is: <em>[!UICONTROL Issue submitted]: &lt;Issue Name&gt; op &lt;Project Name&gt; </em></p> <p>Het onderwerp van het dagelijkse samenvattingsbericht is:<em> Samenvatting van uw Verzoeken &lt;Datum van de dagelijkse samenvatting&gt; </em></p> </td> 
   <td> Projectnaam<br>Naam Portfolio<br>Referentienummer probleem<br>Uw naam <br>Naam probleem<br>Datum ingevoerd <br>Prioriteit probleem<br>Status probleem<br>Toegewezen aan naam<br>Primair contact<br>*Projectnaam<br>*Projectreferentienummer<br>*Totaal aantal toegevoegde problemen<br>*Naam probleem<br>*Datum van overzicht </td> 
   <td> <p><strong> Onmiddellijk </strong> </p> <p><strong> en Dagelijks </strong> </p> </td> 
  </tr> 
  <tr> 
   <td> <p><strong> ik verzend een verzoek (bevestiging) </strong> </p> <p>De primaire contactpersoon over de uitgave ontvangt een e-mailbericht wanneer hij of zij een kwestie indient.</p> <p>Een melding wordt alleen verzonden als de projectstatus [!UICONTROL Current] is en als het project is ingesteld als een [!UICONTROL Help Request Queue] (zoals beschreven in <a href="../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md" class="MCXref xref">[!UICONTROL Create a Request Queue]</a> ).</p> <p>Het onderwerp van de directe melding-e-mail is: <em>[!UICONTROL Request Submitted]: &lt;Request Name&gt; op &lt;Project (Request Queue) Name&gt; </em></p> <p>Het onderwerp van het dagelijkse samenvattingsbericht is:<em> Samenvatting van uw Verzoeken &lt;Datum van de dagelijkse samenvatting&gt; </em></p> </td> 
   <td> <p>Projectnaam (naam wachtrij voor aanvraag)<br>Naam Portfolio<br>Referentienummer probleem<br>Naam probleem<br>Datum ingevoerd <br>Prioriteit probleem<br>Status probleem<br>Toegewezen aan naam<br>Primair contact<br>*Projectreferentienummer<br>*Projectnaam<br>*Totaal aantal ingediende aanvragen<br>*Naam aanvraag<br>*Prioriteit aanvraag<br>*Datum van het dagelijks overzicht</p> </td> 
   <td> <p><strong> Onmiddellijk </strong> </p> <p><strong> en Dagelijks </strong> </p> </td> 
  </tr> 
  <tr> 
   <td> <p><strong> Mijn verzoek is gesloten (bevestiging) </strong> </p> <p>De primaire contactpersoon van de uitgave ontvangt een e-mailbericht wanneer de aanvraag wordt gesloten.</p> <p>Een bericht wordt verzonden slechts als de projectstatus Huidig is en als het project opstelling als a [!UICONTROL Help Request Queue] is (zoals die in <a href="../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md" class="MCXref xref"> wordt beschreven creeer een Rij van het Verzoek </a>).</p> <p>Het onderwerp van de directe bericht e-mail is: <em>[!UICONTROL Your request has been closed]: "&lt;Request Name&gt;"</em></p> <p>Het onderwerp van het dagelijkse samenvattingsbericht is:<em> [!UICONTROL Digest of your Requests] &lt;Date of the daily digest&gt; </em></p> </td> 
   <td> Aanvraagnaam<br>Projectnaam<br>Aanvraagreferentienummer<br>Naam van de gebruiker die de aanvraag heeft gesloten<br>Probleemstatus<br>Datum en tijd waarop de aanvraag is gesloten<br>Vorige aanvraagstatus<br><strong>[!UICONTROL See More Details]</strong> knop<br>*Projectreferentienummer<br>*Projectnaam<br>*Totaal aantal gesloten aanvragen<br>*Aanvraagnaam<br>*Naam van de gebruiker die de aanvraag heeft gesloten<br>*Datum van overzicht </td> 
   <td><strong> Onmiddellijk </strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong> Iemand wordt toegewezen aan mijn verzoek </strong> </p> <p>De primaire contactpersoon voor de uitgave ontvangt een e-mailbericht wanneer een gebruiker aan de uitgave wordt toegewezen, tenzij de primaire contactpersoon en de toegewezen gebruiker dezelfde gebruiker zijn.</p> <p>Er wordt alleen een melding verzonden als de projectstatus Huidig is en als het project is ingesteld als een [!UICONTROL Help Request Queue] (zoals beschreven in <a href="../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md" class="MCXref xref">[!UICONTROL Create a Request Queue]</a> ).</p> <p>Het onderwerp van de directe bericht e-mail is: <em> &lt;Naam van de gebruiker die aan uw verzoek wordt toegewezen&gt; [!UICONTROL has been assigned to your request]: "&lt;Naam van het Verzoek&gt;"</em></p> <p>Het onderwerp van het dagelijkse samenvattingsbericht is:<em> [!UICONTROL Digest of your Requests] &lt;Date of the daily digest&gt; </em></p> </td> 
   <td> <p>De Naam van het dossier <br> Naam van het Project van de 1} Uitgave van het Referentienummer <br> het Type van het Verzoek <br> Toegelaten Datum van het Verzoek <br> <br> Uitgave Prioriteit 6} Primair contact <br> Geplande Status van de Voltooiing <br><strong> zie Meer Details </strong> knoop <br>*De Naam van het Project <br>*Het Aantal van de Verwijzing van het Project <br>*Totaal van 13} Uitgave van 13} Uitgeven aan verzoeken 4}*Naam van verzoek <br>*Toegewezen aan Naam <br>*Datum van dagelijkse samenvatting<br><br><br><br></p> </td> 
   <td><strong> Dagelijks </strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong> de statusveranderingen op een project I creeerde </strong> </p> <p>De gebruiker die het project creeerde ontvangt een e-mailbericht wanneer de projectstatus verandert.</p> <p>Het onderwerp van de directe bericht e-mail is: <em>[!UICONTROL Project Status Change]: &lt;de Naam van het Project&gt; </em></p> <p>Het onderwerp van het dagelijkse samenvattingsbericht is:<em> [!UICONTROL Digest of your Requests] &lt;Date of the daily digest&gt; </em></p> </td> 
   <td> <p>Projectnaam<br>Naam Portfolio<br>Projectreferentienummer<br>Naam van de gebruiker die de status<br>Nieuwe status<br>Datum en tijd waarop de projectstatus werd gewijzigd<br>Vorige projectstatus<br><strong>[!UICONTROL See More Details]</strong> knop<br>*Projectnaam<br>*Projectreferentienummer<br>*Nieuwe projectstatus<br>*Naam van de gebruiker die de projectstatus<br>*Datum van dagelijks overzicht heeft gewijzigd</p> </td> 
   <td> <p><strong> Onmiddellijk </strong> </p> </td> 
  </tr> 
  <tr> 
   <td> <p><strong> de statusveranderingen op mijn verzoek </strong> </p> <p>De primaire contactpersoon van de uitgave ontvangt een e-mailbericht wanneer de status van de uitgave verandert, tenzij de gebruiker die de status heeft gewijzigd ook de primaire contactpersoon is.</p> <p>Er wordt alleen een melding verzonden als de projectstatus Huidig is en het project is ingesteld als een [!UICONTROL Help Request Queue] (zoals beschreven in <a href="../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md" class="MCXref xref">[!UICONTROL Create a Request Queue]</a> ).</p> <p>Het onderwerp van de directe bericht e-mail is: <em> &lt;Request Name&gt; is &lt;New Status&gt; </em></p> <p>Het onderwerp van het dagelijkse samenvattingsbericht is:<em> Samenvatting van uw Verzoeken &lt;Datum van de dagelijkse samenvatting&gt; </em></p> </td> 
   <td> Aanvraagnaam<br>Projectnaam<br>Aanvraagreferentienummer<br>Naam van de gebruiker die de status van de aanvraag heeft gewijzigd<br>Nieuwe status<br>Datum en tijd waarop de status van de aanvraag is gewijzigd<br>Vorige aanvraagstatus<br><strong>[!UICONTROL See More Details]</strong> knop<br>*Projectnaam<br>*Projectreferentienummer<br>*Totaal aantal aanvragen waarvan de status is gewijzigd<br>*Aanvraagnaam<br>*Vorige aanvraagstatus<br>*Nieuw Status aanvragen<br>*Naam van de gebruiker die de status<br>*Datum van het dagelijks overzicht heeft gewijzigd<br></td> 
   <td> <p><strong> Dagelijks </strong> </p> <p> </p> </td> 
  </tr> 
 </tbody> 
</table>
