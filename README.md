# 📊 Projet Comptabilité

![Statut du projet](https://img.shields.io/badge/Statut-En_D%C3%A9veloppement-yellow)
![Version](https://img.shields.io/badge/Version-1.0.0-blue)
![Auteur](https://img.shields.io/badge/Auteur-Nelly_DOUCET-orange)

Bienvenue dans le dépôt officiel du projet **Comptabilité**. 
Ce référentiel centralise les outils, les modèles et la documentation nécessaires à la gestion et à l'automatisation comptable.

---

## 👩‍💼 Autrice

Ce projet est conçu, développé et maintenu par :

*   **Nelly DOUCET** - *Créatrice et Responsable Comptable*

> Pour toute question ou suggestion, n'hésitez pas à ouvrir une *Issue* sur ce dépôt.

---

## 📑 Table des matières

1.  [À propos du projet](#-à-propos-du-projet)
2.  [Statut d'avancement](#-statut-davancement)
3.  [Structure du dépôt](#-structure-du-dépôt)
4.  [Technologies utilisées](#-technologies-utilisées)
5.  [Exemple d'utilisation](#-exemple-dutilisation)
6.  [Installation](#-installation)
7.  [Licence](#-licence)

---

## 🎯 À propos du projet

L'objectif de ce dépôt est de fournir une base solide pour :
*   La gestion des factures clients et fournisseurs.
*   L'automatisation des rapprochements bancaires.
*   La génération de rapports financiers (Bilan, Compte de résultat).
*   Le calcul automatique de la TVA.

## 🚦 Statut d'avancement

Voici l'état actuel des fonctionnalités du projet :

- [x] Création du référentiel et de la documentation
- [x] Modèles de factures (Excel et PDF)
- [x] Script de calcul de TVA
- [ ] Automatisation des rapprochements bancaires
- [ ] Tableau de bord interactif (Power BI / Looker)
- [ ] Génération automatique des déclarations fiscales

## 📂 Structure du dépôt

| Dossier | Description | Statut |
| :--- | :--- | :---: |
| `/docs` | Documentation comptable et procédures internes | 🟢 Terminé |
| `/modeles` | Modèles de factures, devis et relevés | 🟢 Terminé |
| `/scripts` | Scripts Python et macros VBA d'automatisation | 🟡 En cours |
| `/rapports` | Exemples de rapports générés | 🔴 À faire |

## 🛠️ Technologies utilisées

Ce projet utilise une combinaison d'outils bureautiques et de programmation :

*   **Excel / VBA** : Pour les modèles et macros de base.
*   **Python** : Pour l'automatisation des calculs et le traitement des données.
*   **Markdown** : Pour toute la documentation.

## 💻 Exemple d'utilisation

Voici un exemple de script Python utilisé pour calculer la TVA à partir d'un montant HT :

```python
# Calcul de la TVA (Taux à 20%)
def calculer_ttc(montant_ht, taux_tva=0.20):
    """
    Retourne le montant TTC et le montant de la TVA.
    """
    montant_tva = montant_ht * taux_tva
    montant_ttc = montant_ht + montant_tva
    return montant_ttc, montant_tva

# Exemple d'appel
prix_ht = 1000
ttc, tva = calculer_ttc(prix_ht)

print(f"Prix HT : {prix_ht}€")
print(f"TVA (20%) : {tva}€")
print(f"Prix TTC : {ttc}€")
