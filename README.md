# 📚 Sting² - Bibliothèque de solutions

Bibliothèque collaborative de missions de référence pour Sting².

## 🎯 À propos

Cette bibliothèque contient des missions pré-configurées pour dimensionner rapidement vos offres dans Sting². Chaque mission est une combinaison de briques testée et validée pour des cas d'usage courants.

## 📂 Structure

```
sting-missions-library/
├── README.md
├── index.json                    # Catalogue des missions
└── missions/
    ├── logistique/
    │   ├── depot-chariot-standard.json
    │   └── ...
    ├── controles/
    │   ├── controle-qualite-pharma.json
    │   └── ...
    └── avant-prestation/
        ├── ouverture-mission.json
        └── ...
```

## 🚀 Utilisation

### Dans l'application Sting²

1. Cliquez sur le bouton **📚 Bibliothèque**
2. Parcourez les solutions disponibles
3. Cliquez sur **📥 Charger** pour importer une solution dans votre éditeur

### Configuration dans votre instance

Dans `main.js`, modifiez la constante `LIBRARY_REPO` :

```javascript
const LIBRARY_REPO = 'https://raw.githubusercontent.com/VOTRE-USERNAME/sting-missions-library/main';
```

## 🤝 Contribuer

### Méthode 1 : Via l'application (recommandé)

1. Créez votre mission dans Sting²
2. Cliquez sur **📚 Bibliothèque** → **💾 Sauvegarder ma solution**
3. Remplissez le formulaire (nom, description, catégorie)
4. Téléchargez les fichiers générés
5. Suivez les instructions pour créer une Pull Request

### Méthode 2 : Manuellement

1. Fork ce repository
2. Créez votre fichier JSON dans le bon dossier (`missions/categorie/`)
3. Ajoutez une entrée dans `index.json`
4. Créez une Pull Request

### Format d'une entrée dans index.json

```json
{
  "id": "categorie-nom-unique",
  "nom": "Nom de la solution",
  "description": "Description détaillée de ce que fait cette mission",
  "categorie": "logistique|controles|avant-prestation",
  "tags": ["tag1", "tag2"],
  "auteur": "Votre nom",
  "duree_estimee": "Xmin Ys",
  "nombre_briques": 3,
  "fichier": "missions/categorie/nom-fichier.json",
  "date_creation": "2026-01-17"
}
```

## 📋 Catégories disponibles

- **📦 Logistique** : Manutention, transport, dépôt
- **🔍 Contrôles** : Contrôle qualité, vérification, comptage
- **🚀 Avant la prestation** : Ouverture de mission, préparation

## 📄 Licence

Ces missions sont partagées librement pour usage interne La Poste.

## 💡 Support

Pour toute question, contactez l'équipe Sting² ou ouvrez une issue.

---

**Dernière mise à jour :** 17 janvier 2026  
**Nombre de missions :** 3  
**Contributeurs :** Équipe Sting²
