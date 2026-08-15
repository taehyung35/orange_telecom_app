# Orange Telecom App (démo)

Application Flutter simple inspirée de l'app Orange Telecom : forfait, consommation (data/appels), facture, profil. Pas de backend réel — les données sont simulées (mock) après le login.

## Écrans
- **Login** : validation numéro de téléphone (format `06XXXXXXXX` / `07XXXXXXXX`) + mot de passe
- **Accueil** : carte forfait, consommation internet/appels avec barres de progression, facture en cours, actions rapides
- **Profil** : infos client, menu, déconnexion

## Lancer le projet

```bash
flutter pub get
flutter run
```

## Structure

```
lib/
  main.dart
  theme/app_theme.dart        # couleurs & thème Orange
  models/user_model.dart      # modèle utilisateur + données mock
  screens/
    login_screen.dart
    home_shell.dart           # bottom navigation
    home_screen.dart
    profile_screen.dart
  widgets/usage_card.dart     # carte réutilisable data/appels
```

## Mettre sur Git

```bash
cd orange_telecom_app
git init
git add .
git commit -m "Init: Orange Telecom app simple (Flutter)"
git branch -M main
git remote add origin <URL_DYAL_REPO_DYALK>
git push -u origin main
```

## À faire après (optionnel)
- Brancher un vrai backend (API REST / Firebase) au lieu du mock
- Ajouter `flutter_secure_storage` pour sauvegarder la session
- Ajouter des tests (`flutter test`)
