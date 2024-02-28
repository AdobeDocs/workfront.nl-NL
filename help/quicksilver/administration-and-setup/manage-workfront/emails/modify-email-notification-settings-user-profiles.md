---
user-type: administrator
product-area: system-administration
keywords: wijzigen,e-mail,melding,instellingen,bulk,bulkbewerking,configureren,meerdere,gebruikers
navigation-topic: emails-administration
title: Instellingen voor e-mailmeldingen van meerdere gebruikers wijzigen
description: Dit artikel bevat informatie voor de Workfront of groepsbeheerders over hoe ze de e-mailmeldingen van andere gebruikers kunnen bijwerken.
author: Nolan
feature: System Setup and Administration
role: Admin
exl-id: 658f97cd-0500-421d-9c89-26041ca59655
source-git-commit: 1c0a656f2603c5decabd2bb4e88da1b9530f9e1c
workflow-type: tm+mt
source-wordcount: '447'
ht-degree: 0%

---

# Instellingen voor e-mailmeldingen van meerdere gebruikers wijzigen

<!-- Audited: 12/2023 -->

Als u een Adobe Workfront-beheerder bent of als u een Planner-toegangsniveau hebt waarmee u de instellingen van andere gebruikers kunt bewerken, kunt u de meldingsinstellingen voor meerdere gebruikers tegelijk configureren. Dit omvat het opgeven of gebruikers meldingen ontvangen wanneer gebeurtenissen plaatsvinden, of in één e-mail met dagelijkse controlesamenvatting, zoals beschreven in [Adobe Workfront-berichten](../../../workfront-basics/using-notifications/wf-notifications.md). Voor informatie over het toegangsniveau nodig om gebruikers uit te geven, zie [Toegang verlenen aan gebruikers](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md).

U kunt ook e-mailmeldingen voor één gebruiker tegelijk configureren, inclusief uw eigen profiel. Zie voor meer informatie [Uw eigen e-mailmeldingen wijzigen](../../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md).


## Toegangsvereisten

U moet de volgende toegang hebben om de stappen in dit artikel uit te voeren:

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
   <td> <p>Nieuw abonnement: standaard </p>
 <p>of</p> 
<p>Huidig plan: Plan </p> 
</td> 
  </tr> 
 </tbody> 
</table>

Zie voor meer informatie over de informatie in deze tabel [Toegangsvereisten in Workfront-documentatie](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

## Instellingen voor e-mailmeldingen wijzigen voor meerdere gebruikers

Wanneer u berichtmontages in massa vormt, kunt u slechts de montages veranderen die de geselecteerde gebruikers in gemeenschappelijk hebben.

Als u een meldingsinstelling wijzigt, wordt het label **Bewerkt** verschijnt voor die bericht het plaatsen, om u te laten weten dat die bericht het plaatsen is gewijzigd.

Instellingen voor e-mailmeldingen voor meerdere gebruikers wijzigen:

{{step-1-to-users}}

1. Selecteer de gebruikers en klik vervolgens op **Bewerken**.
1. In de **Persoon bewerken** vak dat wordt weergegeven, klikt u op **Meldingen**.

1. Vouw een categorie uit om meldingsinstellingen voor die categorie weer te geven.

   Als er ten minste één gebruiker is geselecteerd die niet overeenkomt met de meldingen van de andere geselecteerde gebruikers, bevat het selectievakje voor categorie van die melding een horizontale lijn ![](assets/straight-line-instead-of-checkmark.jpg) in plaats van een vinkje.


1. Klik op de berichten die de gebruikers dagelijks of direct moeten ontvangen of op de berichten die u niet meer wilt ontvangen.

   >[!NOTE]
   >
   >   Voor de **Communicatie** rubriek, kunt u afzonderlijke meldingen selecteren voor alleen directe levering. U moet alle berichten selecteren die in een dagelijkse samenvatting moeten worden geleverd.


1. Als u meldingen hebt geselecteerd die als een dagelijkse samenvatting moeten worden verzonden, selecteert u de tijd van de dag waarop u de samenvatting boven aan het dialoogvenster wilt verzenden **Meldingen** in de **Dagelijkse samenvatting e-mailen na** -menu.

   ![](assets/daily-digest-time.png)

   De dagelijkse samenvatting bevat gebeurtenissen die 24 uur vóór de geselecteerde tijd voldoen aan de criteria voor de meldingen. Gebruikers ontvangen één e-mail met dagelijkse samenvatting voor elk berichttype.

   De dagelijkse controlesamenvatting kan aankomen na de tijd die u selecteert, afhankelijk van het aantal e-mails in de wachtrij voor levering in het systeem. De vermelde tijd is uw lokale tijd zoals die in uw browser montages wordt gespecificeerd.
