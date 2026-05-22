# 📋 Dashboard Suivi Sorties Locataires

> Tableau de bord interactif pour le suivi des dossiers de sortie de locataires — import Excel mensuel, design liquid glass, 100% client-side.

---

## ✨ Fonctionnalités

- **Import Excel mensuel** — chargez votre fichier `.xlsx` de suivi chaque mois, les données s'accumulent automatiquement
- **Vue d'ensemble** — KPIs en temps réel : dossiers en cours, complétés, en retard, bientôt à échéance
- **Suivi par étapes** — 5 étapes par dossier (EDL · Comparatif · Devis · Compte départ · Restitution) cochables directement depuis le tableau de bord
- **Option NC (Non Concerné)** sur l'étape Devis — adapte automatiquement le délai de retard (1 mois si NC, 2 mois sinon)
- **Annotations** — annotez chaque étape sans la valider, avec affichage en bulle au survol
- **Statuts propriétaire** — indicateurs visuels 💰 En vente · ⚖️ Litige · 🔑 Congé affichés directement sur chaque carte
- **GLI Verlingue** — badge togglable sur chaque carte et dans le modal de détail ; affiche le logo Verlingue sur la carte quand activé
- **Alertes automatiques** — badge ⚠️ En retard et ⏰ Bientôt selon les délais calculés
- **Suppression manuelle** de dossiers
- **Sauvegarde / Restauration JSON** — exportez toutes vos données et restaurez-les sans perte
- **Recherche & filtres** — par locataire, propriétaire, ville, statut d'avancement
- **Navigation multi-mois** — historique complet mois par mois
- **Design Liquid Glass** inspiré d'Apple, responsive mobile / tablette / desktop
- **100% local** — aucun serveur, aucune installation, toutes les données stockées dans le navigateur (localStorage)

---

## 🚀 Utilisation

1. Ouvrir `index.html` dans un navigateur (Chrome, Edge, Safari, Firefox)
2. Cliquer sur **Importer un fichier Excel** et sélectionner votre fichier `.xlsx` mensuel
3. Naviguer entre les mois via le sélecteur en haut de page
4. Cliquer sur une carte pour ouvrir le détail et cocher les étapes

### Format du fichier Excel attendu

| Colonne | Contenu |
|---|---|
| Locataire | Nom du locataire |
| Propriétaire | Nom du propriétaire |
| Ville | Ville du bien |
| Date de sortie | Date au format `jj/mm/aaaa` |
| EDL reçu | Case cochée ou annotation |
| Comparatif | Case cochée ou annotation |
| Devis | Case cochée ou annotation |
| Compte départ | Case cochée ou annotation |
| Restitution | Case cochée ou annotation |

---

## 🛠️ Stack technique

- **Vanilla HTML / CSS / JavaScript** — aucune dépendance framework
- **[SheetJS (xlsx)](https://sheetjs.com/)** — lecture des fichiers Excel
- **[Chart.js](https://www.chartjs.org/)** — graphiques du tableau de bord
- **localStorage** — persistance des données côté client

---

## 📱 Compatibilité

| Navigateur | Support |
|---|---|
| Chrome / Edge | ✅ |
| Safari | ✅ |
| Firefox | ✅ |
| Mobile (iOS / Android) | ✅ |

---

## 📄 Licence

Usage personnel / interne.
