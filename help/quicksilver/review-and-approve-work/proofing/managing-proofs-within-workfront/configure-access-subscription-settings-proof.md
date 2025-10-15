---
product-area: documents;system-administration;setup
navigation-topic: manage-proofs-within-workfront
title: Toegang- en abonnementsinstellingen configureren voor een proefdruk
description: U kunt bepaalde toegangs en abonnementsmontages voor individuele proefdrukken vormen, zoals of om gebruikers te vereisen login en of om gebruikers toe te staan om op de proef in te tekenen. U kunt toegang- en abonnementsinstellingen instellen voor een proefdruk terwijl u deze maakt, of u kunt deze instellingen instellen voor een proefdruk die al in Workfront bestaat.
author: Courtney
feature: Digital Content and Documents
exl-id: f242887b-d768-4d56-b530-a1ac6294b2d4
source-git-commit: ac714bd5a5259d6f995ac445efbd0125e07022cb
workflow-type: tm+mt
source-wordcount: '860'
ht-degree: 0%

---

# Toegang- en abonnementsinstellingen configureren voor een proefdruk

U kunt bepaalde toegangs en abonnementsmontages voor individuele proefdrukken vormen, zoals of om gebruikers te vereisen login en of om gebruikers toe te staan om op de proef in te tekenen. U kunt toegang- en abonnementsinstellingen instellen voor een proefdruk terwijl u deze maakt, of u kunt deze instellingen instellen voor een proefdruk die al in Workfront bestaat.

## Toegangsvereisten

+++ Breid uit om de toegangseisen voor de functionaliteit in dit artikel weer te geven.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-pakket</td> 
   <td> <p>Alle</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-licentie</td> 
   <td> 
   <p>Standard</p>
   <p>Werken of plannen</p> 
    </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Bewijs van machtigingsprofiel </td> 
   <td>Manager of hoger</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraties op toegangsniveau</td> 
   <td> <p>Toegang tot documenten bewerken</p></td> 
  </tr> 
 </tbody> 
</table>

Voor informatie, zie [&#x200B; vereisten van de Toegang in de documentatie van Workfront &#x200B;](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Toegang- en abonnementsinstellingen configureren tijdens het maken van een proefdruk

Als u toegang- en abonnementsinstellingen voor een proefdruk wilt instellen terwijl u de proefdruk maakt:

1. Ga naar het project, de taak, of de kwestie waar u de proef wilt, dan klik de **sectie van Documenten**.
1. Klik **toevoegen Nieuw** op het hoger-juiste gebied.
1. De rol aan de **sectie van de Montages van het Bewijs** in de laag-juiste hoek van de **Nieuwe proef** pagina.

1. Configureer de volgende instellingen:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong> Toestaan het delen van bewijs via openbare URL of bedt code </strong> in </td> 
      <td>Als deze optie is geselecteerd, kan de proefdruk worden gedeeld via een openbare URL of insluitcode.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong> sta het abonneren op bewijs via openbare URL toe of bedt code </strong> in </td> 
      <td>Als deze optie is geselecteerd, kunnen personen die niet expliciet aan de proefdruk zijn toegevoegd, zich op de proefdruk abonneren. De persoon die zich op de proef abonneert, krijgt de rol en e-mail die u in de volgende montages bepaalt:
       <ul>
        <li><p><strong> de rol van de Abonnee:</strong> de standaardproefdrukrol die aan alle recensenten wordt toegewezen die aan de proef intekenen. </p><p>Belangrijk: Als <strong> het Delen met </strong> toestaat wordt geplaatst aan om het even wat buiten <strong> iedereen </strong> in de montages van Workfront Proof, het abonnementswerk slechts voor mensen binnen de organisatie. Voor meer informatie, zie <a href="../../../workfront-proof/wp-work-proofsfiles/manage-your-work/configure-proof-settings.md" class="MCXref xref"> de Montages van het Bewijs in Workfront Proof </a> vormen.</p></li>
        <li><strong> e-mail waakzame montages voor abonnees:</strong> het standaard e-mailalarm dat aan alle recensenten wordt toegewezen die aan de proef intekenen.</li>
       </ul><p>
        <ul>
         <li><strong> vereiste toegang van het Bewijs via e-mailverbinding voor:</strong> Vorm of de abonnee een e-mail met een verbinding aan de proef ontvangt. U kunt <strong> Geen e-mail </strong> selecteren (de e-mailverbinding wordt niet vereist om tot de proef toegang te hebben), <strong> het bericht van het Bewijs slechts </strong> (de abonnee ontvangt een verbinding aan de proef via e-mail zonder enige controle), of <strong> Bevestiging en proef bericht e-mails </strong> (de abonnee ontvangt een verbinding aan de proef via e-mail en moet de verbinding klikken om tot een proef toegang te hebben, is het doel van deze optie ervoor te zorgen dat de persoon een correct is ingegaan e-mailadres waartoe zij toegang hebben).</li>
        </ul><p>Opmerking:  Als de proefdrukken de Geautomatiseerde Werkstroom in bijlage hebben alle abonnementen zullen bevestigingse-mail aan de bewijseigenaars produceren, zodat kunnen zij beslissen welk stadium de persoon aan zou moeten worden toegevoegd.<br></p></p></td> 
     </tr> 
    </tbody> 
   </table>

1. Blijf uw proefdruk maken.

## Toegang- en abonnementsinstellingen configureren voor een bestaande proefdruk

U kunt als volgt toegangs- en abonnementsinstellingen instellen voor een proefdruk die al in Workfront bestaat:

1. In het gebied van Documenten, selecteer het document dat de proef bevat u montages voor wilt vormen, dan **Details van het Document** klikken.
1. In het linkerpaneel, klik **het Proofing de Montages van de Kijker**.
1. Configureer de volgende instellingen:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong> staat het delen van bewijs via openbare URL toe of bedt code </strong> <strong> e </strong> in </td> 
      <td>Als deze optie is geselecteerd, kan de proefdruk worden gedeeld via een openbare URL of insluitcode.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong> sta het abonneren op bewijs via openbare URL toe of bedt code </strong> in </td> 
      <td>Als deze optie is geselecteerd, kunnen personen die niet expliciet aan de proefdruk zijn toegevoegd, zich op de proefdruk abonneren. De persoon die zich op de proef abonneert, krijgt de rol en e-mail die u in de volgende montages bepaalt:
       <ul>
        <li><p><strong> de rol van de Abonnee:</strong> de standaardproefdrukrol die aan alle recensenten wordt toegewezen die aan de proef intekenen. </p><p>Belangrijk: Als <strong> het Delen met </strong> toestaat wordt geplaatst aan om het even wat buiten <strong> iedereen </strong> in de montages van Workfront Proof, het abonnementswerk slechts voor mensen binnen de organisatie. Voor meer informatie, zie <a href="../../../workfront-proof/wp-work-proofsfiles/manage-your-work/configure-proof-settings.md" class="MCXref xref"> de Montages van het Bewijs in Workfront Proof </a> vormen.</p></li>
        <li><strong> e-mail waakzame montages voor abonnees:</strong> het standaard e-mailalarm dat aan alle recensenten wordt toegewezen die aan de proef intekenen.</li>
       </ul><p>
        <ul>
         <li><strong> vereiste toegang van het Bewijs via e-mailverbinding voor:</strong> Vorm of de abonnee een e-mail met een verbinding aan de proef ontvangt. U kunt <strong> Geen e-mail </strong> selecteren (de e-mailverbinding wordt niet vereist om tot de proef toegang te hebben), <strong> het bericht van het Bewijs slechts </strong> (de abonnee ontvangt een verbinding aan de proef via e-mail zonder enige controle), of <strong> Bevestiging en proef bericht e-mails </strong> (de abonnee ontvangt een verbinding aan de proef via e-mail en moet de verbinding klikken om tot een proef toegang te hebben, is het doel van deze optie ervoor te zorgen dat de persoon een correct is ingegaan e-mailadres waartoe zij toegang hebben).</li>
        </ul><p>Opmerking:  Als de proefdrukken de Geautomatiseerde Werkstroom in bijlage hebben alle abonnementen zullen bevestigingse-mail aan de bewijseigenaars produceren, zodat kunnen zij beslissen welk stadium de persoon aan zou moeten worden toegevoegd.<br></p></p></td> 
     </tr> 
    </tbody> 
   </table>

1. Klik **sparen**.
