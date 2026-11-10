<p align="center">
  <picture>
    <source media="(prefers-color-scheme: dark)" srcset="brand/logo-horizontal-dark.svg">
    <img src="brand/logo-horizontal.svg" alt="Atelier" width="440">
  </picture>
</p>

<p align="center">
  <b>Atelier de développement : lanceur de projets, ports réseau et dépôts Git réunis dans une seule application de bureau.</b><br>
  <sub>Electron · Angular · Spring Boot 3 · Java 17</sub>
</p>

<p align="center">
  <a href="../../releases/latest"><img alt="Télécharger pour Windows" src="https://img.shields.io/badge/Windows-T%C3%A9l%C3%A9charger%20l'installeur-22D3EE?style=for-the-badge&labelColor=101833"></a>
</p>

---

## Pourquoi Atelier ?

Au quotidien, un développeur Java / Angular jongle entre un terminal pour lancer ses services, un outil pour savoir quel processus occupe le port 8080, et un client Git. **Atelier réunit ces trois gestes dans une seule fenêtre.** Le logo représente cette idée : trois modules reliés à un même cœur.

## Modules

### 🚀 Lanceur
- Détection des projets du poste
- Lancement des applications Spring Boot et suivi des logs
- Bouton « Tout arrêter »

### 🔌 Ports
- Liste des ports en écoute et des connexions TCP
- Libération d'un port occupé
- Recherche d'un port libre et test d'un port

### 🌿 Espace Git
- Clone, commit et merge
- Règles de message de commit (expressions régulières)
- Commit et push programmés, sauvegardes
- Création de dépôts GitHub / Bitbucket, token stocké chiffré

### ⚙️ DevOps
- Génération de Jenkinsfile
- Quality Gate SonarQube
- Cible de déploiement

## Architecture

| Couche | Technologie |
|---|---|
| Application de bureau | Electron |
| Interface | Angular · TypeScript |
| Service local (GitDock) | Spring Boot 3.5 · Java 17 · H2 · Flyway · JPA |
| Runtime | JRE embarqué, aucune installation de Java requise |

Le service local écoute uniquement sur `127.0.0.1` et chaque démarrage génère une nouvelle clé d'API (`X-GitDock-Key`).

## Installation (Windows)

1. Télécharger `Atelier-Setup-0.1.0.exe` depuis la page [Releases](../../releases/latest).
2. Lancer l'installeur. L'application s'installe dans `%LOCALAPPDATA%\Programs\Atelier`.
3. Les données locales sont stockées dans `%APPDATA%\GitDock`.

## Identité visuelle

Le dossier [`brand/`](brand) contient le logo et toutes les icônes : SVG, PNG de 32 à 1024 px, `icon.ico` Windows, favicon et icônes de barre système.

| Cyan | Violet | Nuit |
|---|---|---|
| `#22D3EE` | `#A78BFA` | `#101833` |

---

## English

**Atelier** is a desktop developer workbench that brings together a project launcher, network port tools and a Git workspace in a single app (Electron, Angular, Spring Boot 3, Java 17). Download the Windows installer from [Releases](../../releases/latest).

---

<p align="center"><sub>© 2026 Rached Chakchouk · Tous droits réservés</sub></p>
