# LinkedIn Management

Tout ce qui sert à gérer ma présence LinkedIn avec Claude Code :

- **Agent `linkedin-manager`** (`.claude/agents/linkedin-manager.md`) : profil, posts, commentaires, réseau. Il s'appuie sur le plugin [linkedin-skills](https://github.com/sergebulaev/linkedin-skills).
- **Skill `/linkedin-roast`** (`.claude/skills/linkedin-roast/`, repris de [alexyc9381/linkedin-roast-skill](https://github.com/alexyc9381/linkedin-roast-skill), licence MIT) : cinq relectures indépendantes du profil, puis sa réécriture.
- **Fichiers de mémoire** (ce dossier) : lus et mis à jour par l'agent.

L'agent et le skill restent dans `.claude/` à la racine du dépôt : c'est là que Claude Code les cherche.

## Installation du plugin (à faire une fois)

Dans Claude Code :

```
/plugin marketplace add sergebulaev/linkedin-skills
/plugin install linkedin-skills@linkedin-skills
```

Options (fichier `.env` à la racine du dossier du plugin, voir son `.env.example`) :
- `PUBLORA_API_KEY` + `LINKEDIN_PLATFORM_ID` : publication et programmation après validation
- `APIFY_TOKEN` : lecture des posts, des fils et des personnes qui interagissent, sans connexion LinkedIn
- `PIXFARO_TOKEN` : génération de visuels

Sans ces clés, l'agent fonctionne en mode brouillon (copier-coller).

## Utilisation

- `/linkedin-roast mon-profil.pdf` : critique et réécriture du profil
- « Utilise l'agent linkedin-manager pour auditer mon profil »
- « linkedin-manager : écris mon post de demain sur … »
- « linkedin-manager : propose des commentaires sur ces posts : <URL> »
- « linkedin-manager : trouve 10 personnes actives à ajouter parmi celles qui ont réagi à mon dernier post »

## Fichiers de mémoire

`profil-voix.md`, `story-bank.md`, `calendrier.md`, `reseau.md`, `journal.md`, lus et mis à jour par l'agent à chaque session.

## Garde-fous

Rien n'est publié sans ta validation. Les demandes de connexion et les messages privés sont préparés par l'agent mais envoyés **par toi** : LinkedIn interdit leur automatisation.
