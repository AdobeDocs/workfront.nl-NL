---
user-type: administrator
product-area: system-administration
keywords: wijzigen,e-mail,melding,instellingen,bulk,bulkbewerking,configureren,meerdere,gebruikers
navigation-topic: emails-administration
title: Meerdere gebruikers-instellingen voor e-mailmeldingen wijzigen
description: Dit artikel bevat informatie voor de Workfront of groepsbeheerders over hoe ze de e-mailmeldingen van andere gebruikers kunnen bijwerken.
author: Nolan
feature: System Setup and Administration
role: Admin
exl-id: 658f97cd-0500-421d-9c89-26041ca59655
source-git-commit: e34abb5ff1068de99eaba33dc95287164e556742
workflow-type: tm+mt
source-wordcount: '440'
ht-degree: 0%

---

# Instellingen voor e-mailmeldingen van meerdere gebruikers wijzigen

<!-- Audited: 12/2023 -->

Als u een Adobe Workfront-beheerder bent of als u een Planner-toegangsniveau hebt waarmee u de instellingen van andere gebruikers kunt bewerken, kunt u de meldingsinstellingen voor meerdere gebruikers tegelijk configureren. Dit omvat het specificeren of de gebruikers berichten ontvangen aangezien de gebeurtenissen gebeuren, of in één dagelijkse samenvatting e-mail, zoals die in [&#x200B; Adobe Workfront berichten &#x200B;](../../../workfront-basics/using-notifications/wf-notifications.md) wordt beschreven. Voor informatie over het toegangsniveau nodig om gebruikers uit te geven, zie [&#x200B; Toegang van de Verlening tot gebruikers &#x200B;](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md).

U kunt ook e-mailmeldingen voor één gebruiker tegelijk configureren, inclusief uw eigen profiel. Voor meer informatie, zie [&#x200B; uw eigen e-mailberichten wijzigen &#x200B;](../../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md).


## Toegangsvereisten

+++ Breid uit om de toegangseisen voor de functionaliteit in dit artikel weer te geven.


<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-pakket</td> 
   <td>Alle</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-licentie</td> 
   <td> 
    <p>Standard</p>
    <p>Plan</p>
   </td>
  </tr> 
 </tbody> 
</table>

Voor informatie, zie [&#x200B; vereisten van de Toegang in de documentatie van Workfront &#x200B;](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Instellingen voor e-mailmeldingen wijzigen voor meerdere gebruikers

Wanneer u berichtmontages in massa vormt, kunt u slechts de montages veranderen die de geselecteerde gebruikers in gemeenschappelijk hebben.

Wanneer u een bericht het plaatsen wijzigt, verschijnt het etiket **Bewerkte** voor dat bericht het plaatsen, om u te laten weten dat bericht het plaatsen is gewijzigd.

Instellingen voor e-mailmeldingen voor meerdere gebruikers wijzigen:

{{step-1-to-users}}

1. Selecteer de gebruikers, dan klik **uitgeven**.
1. In **geef Persoon** doos uit die verschijnt, klik **Meldingen**.

1. Vouw een categorie uit om meldingsinstellingen voor die categorie weer te geven.

   Als er minstens één gebruiker wordt geselecteerd waar de berichten niet de berichten van de andere geselecteerde gebruikers aanpassen, bevat het vakje van de categoriecontrole voor dat bericht een horizontale lijn ![&#x200B; Lijn in plaats van controle &#x200B;](assets/straight-line-instead-of-checkmark.jpg) in plaats van een vinkje.


1. Klik op de berichten die de gebruikers dagelijks of direct moeten ontvangen of op de berichten die u niet meer wilt ontvangen.

   >[!NOTE]
   >
   >   Voor de **Communicatie** categorie, kunt u individuele berichten voor onmiddellijke levering slechts selecteren. U moet alle berichten selecteren die in een dagelijkse samenvatting moeten worden geleverd.


1. Als u berichten selecteerde die als dagelijkse samenvatting moeten worden verzonden, selecteer de tijd van de dag u de samenvatting wilt die bij de bovenkant van de **sectie van Meldingen** in de **E-mail Dagelijkse Samenvatting na** menu wordt geleverd.

   ![&#x200B; Dagelijkse samenvattingstijd &#x200B;](assets/daily-digest-time.png)

   De dagelijkse samenvatting bevat gebeurtenissen die 24 uur vóór de geselecteerde tijd voldoen aan de criteria voor de meldingen. Gebruikers ontvangen één e-mail met dagelijkse samenvatting voor elk berichttype.

   De dagelijkse controlesamenvatting kan aankomen na de tijd die u selecteert, afhankelijk van het aantal e-mails in de wachtrij voor levering in het systeem. De vermelde tijd is uw lokale tijd zoals die in uw browser montages wordt gespecificeerd.
