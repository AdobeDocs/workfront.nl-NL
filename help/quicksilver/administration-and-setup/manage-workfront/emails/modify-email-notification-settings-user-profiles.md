---
user-type: administrator
product-area: system-administration
keywords: wijzigen,e-mail,melding,instellingen,bulk,bulkbewerking,configureren,meerdere,gebruikers
navigation-topic: emails-administration
title: Instellingen voor e-mailmeldingen van meerdere gebruikers wijzigen
description: Dit artikel biedt informatie voor de Workfront of groepsbeheerders over hoe ze de e-mailmeldingen van andere gebruikers kunnen bijwerken.
author: Courtney
feature: System Setup and Administration
role: Admin
exl-id: 658f97cd-0500-421d-9c89-26041ca59655
source-git-commit: 6a6d3d47ed5741e3202c44b7240a2e67b687ea95
workflow-type: tm+mt
source-wordcount: '440'
ht-degree: 0%

---

# Instellingen voor e-mailmeldingen van meerdere gebruikers wijzigen

<!-- Audited: 12/2023 -->

Als u een Adobe Workfront-beheerder bent of als u een Planner Access-niveau hebt waarmee u de instellingen van andere gebruikers kunt bewerken, kunt u de meldingsinstellingen voor meerdere gebruikers tegelijk configureren. Dit omvat het specificeren of de gebruikers berichten ontvangen aangezien de gebeurtenissen gebeuren, of in één dagelijkse samenvatting e-mail, zoals die in [&#x200B; Adobe Workfront berichten &#x200B;](../../../workfront-basics/using-notifications/wf-notifications.md) wordt beschreven. Voor informatie over het toegangsniveau nodig om gebruikers uit te geven, zie [&#x200B; toegang van de Verlening tot gebruikers &#x200B;](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md).

U kunt ook e-mailmeldingen voor één gebruiker tegelijk configureren, inclusief uw eigen profiel. Voor meer informatie, zie [&#x200B; uw eigen e-mailberichten &#x200B;](../../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md) wijzigen.


## Toegangsvereisten

+++ Vouw uit om de toegangsvereisten voor de functionaliteit in dit artikel weer te geven.


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

Wanneer u berichtinstellingen in bulk configureert, kunt u alleen de instellingen wijzigen die de geselecteerde gebruikers gemeenschappelijk hebben.

Wanneer u een bericht het plaatsen wijzigt, verschijnt het etiket **Uitgegeven** voor dat bericht het plaatsen, om u te laten weten dat berichtplaatsing is gewijzigd.

Instellingen voor e-mailmeldingen voor meerdere gebruikers wijzigen:

{{step-1-to-users}}

1. Selecteer de gebruikers, dan klik **uitgeven**.
1. In **geef Persoon** doos uit die verschijnt, klik **Meldingen**.

1. Vouw een categorie uit om meldingsinstellingen voor die categorie weer te geven.

   Als er minstens één geselecteerde gebruiker is waar de berichten niet de berichten van de andere geselecteerde gebruikers aanpassen, bevat het vakje van de categoriecontrole voor dat bericht een horizontale lijn ![&#x200B; Lijn in plaats van controle &#x200B;](assets/straight-line-instead-of-checkmark.jpg) in plaats van een vinkje.


1. Klik op alle meldingen die u wilt dat gebruikers dagelijks of onmiddellijk ontvangen, of wissel alle meldingen die u niet meer wilt ontvangen.

   >[!NOTE]
   >
   >   Voor de **Communicatie** categorie, kunt u individuele berichten voor onmiddellijke slechts levering selecteren. U moet alle meldingen selecteren die u wilt verzenden in een dagelijks overzicht.


1. Als u berichten selecteerde om als dagelijkse samenvatting worden verzonden, selecteer de tijd van de dag u de samenvatting wilt die bij de bovenkant van de **sectie van Meldingen** in de **E-mail Dagelijkse Samenvatting na** menu wordt geleverd.

   ![&#x200B; Dagelijkse samenvattingstijd &#x200B;](assets/daily-digest-time.png)

   De dagelijkse samenvatting bevat gebeurtenissen die voldoen aan de criteria van de meldingen 24 uur voor de geselecteerde tijd. Gebruikers ontvangen één e-mail met een dagelijks overzicht voor elk berichttype.

   De dagsamenvatting komt mogelijk aan na de tijd die u selecteert, afhankelijk van het aantal e-mails dat in de wachtrij voor levering in het systeem staat. De vermelde tijd is uw lokale tijd zoals die in uw browser montages wordt gespecificeerd.
