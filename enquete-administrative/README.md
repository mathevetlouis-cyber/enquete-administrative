# 📋 Enquête Administrative - Outil Professionnel

Outil de conduite d'enquête administrative pour les collectivités territoriales françaises.

![Version](https://img.shields.io/badge/version-1.0-blue)
![License](https://img.shields.io/badge/licence-MIT-green)
![HTML](https://img.shields.io/badge/HTML-CSS--JS-orange)

## 📋 Description

Application web permettant aux collectivités territoriales, centres de gestion (CDG), directions des ressources humaines et référents déontologues de conduire et documenter une **enquête administrative interne** de manière structurée, dans le respect du contradictoire et des droits de la défense.

L'outil guide l'enquêteur à travers les 9 étapes clés d'une enquête administrative, de l'ouverture à la génération du rapport final.

### Fonctionnalités principales

- **Parcours guidé en 9 étapes** : contexte, personnes concernées, chronologie, preuves, auditions, témoins, qualification juridique, analyse, conclusions
- **Suivi des délais** : calcul automatique des jours écoulés avec alertes visuelles (délai recommandé de 60 jours)
- **Barre de progression** : visualisation de l'avancement global de l'enquête
- **Tableau de bord** : statistiques en temps réel (personnes, témoins, auditions, documents)
- **Qualification juridique assistée** : 20 manquements pré-définis (probité, harcèlement, conflits d'intérêts, etc.)
- **Modèles de questions d'audition** : banque de questions organisées par thème (contexte, faits, preuves, conséquences)
- **Rappels juridiques** : encadrés sur le principe du contradictoire, le cadre des auditions, le RGPD
- **Notes privées** : espace de travail non inclus dans le rapport final
- **Sauvegarde automatique** : toutes les 30 secondes via localStorage
- **Génération de rapport** : export du rapport d'enquête complet au format texte

## 🚀 Démarrage rapide

### Utilisation en ligne

Ouvrez directement le fichier `index.html` dans votre navigateur. Aucune installation requise.

```bash
git clone https://github.com/VOTRE-UTILISATEUR/enquete-administrative.git
open index.html
```

### Déploiement sur GitHub Pages

1. Forkez ce dépôt
2. Allez dans **Settings** → **Pages**
3. Sélectionnez la branche `main` et le dossier `/ (root)`
4. L'outil sera accessible à `https://VOTRE-UTILISATEUR.github.io/enquete-administrative/`

## 🏗️ Architecture

Application HTML unique (Single Page Application) sans dépendance serveur :

```
enquete-administrative/
├── index.html          # Application complète (HTML + CSS + JS)
├── README.md           # Documentation
├── LICENSE             # Licence MIT
└── .gitignore          # Fichiers ignorés par Git
```

### Technologies

- **HTML5 / CSS3 / JavaScript** (vanilla, aucun framework)
- **localStorage** pour la persistance et la sauvegarde automatique

## 📊 Les 9 étapes de l'enquête

| # | Étape | Obligatoire | Description |
|---|-------|:-----------:|-------------|
| 1 | **Contexte** | ✅ | Collectivité, date, objet, origine du signalement, urgence |
| 2 | **Personnes concernées** | ✅ | Identité, statut, fonction, notification, accusé de réception |
| 3 | **Chronologie des faits** | ✅ | Description générale + timeline détaillée (date, heure, lieu) |
| 4 | **Preuves** | — | Documents recueillis avec type, référence et valeur probante |
| 5 | **Auditions** | ✅ | Personnes auditionnées, qualité, synthèse des déclarations |
| 6 | **Témoins** | — | Témoignages avec évaluation de fiabilité |
| 7 | **Qualification juridique** | ✅ | Manquements identifiés, textes applicables, jurisprudence |
| 8 | **Analyse** | ✅ | Analyse juridique approfondie + notes privées |
| 9 | **Conclusions** | ✅ | Conclusions, recommandations, mesures disciplinaires |

## ⚖️ Manquements pré-définis

L'outil propose 20 qualifications juridiques courantes :

- Manquement à l'obligation de service, absence injustifiée, retard répété, insubordination
- Défaut de probité, conflit d'intérêts, prise illégale d'intérêt
- Harcèlement moral, harcèlement sexuel, discrimination
- Détournement de fonds publics, utilisation abusive de biens publics
- Manquement au devoir de neutralité / réserve
- Divulgation d'informations confidentielles, cumul irrégulier d'activités
- Et autres...

## 📄 Rapport généré

Le rapport d'enquête exporté comprend les sections suivantes :

1. Contexte de l'enquête
2. Personnes concernées
3. Chronologie des faits
4. Éléments de preuve recueillis
5. Auditions réalisées
6. Témoignages
7. Qualification juridique
8. Analyse juridique
9. Conclusions
10. Recommandations
11. Mesures disciplinaires (si applicable)

Le rapport est généré au format `.txt` avec un nommage automatique incluant le numéro d'enquête, la collectivité et la date.

## 🔒 Confidentialité

Toutes les données sont stockées **localement** dans le navigateur (localStorage). **Aucune donnée n'est envoyée à un serveur.** Cela garantit la confidentialité des informations sensibles relatives aux enquêtes administratives.

> ⚠️ **Important** : Pensez à exporter régulièrement vos données. Le localStorage peut être effacé par un nettoyage du navigateur.

## 👤 Auteur

**Louis MATHEVET-BIDINI**
- Président de l'AP2DFP (Association pour la Promotion et le Développement de la Déontologie dans la Fonction Publique)
- Secrétaire Général National de l'ARDT (Association des Référents Déontologues Territoriaux)
- Doctorant en droit public – Université de Lorraine

## 📄 Licence

Ce projet est distribué sous licence MIT. Voir le fichier [LICENSE](LICENSE) pour plus de détails.

## 🤝 Contribuer

Les contributions sont les bienvenues ! N'hésitez pas à :

1. Forker le projet
2. Créer une branche (`git checkout -b feature/amelioration`)
3. Commiter vos changements (`git commit -m 'Ajout d'une fonctionnalité'`)
4. Pousser la branche (`git push origin feature/amelioration`)
5. Ouvrir une Pull Request

## 📞 Contact

Pour toute question relative à l'utilisation de cet outil dans le cadre de vos enquêtes administratives internes, contactez l'AP2DFP.
