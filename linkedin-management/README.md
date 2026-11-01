# LinkedIn Management

Projet Claude Code autonome qui regroupe tout mon travail LinkedIn. **Ouvre Claude Code dans ce dossier** (`linkedin-management/`) pour que l'agent, le skill et le plugin soient chargés.

```
linkedin-management/
├── CLAUDE.md                     instructions lues à l'ouverture du projet
├── .claude/
│   ├── settings.json             active le plugin linkedin-skills
│   ├── agents/linkedin-manager.md
│   └── skills/linkedin-roast/
└── memoire/                      voix, story bank, calendrier, réseau, journal
```

- **Agent `linkedin-manager`** : profil, posts, commentaires, réseau. Il s'appuie sur le plugin [linkedin-skills](https://github.com/sergebulaev/linkedin-skills).
- **Skill `/linkedin-roast`** (repris de [alexyc9381/linkedin-roast-skill](https://github.com/alexyc9381/linkedin-roast-skill), licence MIT) : cinq relectures indépendantes du profil, puis sa réécriture.
- **`memoire/`** : fichiers lus et mis à jour par l'agent à chaque session.

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

## Garde-fous

Rien n'est publié sans ta validation. Les demandes de connexion et les messages privés sont préparés par l'agent mais envoyés **par toi** : LinkedIn interdit leur automatisation.
