---
title: Aanmeldingsgegevens van gebruikers weergeven
user-type: administrator
product-area: system-administration;user-management
navigation-topic: create-and-manage-users
description: U kunt zien hoe vaak de gebruikers zich bij Workfront aanmelden, evenals de laatste tijd zij het programma hebben geopend, door erop te wijzen dat u deze informatie in de mening van een lijst van gebruikers, of in een rapport voor gebruikers wilt omvatten.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 7b37c34a-d628-4d9b-9688-e4b9f89c666b
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '570'
ht-degree: 0%

---

# Aanmeldingsgegevens van gebruikers weergeven

U kunt zien hoe vaak de gebruikers zich bij Adobe Workfront aanmelden, evenals de laatste tijd zij het programma hebben geopend, door erop te wijzen dat u deze informatie in de mening van een lijst van gebruikers, of in een rapport voor gebruikers wilt omvatten.

## Toegangsvereisten

U moet het volgende hebben om de stappen in dit artikel uit te voeren:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-plan</td> 
   <td>Alle</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-licentie</td> 
   <td> <p>Plan </p>   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraties op toegangsniveau</td> 
   <td> <p>U moet een van de volgende opties hebben:</p> 
    <ul> 
     <li> <p>Het toegangsniveau van de Beheerder van het Systeem. Zie voor meer informatie <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Volledige administratieve toegang verlenen aan een gebruiker</a>. </p> </li> 
     <li> <p><b>Gebruikers</b> het plaatsen in uw toegangsniveau dat wordt gevormd aan <b>Bewerken</b> toegang, met <b>Maken</b> en ten minste één van beide <b>Gebruikersbeheerder</b> opties ingeschakeld onder <b>Uw instellingen nauwkeurig afstellen</b> <img src="assets/gear-icon-in-access-levels.png">. </p> <p>Van deze twee opties, als Gebruiker <b>Admin (Groepgebruikers)</b> wordt toegelaten, moet u een groepsbeheerder van een groep zijn waar de gebruiker een lid is.</p> <p>Voor meer informatie over de <b>Gebruikers</b> het plaatsen in een toegangsniveau, zie <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md" class="MCXref xref">Toegang verlenen aan gebruikers</a>.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

## Hoe Workfront aanmeldingsgegevens registreert

Workfront registreert de volgende informatie over gebruikers die zich aanmelden bij het systeem:

* **Aantal aanmeldingen**: Workfront telt elke 24 uur een gebruiker die zich aanmeldt bij de toepassing. Als een gebruiker zich meerdere keren aanmeldt met verschillende browsers, computers of mobiele apparaten, telt Workfront alle logins die zich op één dag hebben voorgedaan als één aanmelding. Het aantal aanmelding bevat gegevens die beginnen bij het maken van de gebruiker.
* **Laatste aanmeldingsdatum**: De laatste datum waarop een gebruiker zich heeft aangemeld. De datum van elke aanmelding van een browser, mobiel apparaat of andere toepassingen wordt in dit veld vastgelegd.

Aanmelden bij Workfront op een van de volgende manieren telt als aanmelding bij Workfront:

* De Workfront-webtoepassing
* De Workfront Mobile-apps (iOS- of Android-apparaten)
* Elke ondersteunde Workfront-integratie met een andere toepassing van derden (Slack, Jira)
* Elke aangepaste integratie tussen Workfront en een andere toepassing van derden.
* De Workfront API

   >[!NOTE]
   >
   >Aanmelden bij Workfront via de Workfront API is alleen beschikbaar voor organisaties die nog niet zijn aangemeld bij het Adobe Business Platform.

## Gebruiksgegevens weergeven in een gebruikerslijst of rapport

U kunt het Aantal Login en de Laatste gebieden van de Datum van Aanmelding in de mening van een lijst van gebruikers, of in een rapport voor gebruikers tonen.\
Voor meer informatie over het creëren van een rapport, zie [Een aangepast rapport maken](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).

Gebruiksinformatie weergeven in de weergave van een lijst met gebruikers:

1. Ga naar een lijst met gebruikers in Workfront.
1. Van de **Weergave** vervolgkeuzelijst, selecteert u **Nieuwe weergave**.

1. Klikken **Kolom toevoegen** in de rechterbenedenhoek van het scherm.
1. In de **Tonen in deze kolom** veld, beginnen met typen **Aantal aanmeldingen** en selecteert u de selectie wanneer deze in de lijst onder wordt weergegeven **Gebruiker**.

1. Klikken **Kolom toevoegen** opnieuw.
1. In de **Tonen in de kolom** veld, beginnen met typen **Laatste aanmeldingsdatum** en selecteert u de selectie wanneer deze in de lijst onder wordt weergegeven **Gebruiker**.

1. (Optioneel) Klik op **Geavanceerde opties** Selecteer vervolgens een **Veldindeling** in het keuzemenu om de tijd of de dag van de week van de laatste aanmelding in uw kolom op te nemen.

1. Klikken **Weergave opslaan**.\
   De weergave bevat informatie over het aantal keren dat de gebruikers zich hebben aangemeld en het tijdstip waarop ze zich voor het laatst hebben aangemeld.
