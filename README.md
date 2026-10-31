# Agent LinkedIn

Agent Claude Code `linkedin-manager` (défini dans `.claude/agents/linkedin-manager.md`).
Il s'appuie sur le plugin [linkedin-skills](https://github.com/sergebulaev/linkedin-skills).

## Installation du plugin (à faire une fois)

Dans Claude Code :

```
/plugin marketplace add sergebulaev/linkedin-skills
/plugin install linkedin-skills@linkedin-skills
```

Options (fichier `.env` à la racine du dossier du plugin, voir son `.env.example`) :
- `PUBLORA_API_KEY` + `LINKEDIN_PLATFORM_ID` : publication/programmation après validation
- `APIFY_TOKEN` : lecture des posts, fils et engagés sans login LinkedIn
- `PIXFARO_TOKEN` : génération de visuels

Sans ces clés, l'agent fonctionne en mode brouillon (copier-coller).

## Utilisation

- « Utilise l'agent linkedin-manager pour auditer mon profil »
- « linkedin-manager : écris mon post de demain sur … »
- « linkedin-manager : propose 5 commentaires sur ces posts : <URL> »
- « linkedin-manager : trouve 10 personnes actives à ajouter à partir des engagés de mon dernier post »

## Fichiers de mémoire

`profil-voix.md`, `story-bank.md`, `calendrier.md`, `reseau.md`, `journal.md`, lus et mis à jour par l'agent à chaque session.

## Garde-fous

Rien n'est publié sans ta validation. Les demandes de connexion et les messages privés sont préparés par l'agent mais envoyés **par toi** : LinkedIn interdit leur automatisation.
