# Audit du profil LinkedIn de Karim : 31/10/2026

**Statut : audit en attente de données.** Aucune section n'est notée : il manque le contenu réel du profil.

Ce document contient :
1. ce qui a été cherché et pourquoi l'audit n'a pas pu être noté,
2. la grille d'audit qui sera appliquée, section par section,
3. les recommandations qui valent quel que soit le contenu actuel,
4. la liste précise de ce que Karim doit fournir.

Méthode : skill `linkedin-profile-optimizer` du plugin linkedin-skills (sergebulaev/linkedin-skills). Le plugin n'est pas installé dans cette session, donc la méthode a été reprise depuis la description publique du skill sur GitHub.

---

## 1. Sources consultées

| Source | Résultat |
|---|---|
| `linkedin/profil-voix.md` | Modèle vide : objectif, audience, langue et positionnement non renseignés |
| `linkedin/story-bank.md` | Modèle vide |
| `linkedin/calendrier.md`, `reseau.md`, `journal.md` | Modèles vides |
| Autres fichiers du dépôt (`.claude/`, `README.md`) | Configuration de l'agent et du plugin uniquement. Aucune URL de profil, aucun export, aucun texte de profil |
| Plugin `linkedin-skills` | Déclaré dans `.claude/settings.json`, mais pas installé dans cette session (skills introuvables) |
| Recherche web sur le nom | Refusée par l'outil de recherche (pas de recherche de personnes par nom) |
| `linkedin.com` | Domaine bloqué par le réseau de la session. Même accessible, LinkedIn affiche un mur de connexion aux visiteurs non connectés |

Le skill impose aussi de ne pas noter un profil à partir de son URL seule : il faut le texte réel de chaque section et des captures d'écran pour les éléments visuels.

---

## 2. Grille d'audit (à appliquer dès réception des données)

Notation par section : **OK** / **À améliorer** / **Insuffisant**, puis score global sur 100.

| # | Section | Critères | Poids | Note actuelle |
|---|---|---|---|---|
| 1 | Photo | Récente, bien éclairée, visage net qui occupe environ 60 % du cadre, fond neutre | 10 | Non notée (pas de données) |
| 2 | Bannière | 1584 x 396 px, contraste fort, proposition de valeur et appel à l'action lisibles sur mobile (attention à la zone masquée par la photo) | 5 | Non notée |
| 3 | Titre | Utilise les 220 caractères. Structure : ce que je fais, pour qui, avec quel résultat. Mots-clés que l'audience cible tape dans la recherche | 20 | Non noté |
| 4 | Infos (À propos) | 200 à 300 mots, à la première personne, accroche forte dans les ~200 premiers caractères (avant « voir plus »), paragraphes courts, preuves chiffrées, appel à l'action final | 20 | Non noté |
| 5 | Sélection (Featured) | 3 éléments alignés sur l'objectif (offre, preuve, contenu phare), avec vignettes personnalisées | 10 | Non notée |
| 6 | Expériences | Chaque puce = verbe d'action + résultat mesurable. Plusieurs compétences rattachées par poste. Médias joints sur les postes clés | 15 | Non notées |
| 7 | Compétences | Jusqu'à 50, les 3 principales épinglées et alignées sur l'objectif, chacune validée au moins une fois | 5 | Non notées |
| 8 | Recommandations | Au moins 3 récentes, précises, de contextes variés (client, manager, pair) | 5 | Non notées |
| 9 | URL personnalisée | Basée sur le nom (ex. `linkedin.com/in/prenom-nom`), pas l'identifiant par défaut avec chiffres | 5 | Non notée |
| 10 | Activité | Publications ou commentaires dans les 30 derniers jours, régularité, cohérence avec les piliers | 5 | Non notée |
| — | Cohérence du positionnement | Titre, À propos, Sélection, expériences et activité racontent la même promesse à la même audience | transverse | Non notée |

---

## 3. Recommandations valables quel que soit le profil actuel

Ces points sont des bonnes pratiques à vérifier dès maintenant. Ils ne disent rien du profil de Karim tant qu'on ne l'a pas vu.

1. **Définir l'objectif et l'audience avant toute réécriture.** Un titre pour trouver des clients ne ressemble pas à un titre pour décrocher un poste. C'est le préalable à tout le reste (à renseigner dans `profil-voix.md`).
2. **Titre : remplacer l'intitulé de poste seul par une promesse.** Modèle : `[Ce que je fais] pour [qui] | [résultat ou preuve chiffrée] | [2e mot-clé]`, en utilisant les 220 caractères.
3. **À propos : soigner les 2 premières lignes.** C'est la seule partie visible avant « voir plus ». Commencer par le problème de l'audience ou par un résultat concret, pas par « Passionné par… ».
4. **Sélection : 3 éléments** (souvent vide sur la plupart des profils) : 1 qui présente l'offre ou le service, 1 preuve (étude de cas, résultat, témoignage réel), 1 contenu phare (meilleur post ou article).
5. **URL personnalisée** : vérifier qu'elle est au format `linkedin.com/in/prenom-nom` (Paramètres > Profil public). Gain rapide, 2 minutes.
6. **Expériences** : réécrire les 2 postes les plus récents en puces « verbe + résultat chiffré ».
7. **Recommandations** : demander 3 recommandations ciblées avec un message personnalisé qui suggère un angle précis (un projet, un résultat), plutôt que le modèle générique de LinkedIn.
8. **À éviter partout** : la troisième personne, « passionné », « orienté résultats », « leader d'opinion », les gros blocs de texte sans retour à la ligne.

---

## 4. Propositions de réécriture

**Pas encore possibles.** Le titre et la section À propos seront réécrits (2 à 3 variantes chacun) dès que les éléments de la section 5 seront disponibles. Aucune version n'est proposée ici pour ne rien inventer sur le parcours de Karim.

Modèle de structure qui sera utilisé pour l'À propos (7 blocs) :
1. Accroche : le problème de l'audience ou un résultat marquant (avant « voir plus »)
2. Pour qui je travaille
3. Ce que je fais concrètement
4. Preuves : chiffres, clients ou projets (avec accord)
5. Ce qui me différencie : méthode, parcours, prise de position
6. Un élément personnel court
7. Appel à l'action : comment me contacter, ce que je propose

---

## 5. Ce que Karim doit fournir

**Option la plus simple : l'export PDF du profil.** Sur son profil : bouton « Plus » > « Enregistrer au format PDF ». Puis le déposer dans `linkedin/` ou le coller ici.

Sinon, copier-coller ou fournir :

**Contenu du profil**
- [ ] Le titre (headline) exact
- [ ] Le texte complet de la section Infos / À propos
- [ ] Les expériences : intitulé, entreprise, dates, description de chaque poste (au moins les 3 derniers)
- [ ] La liste des compétences, et les 3 épinglées
- [ ] Le nombre de recommandations reçues (et 1 ou 2 extraits)
- [ ] Le contenu de la section Sélection (ou « vide »)
- [ ] L'URL du profil (pour vérifier si elle est personnalisée)
- [ ] Une capture d'écran du haut du profil (photo + bannière + titre), si possible aussi en version mobile
- [ ] Les 3 à 5 derniers posts ou commentaires publiés, avec leur date (pour l'activité et la voix)
- [ ] Formation, certifications, langues, si pertinentes pour l'objectif

**Contexte (pour `profil-voix.md`)**
- [ ] Objectif principal sur LinkedIn : clients, emploi, recrutement, notoriété, autre
- [ ] Audience cible : qui doit avoir envie de le contacter après lecture du profil (fonction, secteur, taille d'entreprise, zone)
- [ ] Langue de publication : français, anglais ou les deux
- [ ] Offre ou poste visé, en une phrase
- [ ] 2 ou 3 résultats chiffrés dont il est fier, utilisables publiquement

**Option technique (facultative)**
- Autoriser `www.linkedin.com` dans les réglages réseau de la session et configurer `APIFY_TOKEN` dans le `.env` du plugin. Même dans ce cas, le texte collé par Karim reste la source la plus fiable.
- Installer le plugin dans Claude Code : `/plugin install linkedin-skills@linkedin-skills`.

---

## 6. Prochaines étapes

1. Karim fournit l'export PDF (ou les textes) et répond aux 5 questions de contexte.
2. Notation des 10 sections et score global, classement des corrections par impact.
3. Réécriture du titre (3 variantes) et de l'À propos (2 variantes), puis des puces d'expérience.
4. Session `linkedin-interviewer` pour remplir `story-bank.md` (matière pour les preuves de l'À propos).
5. Karim applique lui-même les modifications sur LinkedIn (aucune API ne modifie le profil).
