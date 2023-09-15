---
content-type: reference
navigation-topic: notifications
title: "Meldingen: Erkenningsgegevens"
description: In de volgende berichten wordt u gewaarschuwd voor goedkeuringsactiviteiten voor een onderdeel dat u gebruikt. Zie Uw eigen e-mailmeldingen wijzigen voor informatie over het configureren van de berichten die u ontvangt.
author: Lisa
feature: Get Started with Workfront
exl-id: e152913e-de7e-405f-af63-827a9b91e2ae
source-git-commit: f6335f4e94d286681adfb50165562b2c41b5acac
workflow-type: tm+mt
source-wordcount: '571'
ht-degree: 0%

---

# Meldingen: goedkeuringsgegevens

In de volgende berichten wordt u gewaarschuwd voor goedkeuringsactiviteiten voor een onderdeel dat u gebruikt. Voor informatie over het vormen van welke berichten u ontvangt, zie [Uw eigen e-mailmeldingen wijzigen](../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md).

Zie ook [Gebeurtenismeldingen](../../workfront-basics/using-notifications/event-notifications.md).

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
   <td> <p><strong>Een verzoek tot goedkeuring van een gedelegeerde afgifte is voltooid</strong> </p> <p>Een goedkeuring van de uitgave die u aan een andere gebruiker hebt gedelegeerd werd goedgekeurd of verworpen door die gebruiker.</p> <p>Het onderwerp van de e-mail met onmiddellijke kennisgeving is: <em>[!UICONTROL Issue Approval/ Rejection Made on Your Behalf by] &lt;user name=""&gt;</em></p> <p>Het onderwerp van de dagelijkse overzichtsmelding is:<em> [!UICONTROL Digest of Approval Information] &lt;date of="" daily="" digest=""&gt;</em></p> </td> 
   <td> <p>Naam van uitgave<br>Projectnaam<br>Referentienummer van uitgave<br>Naam van de gebruiker die het probleem namens u heeft goedgekeurd/afgewezen<br>Goedkeuringsbesluit<br>Status van afgifte<br>Naam van de gebruiker die de goedkeuring heeft aangevraagd<br><strong>[!UICONTROL See More Details]</strong> knop<br>*Referentienummer van project<br>*Projectnaam<br>*Totaal aantal gedelegeerde emissiecontroles<br>*Naam van uitgave<br>*Naam fiatteur<br>*Datum van de dagelijkse samenvatting<br><br></p> </td> 
   <td><strong>Dagelijks</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Een gedelegeerd verzoek tot goedkeuring van een project is voltooid</strong> </p> <p>Een projectgoedkeuring die u aan een andere gebruiker delegeerde werd goedgekeurd of verworpen door die gebruiker.</p> <p>Het onderwerp van de e-mail met onmiddellijke kennisgeving is: <em>[!UICONTROL Project Approval/ Rejection Made on Your Behalf by] &lt;user name=""&gt;</em></p> <p><em>Het onderwerp van de dagelijkse overzichtsmelding is: [!UICONTROL Digest of Approval Information] &lt;date of="" daily="" digest=""&gt;</em> </p> </td> 
   <td> Projectnaam<br>[!UICONTROL Portfolio Name]<br>[!UICONTROL Project Reference Number]<br>Naam van de gebruiker die het project namens u heeft goedgekeurd/afgewezen<br>[!UICONTROL Approval Decision]<br>[!UICONTROL Project Status]<br>Naam van de gebruiker die de goedkeuring heeft aangevraagd<br><strong>[!UICONTROL See More Details]</strong> knop<br>*Referentienummer van project<br>*Projectnaam<br>*Naam fiatteur<br>[!UICONTROL *Date of the daily digest]<br></td> 
   <td><strong>Dagelijks</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Een verzoek voor gedelegeerde taakgoedkeuring is voltooid</strong> </p> <p>Een taakgoedkeuring die u aan een andere gebruiker delegeerde werd goedgekeurd of verworpen door die gebruiker.</p> <p>Het onderwerp van de e-mail met onmiddellijke kennisgeving is: <em>[!UICONTROL Task Approval/ Rejection Made on Your Behalf by] &lt;user name=""&gt;</em></p> <p>Het onderwerp van de dagelijkse overzichtsmelding is:<em> [!UICONTROL Digest of Approval Information] &lt;date of="" daily="" digest=""&gt;</em></p> </td> 
   <td> Taaknaam<br>Projectnaam<br>Referentienummer taak<br>Naam van de gebruiker die de taak namens u heeft goedgekeurd/afgewezen<br>Goedkeuringsbesluit<br>Taakstatus<br>Naam van de gebruiker die de goedkeuring heeft aangevraagd<br><strong>Meer informatie</strong> knop<br>*Referentienummer van project<br>*Projectnaam<br>*Totaal aantal gedelegeerde taakgoedkeuringen<br>*Taaknaam<br>*Naam fiatteur<br>*Datum van de dagelijkse samenvatting<br></td> 
   <td><strong>Dagelijks</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Een aanvraag voor documentgoedkeuring is geannuleerd</strong> </p> <p>De documentfiatteur van het document ontvangt een e-mailbericht wanneer het verzoek om documentgoedkeuring wordt geannuleerd.</p> <p>Het onderwerp van de e-mail met onmiddellijke kennisgeving is: <em>&lt;user name=""&gt; [!UICONTROL canceled the document approval request]</em></p> <p> <p>Opmerking: u kunt dit bericht niet configureren voor een e-mailbericht met dagelijkse samenvatting.</p> </p> </td> 
   <td> Naam van de gebruiker die de goedkeuringsaanvraag heeft geannuleerd<br>[!UICONTROL Document Name] </td> 
   <td><strong>Meteen</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Ik ben gedelegeerd als fiatteur</strong> </p> <p>Als iemand u toestemming heeft gegeven, ontvangt u een e-mailbericht. </p> <p>Het onderwerp van de e-mail met onmiddellijke kennisgeving is: <em>[!UICONTROL Delegated] &lt;object type=""&gt; [!UICONTROL Approval - Please Review] &lt;object name=""&gt;</em></p> <p> <p>Opmerking: u kunt dit bericht niet configureren voor een e-mailbericht met dagelijkse samenvatting.</p> </p> </td> 
   <td> <p>[!UICONTROL Object Name]<br>[!UICONTROL Parent Object Name]<br>[!UICONTROL Object Reference Number]<br>Naam van de gebruiker die het object ter goedkeuring heeft ingediend<br>Naam van de gebruiker namens wie u het voorwerp goedkeurt<br>Objectstatus<br>Datum en tijdstip waarop de goedkeuring is aangevraagd<br>Objectprioriteit<br>Naam goedkeuringsstap<br>[!UICONTROL Planned Completion Date] van het object<br><strong>[!UICONTROL Make Approval Decision]</strong> knop</p> </td> 
   <td><strong>Meteen</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Mijn timesheet is goedgekeurd</strong> </p> <p>Wanneer uw tijdspagina is goedgekeurd, ontvangt u een e-mailbericht.</p> <p>Het onderwerp van de e-mail met onmiddellijke kennisgeving is: <em>[!UICONTROL Timesheet Approved]: &lt;timesheet start="" date=""&gt; - &lt;timesheet end="" date=""&gt;</em></p> <p> <p>Opmerking: u kunt dit bericht niet configureren voor een e-mailbericht met dagelijkse samenvatting.</p> </p> </td> 
   <td> Naam van de gebruiker die uw tijdspagina heeft goedgekeurd<br>Datum en tijdstip waarop het tijdschrift is goedgekeurd<br>Status van het tijdschrift ([!UICONTROL Approved])<br>Begindatum en Einddatum van het tijdblad<br>Totaal aantal uren dat is aangemeld op de tijdpagina<br>Overuren die zijn aangemeld bij de tijdpagina </td> 
   <td><strong>Meteen</strong> </td> 
  </tr> 
 </tbody> 
</table>
