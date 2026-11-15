# Cahier des Charges & Plan de Conception : Portfolio Développeur

## 1. Vision & Objectif du Projet
Créer un portfolio statique (HTML/CSS/JS) hébergé sur **GitHub Pages** pour présenter mon profil technique, mon évolution académique et mes projets de développement.
- **Positionnement actuel :** Étudiant en Bachelor Développement Logiciel.
- **Orientation future :** Préparation d'un Master en Systèmes Embarqués.
- **Objectif de carrière :** Travailler dans le domaine de la **simulation aéronautique**.
- **Stratégie de contenu :** Ayant une seule expérience professionnelle (stage), le portfolio doit prioritairement mettre en valeur mes **meilleurs projets GitHub**, ma rigueur technique et ma trajectoire vers l'embarqué et l'aéronautique.

---

## 2. Identité Visuelle & Direction Artistique (Thème "Cockpit / Station de Vol")
L'interface doit s'inspirer d'un **tableau de bord d'avion (Glass Cockpit)** ou d'une **console de simulation aéronautique** (HUD - Head-Up Display) : sobre, technique, lisible et précis.

### Palette de couleurs
- **Fond principal :** Gris anthracite très sombre / Noir cockpit (`#0B0E14` ou `#0D1117`)
- **Fond des cartes / modules :** Gris acier foncé (`#161B22`) avec bordures fines (`1px solid #30363D`)
- **Couleur primaire (Accents HUD) :** Vert émeraude / radar (`#00FF66` ou `#10B981`) ou Cyan avionique (`#38BDF8`)
- **Couleur secondaire (Alertes / Statuts) :** Ambre / Orange instrumentation (`#F59E0B`)
- **Texte principal :** Blanc cassé (`#E6EDF3`)
- **Texte secondaire :** Gris technique (`#8B949E`)

### Typographie & Éléments graphiques
- **Titres & Données techniques :** Police monospace (`JetBrains Mono`, `Fira Code` ou `Courier New`) pour rappeler les consoles de vol et terminaux.
- **Textes de lecture :** Police sans-serif moderne et très lisible (`Inter` ou `Roboto`).
- **Détails immersifs :**
  - Indicateurs de statut en haut de page (ex: `SYS_STATUS: ONLINE`, `TARGET: AEROSPACE_SIM`).
  - Séparateurs de sections gradués ou stylisés façon instruments de bord.
  - Coins légèrement biseautés ou bordures nettes sur les cartes de projets.

---

## 3. Architecture des Fichiers
Structure cible du dépôt GitHub :
```text
/
├── index.html          # Structure principale du portfolio (One-Page)
├── style.css           # Feuille de style (Thème Cockpit / Responsive)
├── script.js           # Interactions légères (navigation fluide, animations HUD)
├── portfolio.md        # Ce document de référence (spécifications)
└── assets/
    ├── img/            # Captures d'écran des projets et schémas
    └── cv.pdf          # Curriculum Vitae téléchargeable
```

---

## 4. Structure Détaillée de la Page (`index.html`)

### Section 1 : Barre de Navigation & HUD Header (Accueil)
- **Barre de navigation fixe :** Liens rapides vers *Plan de Vol*, *Hangar (Projets)*, *Carnet de Vol (Stage)*, *Systèmes (Compétences)*, *Contact*.
- **Hero Section :**
  - Badge statut : `BACHELOR DEV LOGICIEL ➔ MASTER SYSTÈMES EMBARQUÉS`
  - Titre principal (H1) : **Mon Nom / Prénom**
  - Accroche : *"Du développement logiciel aux systèmes embarqués : conception et simulation pour l'aéronautique."*
  - Boutons d'action (CTA) :
    1. `[ Explorer le Hangar ]` (Scroll vers les projets GitHub)
    2. `[ Télécharger le CV ]` (Lien vers `assets/cv.pdf`)

### Section 2 : Plan de Vol (À propos & Trajectoire)
Présentation chronologique et logique de mon parcours sous forme de points de passage (Waypoints) :
- **WP1 - Base Logicielle (Actuel) :** Bachelor Développement Logiciel. Acquisition des fondamentaux : algorithmique, programmation orientée objet, architecture logicielle et gestion de versions.
- **WP2 - Transition Bas Niveau (Prochaine étape) :** Master Systèmes Embarqués. Spécialisation sur les contraintes temps réel, l'interaction matériel/logiciel et l'optimisation des ressources.
- **WP3 - Destination Finale :** Ingénierie en Simulation Aéronautique. Conception de modèles physiques, d'interfaces homme-machine (IHM) avioniques et d'environnements de simulation.

### Section 3 : Le Hangar (Projets GitHub — Section Prioritaire)
Grille de cartes présentant mes **3 à 4 meilleurs dépôts GitHub**. Chaque carte doit être structurée comme une fiche technique :
- **En-tête de carte :** Nom du projet + Badge catégorie (ex: `SIMULATION`, `EMBARQUÉ / C++`, `LOGICIEL`).
- **Visuel :** Aperçu ou schéma technique du projet.
- **Description :** Contexte, problématique technique résolue et fonctionnement.
- **Stack technique :** Tags des langages/outils utilisés (ex: `C++`, `Python`, `C`, `Git`, etc.).
- **Liens :** Bouton vers le **Code Source (GitHub)** + Bouton **Démo / Documentation** (si disponible).

*(À compléter avec mes projets spécifiques)* :
- [ ] **Projet 1 :** [Nom du repo] - [Courte description]
- [ ] **Projet 2 :** [Nom du repo] - [Courte description]
- [ ] **Projet 3 :** [Nom du repo] - [Courte description]

### Section 4 : Carnet de Vol (Expérience Professionnelle)
Mise en valeur de mon stage de développement :
- **Intitulé du poste & Entreprise** | Dates
- **Missions réalisées :** Liste concise (3 à 4 points) des tâches techniques accomplies.
- **Compétences transférables :** Rigueur de développement, travail en équipe, débogage, respect d'un cahier des charges.

### Section 5 : Systèmes & Avionique (Compétences Techniques)
Organisation claire par pôles de compétences (sans barres de pourcentage subjectives) :
- **Langages de programmation :** C, C++, Python, Java, JavaScript, HTML/CSS, SQL.
- **Systèmes & Embarqué :** Linux, notions de programmation bas niveau / temps réel, architectures matérielles.
- **Outils & Environnement :** Git, GitHub, VS Code, IDEs C/C++, documentation Markdown.

### Section 6 : Tour de Contrôle (Contact & Footer)
- Appel à l'action simple pour une prise de contact (recherche d'alternance/stage ou échanges techniques).
- Liens directs avec icônes :
  - **GitHub :** `https://github.com/mon-profil`
  - **LinkedIn :** `https://linkedin.com/in/mon-profil`
  - **Email :** `mon.email@exemple.com`

---

## 5. Instructions pour l'Assistant IA (Copilot)
Lorsque je te demande de générer ou modifier le code de ce portfolio :
1. **Respecte strictement** la direction artistique sombre façon cockpit/HUD définie en section 2.
2. **Privilégie un code propre, sémantique et sans dépendances lourdes** (HTML5, CSS3 moderne avec Flexbox/Grid et variables CSS, JavaScript vanilla léger) pour une compatibilité immédiate avec GitHub Pages.
3. **Assure le Responsive Design** : l'interface doit rester lisible et structurée sur ordinateur comme sur mobile.
4. **Mets en avant la section "Le Hangar" (Projets GitHub)** comme élément central de la page.