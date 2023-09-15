---
content-type: reference
navigation-topic: notifications
title: "Meldingen: verzoeken die ik heb gedaan"
description: In de volgende berichten wordt u op de hoogte gebracht van verzoeken die u in Adobe Workfront hebt gedaan.
author: Lisa
feature: Get Started with Workfront
exl-id: 42771f71-dbf8-4e73-9a0e-8efea612af4a
source-git-commit: f6335f4e94d286681adfb50165562b2c41b5acac
workflow-type: tm+mt
source-wordcount: '1297'
ht-degree: 0%

---

# Meldingen: verzoeken die ik heb ingediend

In de volgende berichten wordt u op de hoogte gesteld van verzoeken die u hebt ingediend in [!DNL Adobe Workfront].

Voor informatie over het vormen van welke berichten u ontvangt, zie [Uw eigen e-mailmeldingen wijzigen](../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md).

Zie ook [Gebeurtenismeldingen](../../workfront-basics/using-notifications/event-notifications.md).

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td colspan="3"><strong>Verzoeken die ik heb gedaan</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Een aanvraag voor documentgoedkeuring is voltooid</strong> </p> <p>De gebruiker die een goedkeuring voor een document heeft aangevraagd, ontvangt een e-mailbericht wanneer het verzoek om documentgoedkeuring is voltooid.</p> <p>Het onderwerp van de e-mail met onmiddellijke kennisgeving is:<em> &lt;approver name=""&gt; heeft &lt;approval decision="" span="" id="1" translate="no" /&gt;, [!UICONTROL Approved with Changes], [!UICONTROL Rejected])&gt; dit document.</em>[!UICONTROL Approved]</p> <p>Opmerking: u kunt dit bericht niet configureren voor een e-mailbericht met dagelijkse samenvatting.</p> </td> 
   <td> Documentnaam<br>Naam fiatteur </td> 
   <td><strong>Meteen</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Een document wordt gewijzigd of geüpload naar een probleem waarvoor ik de primaire contactpersoon ben</strong> </p> <p>De primaire contactpersoon van de uitgave ontvangt een e-mailbericht wanneer een document wordt geüpload of gewijzigd tijdens de uitgave, tenzij de gebruiker die het document heeft geüpload of gewijzigd ook de primaire contactpersoon is.</p> <p>Een kennisgeving wordt alleen verzonden als het project als een [!UICONTROL Help Request Queue] (zoals beschreven in <a href="../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md" class="MCXref xref">[!UICONTROL Create a Request Queue]</a>).</p> <p>Het onderwerp van de e-mail met onmiddellijke kennisgeving is: <em>Document toegevoegd aan &lt;issue name=""&gt;</em></p> <p>Het onderwerp van de dagelijkse overzichtsmelding is: <em>Samenvatting van uw verzoeken &lt;date of="" the="" daily="" digest=""&gt;</em></p> </td> 
   <td> Objectnaam waar het document is geüpload<br>Naam bovenliggend object<br>Referentienummer document<br>Naam van de gebruiker die het document heeft geüpload<br>Documentnaam<br>Toegevoegd op datum<br>Documentdetails (formaat, grootte, versienummer)<br>Documentminiatuur<br><strong>[!UICONTROL Preview]</strong> en <strong>[!UICONTROL Download]</strong> knoppen<br>*Projectnaam<br>*Referentienummer van project<br>*Totaal aantal geüploade documenten<br>*Naam van document<br>*Naam van bovenliggend object<br>*Naam van de gebruiker die het document heeft toegevoegd<br>*Datum van de dagelijkse samenvatting </td> 
   <td><strong>Dagelijks</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Er is voldaan aan een aanvraag voor het uploaden van een document</strong> </p> <p>De aanvrager van het document ontvangt een e-mailbericht wanneer aan een aanvraag voor het uploaden van een document is voldaan.</p> <p>Het onderwerp van de e-mail met onmiddellijke kennisgeving is: <em>[!UICONTROL Your document request from] &lt;user name=""&gt; is voldaan</em></p> <p>Opmerking: u kunt dit bericht niet configureren voor een e-mailbericht met dagelijkse samenvatting.</p> </td> 
   <td> <p>Naam van de gebruiker die het document heeft geüpload<br>Objectnaam waar het document is geüpload<br>Documentnaam<br><br></p> </td> 
   <td><strong>Meteen</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Een persoonlijke taak die ik aan iemand anders heb toegewezen, is voltooid</strong> </p> <p>Een bericht wordt verzonden naar de gebruiker die een ad-hoctaak aan iemand anders toewees wanneer die taak wordt voltooid. </p> <p>Voor meer informatie over ad-hoctaken raadpleegt u <a href="../../workfront-basics/using-home/using-the-home-area/create-work-items-in-home.md" class="MCXref xref">Werkitems maken op basis van het tabblad [!UICONTROL Home] gebied</a>.</p> <p>Het onderwerp van de e-mail met onmiddellijke kennisgeving is: <em>Taak voltooid: &lt;task name=""&gt;</em></p> <p> <p>Opmerking: u kunt dit bericht niet configureren voor een e-mailbericht met dagelijkse samenvatting.</p> </p> </td> 
   <td> Taaknaam<br>Standaard Projectnaam (Persoonlijk Project van de gebruiker die de persoonlijke taak ontving)<br>Referentienummer taak<br>Naam taakeigenaar<br>Nieuwe taakstatus<br>Datum en tijd waarop de taak is voltooid<br>Status vorige taak<br><strong>[!UICONTROL See More Details]</strong> knop<br><br><br></td> 
   <td><strong>Meteen</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Een probleem waarvoor ik de primaire contactpersoon ben, is opgelost</strong> </p> <p>De primaire contactpersoon voor een uitgave ontvangt een melding wanneer de uitgave is voltooid.</p> <p>Een kennisgeving wordt alleen verzonden als de projectstatus [!UICONTROL Current] of [!UICONTROL Planning].</p> <p>Het onderwerp van de e-mail met onmiddellijke kennisgeving is: <em>[!UICONTROL Issue Completion]: &lt;issue name=""&gt;</em></p> <p>Het onderwerp van de dagelijkse overzichtsmelding is:<em> Samenvatting van uw verzoeken &lt;date of="" the="" daily="" digest=""&gt;</em></p> <p> </p> </td> 
   <td> Naam van uitgave<br>Projectnaam<br>Referentienummer van uitgave<br>Naam van de gebruiker die de uitgave heeft voltooid<br>Nieuwe status<br>Datum en tijdstip waarop de afgifte is voltooid<br>Status van vorige uitgave<br><strong>[!UICONTROL See More Details]</strong> knop <br>*Projectnaam<br>*Referentienummer van project<br>*Totaal aantal voltooide uitgaven<br>*Naam van uitgave<br>*Naam van de gebruiker die de uitgave heeft voltooid<br>*Datum van de dagelijkse samenvatting </td> 
   <td><strong>Meteen</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Ik voeg een kwestie aan een project toe</strong> </p> <p>Het primaire contact op een kwestie ontvangt een bericht wanneer hij of zij een kwestie in een project toevoegt.</p> <p>Een kennisgeving wordt alleen verzonden als de projectstatus [!UICONTROL Current] of [!UICONTROL Planning].</p> <p>Het onderwerp van de e-mail met onmiddellijke kennisgeving is: <em>[!UICONTROL Issue submitted]: &lt;issue name=""&gt; op &lt;project name=""&gt;</em></p> <p>Het onderwerp van de dagelijkse overzichtsmelding is:<em> Samenvatting van uw verzoeken &lt;date of="" the="" daily="" digest=""&gt;</em></p> </td> 
   <td> Projectnaam<br>Naam Portfolio<br>Referentienummer van uitgave<br>Uw naam<br>Naam van uitgave<br>Datum van invoer<br>Probleemprioriteit<br>Status van afgifte<br>Toegewezen aan naam<br>Primaire contactpersoon<br>*Projectnaam<br>*Referentienummer van project<br>*Totaal aantal toegevoegde uitgaven<br>*Naam van uitgave<br>*Datum van de dagelijkse samenvatting </td> 
   <td> <p><strong>Meteen</strong> </p> <p><strong>en dagelijks</strong> </p> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Ik verzend een verzoek (bevestiging)</strong> </p> <p>De primaire contactpersoon over de uitgave ontvangt een e-mailbericht wanneer hij of zij een kwestie indient.</p> <p>Een kennisgeving wordt alleen verzonden als de projectstatus [!UICONTROL Current] en of het project als een [!UICONTROL Help Request Queue] (zoals beschreven in <a href="../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md" class="MCXref xref">[!UICONTROL Create a Request Queue]</a>).</p> <p>Het onderwerp van de e-mail met onmiddellijke kennisgeving is: <em>[!UICONTROL Request Submitted]: &lt;request name=""&gt; op &lt;project request="" queue="" name=""&gt;</em></p> <p>Het onderwerp van de dagelijkse overzichtsmelding is:<em> Samenvatting van uw verzoeken &lt;date of="" the="" daily="" digest=""&gt;</em></p> </td> 
   <td> <p>Projectnaam (naam wachtrij aanvragen)<br>Naam Portfolio<br>Referentienummer van uitgave<br>Naam van uitgave<br>Datum van invoer<br>Probleemprioriteit<br>Status van afgifte<br>Toegewezen aan naam<br>Primaire contactpersoon<br>*Referentienummer van project<br>*Projectnaam<br>*Totaal aantal ingediende verzoeken<br>*Naam aanvraag<br>*Aanvraagprioriteit<br>*Datum van de dagelijkse samenvatting</p> </td> 
   <td> <p><strong>Meteen</strong> </p> <p><strong>en dagelijks</strong> </p> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Mijn aanvraag is gesloten (bevestiging)</strong> </p> <p>De primaire contactpersoon van de uitgave ontvangt een e-mailbericht wanneer de aanvraag wordt gesloten.</p> <p>Een kennisgeving wordt alleen verzonden als de projectstatus Actief is en als het project is opgezet als een [!UICONTROL Help Request Queue] (zoals beschreven in <a href="../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md" class="MCXref xref">Een aanvraagwachtrij maken</a>).</p> <p>Het onderwerp van de e-mail met onmiddellijke kennisgeving is: <em>[!UICONTROL Your request has been closed]:"&lt;request name=""&gt;"</em></p> <p>Het onderwerp van de dagelijkse overzichtsmelding is:<em> [!UICONTROL Digest of your Requests] &lt;date of="" the="" daily="" digest=""&gt;</em></p> </td> 
   <td> Naam aanvraag<br>Projectnaam<br>Referentienummer aanvragen<br>Naam van de gebruiker die de aanvraag heeft gesloten<br>Status van afgifte<br>Datum en tijdstip waarop het verzoek is gesloten<br>Vorige aanvraagstatus<br><strong>[!UICONTROL See More Details]</strong> knop<br>*Referentienummer van project<br>*Projectnaam<br>*Totaal aantal afgesloten aanvragen<br>*Naam aanvraag<br>*Naam van de gebruiker die de aanvraag heeft gesloten<br>*Datum van de dagelijkse samenvatting </td> 
   <td><strong>Meteen</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Er is iemand toegewezen aan mijn verzoek</strong> </p> <p>De primaire contactpersoon voor de uitgave ontvangt een e-mailbericht wanneer een gebruiker aan de uitgave wordt toegewezen, tenzij de primaire contactpersoon en de toegewezen gebruiker dezelfde gebruiker zijn.</p> <p>Een kennisgeving wordt alleen verzonden als de projectstatus Actief is en als het project is opgezet als een [!UICONTROL Help Request Queue] (zoals beschreven in <a href="../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md" class="MCXref xref">[!UICONTROL Create a Request Queue]</a>).</p> <p>Het onderwerp van de e-mail met onmiddellijke kennisgeving is: <em>&lt;name of="" the="" user="" who="" is="" assigned="" to="" your="" request=""&gt; [!UICONTROL has been assigned to your request]: "&lt;request name=""&gt;"</em></p> <p>Het onderwerp van de dagelijkse overzichtsmelding is:<em> [!UICONTROL Digest of your Requests] &lt;date of="" the="" daily="" digest=""&gt;</em></p> </td> 
   <td> <p>Naam van uitgave<br>Projectnaam<br>Referentienummer van uitgave<br>Naam aanvraag<br>Type aanvraag<br>Datum van invoer<br>Probleemprioriteit<br>Primaire contactpersoon<br>Geplande afsluitdatum<br>Status van afgifte<br><strong>Meer informatie</strong> knop <br>*Projectnaam<br>*Referentienummer van project<br>*Totaal aantal toegewezen verzoeken<br>*Naam aanvraag<br>*Toegewezen aan naam<br>*Datum van de dagelijkse samenvatting</p> </td> 
   <td><strong>Dagelijks</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>De statusveranderingen in een project dat ik creeerde</strong> </p> <p>De gebruiker die het project creeerde ontvangt een e-mailbericht wanneer de projectstatus verandert.</p> <p>Het onderwerp van de e-mail met onmiddellijke kennisgeving is: <em>[!UICONTROL Project Status Change]: &lt;project name=""&gt;</em></p> <p>Het onderwerp van de dagelijkse overzichtsmelding is:<em> [!UICONTROL Digest of your Requests] &lt;date of="" the="" daily="" digest=""&gt;</em></p> </td> 
   <td> <p>Projectnaam<br>Naam Portfolio<br>Projectreferentienummer<br>Naam van de gebruiker die de status heeft gewijzigd<br>Nieuwe status<br>Datum en tijd waarop de projectstatus is gewijzigd<br>Vorige projectstatus<br><strong>[!UICONTROL See More Details]</strong> knop<br>*Projectnaam<br>*Referentienummer van project<br>*Nieuwe status van project<br>*Naam van de gebruiker die de projectstatus veranderde<br>*Datum van de dagelijkse samenvatting</p> </td> 
   <td> <p><strong>Meteen</strong> </p> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>De status verandert op mijn verzoek</strong> </p> <p>De primaire contactpersoon van de uitgave ontvangt een e-mailbericht wanneer de status van de uitgave verandert, tenzij de gebruiker die de status heeft gewijzigd ook de primaire contactpersoon is.</p> <p>Een kennisgeving wordt alleen verzonden als de projectstatus Actief is en het project is opgezet als een [!UICONTROL Help Request Queue] (zoals beschreven in <a href="../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md" class="MCXref xref">[!UICONTROL Create a Request Queue]</a>).</p> <p>Het onderwerp van de e-mail met onmiddellijke kennisgeving is: <em>&lt;request name=""&gt; is &lt;new status=""&gt;</em></p> <p>Het onderwerp van de dagelijkse overzichtsmelding is:<em> Samenvatting van uw verzoeken &lt;date of="" the="" daily="" digest=""&gt;</em></p> </td> 
   <td> Naam aanvraag<br>Projectnaam<br>Referentienummer aanvragen<br>Naam van de gebruiker die de status van de aanvraag heeft gewijzigd<br>Nieuwe status<br>Datum en tijdstip waarop de status van het verzoek is gewijzigd<br>Vorige aanvraagstatus<br><strong>[!UICONTROL See More Details]</strong> knop<br>*Projectnaam<br>*Referentienummer van project<br>*Totaal aantal aanvragen waarvan de status is gewijzigd<br>*Naam aanvraag<br>*Vorige aanvraagstatus<br>*Nieuwe aanvraagstatus<br>*Naam van de gebruiker die de status heeft gewijzigd<br>*Datum van de dagelijkse samenvatting<br></td> 
   <td> <p><strong>Dagelijks</strong> </p> <p> </p> </td> 
  </tr> 
 </tbody> 
</table>
