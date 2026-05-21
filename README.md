# 💪 Hell's Week - App de Suivi d'Entraînement Extrême

Une application mobile React Native pour suivre et tracker une semaine d'entraînement intense !

## 📱 Fonctionnalités

✅ **Suivi quotidien** - 7 jours d'entraînement différents
✅ **Sessions multiples** - Matin, midi, soir pour chaque jour
✅ **Exercices détaillés** - Séries, répétitions, temps de repos
✅ **Progression sauvegardée** - Automatiquement sur ton téléphone
✅ **Design brutal** - Interface sombre et motivante
✅ **Citations inspirantes** - Changent chaque 5 secondes

## 🚀 Installation et Démarrage

### Prérequis
- Node.js (v14+)
- npm ou yarn
- Expo CLI (`npm install -g expo-cli`)

### Étapes

1. **Clone le repo**
   ```bash
   git clone https://github.com/moussamelo28-collab/MELO.git
   cd MELO
   ```

2. **Installe les dépendances**
   ```bash
   npm install
   ```

3. **Lance l'app**
   - Pour iOS: `npm run ios`
   - Pour Android: `npm run android`
   - Pour tester sur le web: `npm run web`

4. **Utilise Expo Go** (Plus simple pour commencer)
   - Télécharge l'app "Expo Go" sur ton téléphone
   - Lance `npm start`
   - Scan le QR code avec ton téléphone

## 📂 Structure du Projet

```
MELO/
├── App.js                    # Point d'entrée principal
├── app.json                  # Configuration Expo
├── package.json              # Dépendances
├── src/
│   ├── screens/
│   │   └── HellsWeek.js     # Écran principal
│   └── data/
│       └── workoutData.js   # Données d'entraînement
└── README.md
```

## 🎯 Comment Utiliser

1. **Sélectionne un jour** - Clique sur LUNDI, MARDI, etc.
2. **Ouvre une session** - Tape sur une session pour voir les exercices
3. **Coche les exercices** - Appuie sur l'exercice pour le marquer comme fait ✓
4. **Regarde ta progression** - La barre PROG se remplit au fur et à mesure
5. **Réinitialise** - Bouton RESET pour recommencer

## 💾 Données Sauvegardées

Ton progrès est sauvegardé **automatiquement** sur ton téléphone via `AsyncStorage`. Pas besoin d'internet !

## 🛠️ Architecture React Native

- **useState** - Gère l'état de l'app (jour actif, exercices cochés, etc.)
- **useEffect** - Charge et sauvegarde les données
- **AsyncStorage** - Stockage local sur le téléphone
- **StyleSheet** - Styles pour React Native
- **Navigation** - (Préparé pour des écrans supplémentaires)

## 📝 Personnalisation

### Changer les couleurs d'un jour
Dans `src/data/workoutData.js`, modifie le `color` :
```javascript
{
  day: "LUNDI",
  theme: "JOUR DU FEU",
  color: "#FF2200",  // Change cette couleur
  // ...
}
```

### Ajouter/Modifier des exercices
Dans `src/data/workoutData.js`, ajoute dans le tableau `exercises` :
```javascript
{
  name: "Mon Exercice",
  sets: "5",
  reps: "10",
  rest: "60s"
}
```

## 🔧 Commandes Utiles

```bash
# Démarrer en développement
npm start

# Build pour iOS
npm run ios

# Build pour Android
npm run android

# Test sur le web (navigateur)
npm run web

# Nettoyer et réinstaller
rm -rf node_modules && npm install
```

## 📦 Dépendances Principales

- `react-native` - Framework mobile
- `expo` - Plateforme pour React Native
- `@react-navigation` - Navigation entre écrans
- `@react-native-async-storage/async-storage` - Stockage local

## ⚡ À Faire Prochainement

- [ ] Statistiques et graphiques
- [ ] Notifications de rappel
- [ ] Export PDF du plan
- [ ] Partage sur les réseaux
- [ ] Mode hors ligne amélioré
- [ ] Support des notifications push

## 💪 Motivation

> "PAIN IS WEAKNESS LEAVING THE BODY" — David Goggins

Bienvenue dans Hell's Week. Pas de jours off. Embrace the suck.

## 📄 License

MIT

---

**Créé avec ❤️ et beaucoup de souffrance** 🔥

Pour toute question ou contribution: [Ouvre une issue](https://github.com/moussamelo28-collab/MELO/issues)
