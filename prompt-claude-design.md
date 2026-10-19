# Prompt Claude Design : plateforme de logement étudiant à Rennes

> Copiez tout le bloc ci-dessous (entre les deux lignes) et collez-le dans Claude Design.
> Remplacez `[NOM DU SITE]` si vous avez choisi un autre nom que « Passe-Clé ».

---

Conçois le design complet d'un site web responsive (mobile en priorité, puis desktop) appelé **Passe-Clé** : une plateforme qui met en relation, à Rennes, les étudiants qui quittent leur logement et ceux qui en cherchent un. Toute l'interface est en français.

## Le problème à résoudre

À Rennes, chaque année, des milliers d'étudiants cherchent un logement au même moment, souvent à distance (étudiants venant d'autres villes ou de l'étranger), pendant que d'autres déménagent et laissent un logement libre. Les annonces sont dispersées sur des groupes Facebook, Leboncoin et le bouche-à-oreille, avec peu de photos, des informations incomplètes et beaucoup d'arnaques. Passe-Clé centralise ces logements « de passation » et permet de **visiter virtuellement** chaque logement grâce à une visite photo pièce par pièce, avec toutes les informations utiles et le contact du bailleur.

## Les deux publics

1. **L'étudiant qui part** : il veut publier son logement vite (en moins de 10 minutes depuis son téléphone), trouver un successeur fiable, et faciliter la relation avec son bailleur.
2. **L'étudiant qui cherche** : il veut filtrer rapidement par budget, quartier et proximité de son campus, voir le logement comme s'il y était, connaître le coût réel (loyer, charges, APL possibles) et contacter le bailleur ou l'étudiant sortant en confiance.

## Écrans à concevoir

### 1. Page d'accueil
- Accroche claire, par exemple : « Le logement de ceux qui partent, pour ceux qui arrivent. »
- Barre de recherche principale : campus ou quartier, budget maximum, date d'entrée souhaitée
- Deux boutons d'action bien distincts : « Je cherche un logement » et « Je libère mon logement »
- Raccourcis par campus : Rennes 1 Beaulieu, Rennes 2 Villejean, Centre-ville / Rennes 1 Droit-Éco, Ker Lann, La Harpe / Rennes 2, Saint-Jacques / Rennes School of Business, Cesson-Sévigné
- Section « Comment ça marche » en 3 étapes
- Section confiance : annonces vérifiées, conseils anti-arnaque, profils étudiants vérifiés
- Aperçu de 3 à 6 logements récents sous forme de cartes

### 2. Résultats de recherche
- Vue liste de cartes + vue carte (plan de Rennes avec repères des logements, lignes de métro A et B visibles)
- Bascule liste / carte sur mobile, affichage côte à côte sur desktop
- Filtres : budget (loyer charges comprises), type (studio, T1, T2, colocation, chambre chez l'habitant, résidence étudiante), meublé ou non, surface, date de disponibilité, éligible APL, temps de trajet vers un campus choisi, proche métro, animaux acceptés
- Tri : plus récent, prix croissant, plus proche de mon campus
- Chaque carte affiche : photo principale, loyer CC en grand, type et surface, quartier, temps de trajet vers le campus choisi, date de disponibilité, badge « Visite virtuelle » et badge « Annonce vérifiée » si applicable

### 3. Fiche logement avec visite virtuelle (écran le plus important)
- **Visite virtuelle photo** : un parcours guidé pièce par pièce (Entrée → Pièce principale → Cuisine → Salle de bain → Vue / extérieur → Immeuble et parties communes). Chaque étape montre plusieurs photos en plein écran, avec le nom de la pièce, sa surface si connue et une courte description. Navigation par flèches, swipe sur mobile et miniatures cliquables. Un bouton « Démarrer la visite » lance le parcours en plein écran.
- **Résumé en haut** : loyer, charges, total mensuel, dépôt de garantie, type, surface, étage, ascenseur, meublé ou non, date de disponibilité
- **Estimation du coût réel** : bloc qui récapitule loyer + charges + estimations (électricité, internet) et rappelle l'éligibilité aux APL (lien vers le simulateur de la CAF)
- **Localisation** : carte du quartier, temps de trajet à pied / vélo / bus / métro vers les principaux campus, commerces et transports à proximité
- **Équipements** : liste à icônes (lit, bureau, lave-linge, fibre, cuisine équipée, etc.)
- **Diagnostic énergétique (DPE)** : étiquette de A à G bien visible
- **Le bailleur** : type (particulier, agence, résidence), nom, moyen de contact (téléphone, e-mail), et conditions demandées (garant, garantie Visale acceptée, dossier requis). **Les coordonnées complètes ne s'affichent qu'aux utilisateurs connectés et vérifiés** (bouton « Voir les coordonnées du bailleur »), pour protéger le bailleur du démarchage et limiter les arnaques.
- **L'étudiant sortant** : prénom, établissement, date de départ, petit mot sur le logement (« Ce que j'ai aimé / ce qu'il faut savoir »), bouton « Envoyer un message »
- Boutons d'action fixes en bas sur mobile : « Contacter » et « Enregistrer »
- Encadré anti-arnaque discret : « Ne versez jamais d'argent avant d'avoir visité ou signé un bail. »
- Bouton « Signaler l'annonce »

### 4. Publication d'une annonce (parcours en étapes)
Un formulaire en 5 étapes avec barre de progression, pensé pour le mobile :
1. Le logement (adresse, type, surface, étage, meublé, équipements)
2. La visite virtuelle : l'utilisateur ajoute ses photos **pièce par pièce** (une section par pièce, avec un exemple de bonne photo et des conseils : lumière du jour, cadrage large, pièce rangée). Il peut réordonner les pièces par glisser-déposer.
3. Le coût (loyer, charges, dépôt de garantie, APL)
4. Le bailleur (type, nom, contact, conditions) avec une case à cocher obligatoire : « J'ai informé mon bailleur et il accepte d'être contacté via Passe-Clé »
5. Disponibilité et aperçu final de l'annonce telle qu'elle apparaîtra

### 5. Espace personnel
- Pour celui qui cherche : logements enregistrés, alertes de recherche (recevoir les nouvelles annonces correspondant à mes critères), messages
- Pour celui qui part : mes annonces, statistiques simples (vues, messages reçus), marquer comme « Logement attribué »
- Vérification du profil étudiant (e-mail universitaire ou certificat de scolarité)

### 6. Messagerie
- Conversation simple entre étudiants, avec la fiche du logement concerné rappelée en haut
- Messages pré-rédigés pour démarrer : « Le logement est-il toujours disponible ? », « Peut-on organiser une visite en visio ? »

### 7. Inscription et connexion
- Création de compte simple, choix du profil (je cherche / je pars / les deux), vérification étudiante

## Direction artistique

- **Ton** : chaleureux, rassurant, entre étudiants. Simple et lisible, jamais administratif.
- **Couleurs** : une couleur principale énergique et rassurante (par exemple un bleu ardoise ou un vert sapin, en clin d'œil à la Bretagne), une couleur d'accent chaude pour les boutons d'action (corail ou jaune doré), beaucoup de blanc. Prévois aussi un mode sombre.
- **Typographie** : une police sans-serif moderne et très lisible sur mobile, avec des titres affirmés.
- **Photos** : elles sont la star du site. Grandes, bord à bord sur mobile, coins légèrement arrondis.
- **Icônes** : style ligne, cohérent, pour les équipements et les informations pratiques.
- **Accessibilité** : contrastes conformes au niveau AA, textes et boutons assez grands pour une utilisation au pouce, libellés clairs sur tous les champs.
- N'utilise aucun logo officiel (ville de Rennes, universités, Star, CAF, CROUS) : seulement leurs noms en texte.

## Contenu d'exemple à utiliser dans les maquettes

Remplis les maquettes avec des annonces fictives réalistes, par exemple :
- Studio meublé de 22 m², quartier Villejean, 430 € CC, à 5 min à pied de Rennes 2, disponible le 1er juillet
- T1 de 30 m², quartier Beaulieu, 520 € CC, à 8 min à vélo de Rennes 1, fibre, DPE C
- Chambre en colocation de 12 m² dans un T4, Centre / Sainte-Anne, 390 € CC, métro ligne A à 2 min

Utilise des noms et coordonnées clairement fictifs pour les bailleurs (ex : « M. Exemple, 06 00 00 00 00 »).

## Ce que j'attends en sortie

1. Les maquettes des 7 écrans ci-dessus, en version mobile et desktop pour l'accueil, les résultats et la fiche logement
2. Un prototype cliquable du parcours principal : accueil → recherche → fiche logement → visite virtuelle → contact du bailleur
3. Une mini charte graphique : couleurs, typographies, boutons, cartes, badges et composants de formulaire réutilisables
