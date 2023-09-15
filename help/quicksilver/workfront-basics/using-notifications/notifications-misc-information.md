---
content-type: reference
navigation-topic: notifications
title: "Meldingen: Diverse informatie"
description: In de volgende berichten wordt u gewaarschuwd voor activiteiten die plaatsvinden in een project dat u sponsort.
author: Lisa
feature: Get Started with Workfront
exl-id: fd93a48b-ef09-4489-b93d-5328240ffed6
source-git-commit: f6335f4e94d286681adfb50165562b2c41b5acac
workflow-type: tm+mt
source-wordcount: '879'
ht-degree: 0%

---

# Meldingen: Diverse informatie

In de volgende berichten wordt u gewaarschuwd voor activiteiten die plaatsvinden in een project dat u sponsort.

Voor informatie over het vormen van welke berichten u ontvangt, zie [Uw eigen e-mailmeldingen wijzigen](../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md).

Zie ook [Gebeurtenismeldingen](../../workfront-basics/using-notifications/event-notifications.md).

>[!NOTE]
>
>U kunt dagelijkse meldingen niet in- of uitschakelen en u ontvangt geen dagelijkse samenvattingse-mails voor de gebeurtenissen in deze categorie. U kunt afzonderlijke instantmeldingen in- of uitschakelen voor de [!UICONTROL Miscellaneous] categorie.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Melding</th> 
   <th> <p>Inclusief velden </p> <p> *Alleen velden voor dagelijkse samenvatting</p> </th> 
   <th>Standaardstatus</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p><strong>Er wordt een bericht verzonden naar de [!UICONTROL Announcement Center]</strong> </p> <p>U ontvangt een e-mailbericht wanneer een nieuw bericht naar de [!UICONTROL Announcement Center]. </p> <p>Het onderwerp van de e-mail met onmiddellijke kennisgeving is: <em>[!UICONTROL [!DNL Adobe Workfront] Mededeling]: &lt;subject of="" the="" announcement=""&gt;</em></p> </td> 
   <td> Betreft: Aankondiging<br>Tekst van het bericht in de aankondiging<br>Bijgevoegd document(en)<br>Naam van de gebruiker die de aankondiging heeft verzonden<br>Datum en tijdstip waarop de aankondiging is verzonden </td> 
   <td><strong>Meteen</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Een wijziging in de taaktoewijzing is van invloed op een van mijn mensen</strong> </p> <p>Wanneer een van de Directe Rapporten van een gebruiker die als manager wordt aangewezen aan een nieuwe taak wordt toegewezen, ontvangt de manager een e-mail over de taak. </p> <p>Een kennisgeving wordt alleen verzonden als de projectstatus [!UICONTROL Current].</p> <p>Het onderwerp van de e-mail met onmiddellijke kennisgeving is: <em>[!UICONTROL Task Resource Assignment]: &lt;task name=""&gt;</em></p> </td> 
   <td>Projectnaam<br>Taaknaam<br>Datum en tijd waarop de taak is gemaakt<br>Naam van de gebruiker die de taak heeft gemaakt<br>Toewijzingsnamen<br>Vervaldatum (geplande afsluitdatum)<br>Taakstatus<br></td> 
   <td><strong>Meteen</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Na ontvangst van een aanvraag voor het uploaden van een document wordt de aanvraag geannuleerd</strong> </p> <p>De documentaanvrager ontvangt een e-mailbericht wanneer een documentverzoek wordt geannuleerd.</p> <p>Het onderwerp van de e-mail met onmiddellijke kennisgeving is: <em>&lt;name of="" the="" user="" who="" canceled="" the="" request=""&gt; heeft de documentaanvraag geannuleerd. </em></p> <p>De volgende tekst is opgenomen in de tekst van de e-mailmelding:</p> <p><em>[!UICONTROL Hi] &lt;your name=""&gt;, <br><br>&lt;name of="" the="" user="" who="" canceled="" the="" request=""&gt;[!UICONTROL no longer needs you to upload anything regarding the request you got earlier. We just wanted to let you know.]</em> </p> </td> 
   <td>Naam van de gebruiker die de aanvraag heeft geannuleerd<br>De tekst van het oorspronkelijke uploadverzoek voor documenten<br>A "[!UICONTROL CANCELED]" banner over de oorspronkelijke documentaanvraag<br>Datum en tijd van de oorspronkelijke documentaanvraag<br></td> 
   <td><strong>Meteen</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Er is een fout gevonden die mijn aandacht vereist</strong> </p> <p>De gebruiker die via e-mail op een opmerking antwoordt, ontvangt een e-mailbericht wanneer het antwoord niet is verzonden.</p> <p>Het onderwerp van de e-mail met onmiddellijke kennisgeving is: <em>[!UICONTROL Failed to Process on] &lt;subject of="" original="" message=""&gt;</em></p> <p>Zie voor informatie over het gebruik van e-mail om opmerkingen te beantwoorden.<strong></strong></p> </td> 
   <td> </td> 
   <td><strong>Meteen</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Een wijziging in de toewijzing van een uitgave is van invloed op een van mijn mensen</strong> </p> <p>De manager van een gebruiker aan een kwestie wordt toegewezen ontvangt een e-mailbericht wanneer die gebruiker van of aan een kwestie wordt verwijderd. </p> <p>Een bericht wordt verzonden slechts als de projectstatus Huidig of Planning is.</p> <p>Het onderwerp van de e-mail met onmiddellijke kennisgeving is: <em>Toewijzing probleem: &lt;issue name=""&gt;</em></p> </td> 
   <td> <p>Naam van uitgave<br>Projectnaam<br>Referentienummer van uitgave<br>Naam van de gebruiker die de toewijzing heeft gemaakt<br>Type probleem<br>Naam van de gebruiker die aan de uitgave is toegewezen<br>Datum van afgifte ingevoerd<br>Probleemprioriteit<br>Primaire contactpersoon<br>Probleem [!UICONTROL Planned Completion Date]<br>Status van afgifte<br><strong>[!UICONTROL See More Details]</strong> knop</p> </td> 
   <td><strong>Meteen</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Een van mijn mensen wordt toegevoegd aan een project</strong> </p> <p>Een manager ontvangt een e-mailbericht wanneer een van zijn of haar gebruikers aan een project wordt toegevoegd. Deze kennisgeving wordt verzonden ongeacht de status van het project. </p> <p>Gebruikers met een [!UICONTROL Review] de licentie ontvangt geen kennisgeving.</p> <p>Het onderwerp van de e-mail is: <em>Projecttoewijzing: &lt;user name=""&gt;[&lt;project guid=""&gt;_ &lt;user guid=""&gt;]</em></p> </td> 
   <td> <p>Projectnaam<br>Naam Portfolio<br>Projectreferentienummer<br>Naam van de gebruiker die de persoon aan het project toevoegde<br>Naam van de gebruiker die aan het project werd toegevoegd<br>Project [!UICONTROL Planned Start Date]<br>Project [!UICONTROL Planned Completion Date]<br>Projectpercentage voltooid<br>Namen van anderen in het project<br>Projectstatus<br>Projecteigenaar<br><strong>[!UICONTROL See More Details]</strong> knop<br><br><br></p> </td> 
   <td><strong>Meteen</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Iemand voegt een project toe aan een portfolio of programma waarvan ik eigenaar ben</strong> </p> <p>De portefeuille en/of de programmaeigenaar ontvangen een bericht wanneer een nieuw project aan een portefeuille of een programma wordt toegevoegd.</p> <p>Het onderwerp van de e-mail met onmiddellijke kennisgeving is: <em>[!UICONTROL Project added to] &lt;portfolio name=""&gt;[Project GUID]</em></p> </td> 
   <td> Naam Portfolio<br>Projectreferentienummer<br>Naam van de gebruiker die het project aan de portefeuille/het programma heeft toegevoegd<br><br></td> 
   <td><strong>Meteen</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Iemand deelt een object met mij</strong> </p> <p>U ontvangt een e-mailbericht wanneer iemand u toevoegt aan de [!UICONTROL Sharing] lijst met machtigingen voor een object.</p> <p>Het onderwerp van de e-mail met onmiddellijke kennisgeving is: <em>[!UICONTROL Access Granted]: &lt;object name=""&gt;</em></p> <p>Er wordt alleen een melding verzonden als het project zich in [!UICONTROL Current] status.</p> </td> 
   <td> Objectnaam<br>Naam bovenliggend object<br>Objectreferentienummer<br>Oorspronkelijke toegang tot het object<br>Nieuwe toegang verleend aan het object<br>Datum en tijdstip waarop de toegang is verleend <br>Naam van de gebruiker die de toegang heeft verleend </td> 
   <td><strong>Meteen</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Iemand deelt een object met mijn team</strong> </p> <p>U ontvangt een e-mailbericht wanneer iemand uw team toevoegt aan de lijst met machtigingen voor delen voor een object.</p> <p>Het onderwerp van de e-mail met onmiddellijke kennisgeving is: <em>[!UICONTROL Access Granted]: &lt;object name=""&gt; [GUID toegangsregel]</em></p> </td> 
   <td> Objectnaam<br>Naam bovenliggend object<br>Objectreferentienummer<br>Oude toegang<br>Nieuwe toegang<br>Datum en tijdstip waarop de toegang is verleend<br>Naam van uw team<br>Naam van de gebruiker die de toegang heeft verleend </td> 
   <td><strong>Meteen</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Een update wordt gemaakt aan een taak, een kwestie, of een project waar ik op geabonneerd ben</strong> </p> <p>Je ontvangt een e-mailbericht wanneer iemand commentaar levert op een object waarop je bent geabonneerd.</p> <p>Het onderwerp van de e-mail met abonnementen is: <em>[!UICONTROL An update was made to the] &lt;object type=""&gt; je bent geabonneerd op: &lt;object name=""&gt;</em></p> </td> 
   <td> Objectnaam<br> Objectreferentienummer<br> Naam van de gebruiker die een opmerking heeft gemaakt over het geabonneerde item<br> Opmerking: datum<br> Opmerking toegevoegd aan het geabonneerde item  </td> 
   <td><strong>Meteen</strong> </td> 
  </tr> 
 </tbody> 
</table>
