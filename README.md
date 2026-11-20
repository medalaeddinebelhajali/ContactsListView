# ContactsListView

Une application Android simple développée en Kotlin permettant d'afficher, sélectionner et modifier une liste de contacts.

## 📱 Fonctionnalités

- **Affichage de la liste des contacts** : Utilisation d'une `ListView` avec un `ArrayAdapter` pour présenter la liste initiale.
- **Sélection d'un contact** : Un clic sur un contact l'active visuellement et remplit automatiquement le champ de saisie (`EditText`).
- **Modification d'un contact** : Mise à jour du nom du contact sélectionné via le bouton **Modifier** ou la touche de validation du clavier (**IME Done**).
- **Validation des données** :
  - Vérification qu'un contact est sélectionné avant toute modification.
  - Alerte si le champ du nouveau nom est vide.
  - Notifications par `Toast` et messages d'erreur explicites.

## 🛠️ Technologies & Configuration

- **Langage** : Kotlin
- **Compile SDK** : 35
- **Min SDK** : 24 (Android 7.0)
- **Target SDK** : 35
- **Interface Utilisateur** : Material Components, `AppCompatActivity`, `ListView`, `EditText`, `Button`
- **Build System** : Gradle (Version Catalog `libs.versions.toml` & Kotlin DSL)

## 📁 Structure du Projet

```text
ContactsListView/
├── app/
│   ├── src/
│   │   └── main/
│   │       ├── java/com/example/contactslistview/
│   │       │   └── MainActivity.kt        # Logique principale de l'application
│   │       ├── res/
│   │       │   ├── layout/
│   │       │   │   └── activity_main.xml  # Layout XML principal
│   │       │   └── values/
│   │       │       ├── strings.xml        # Ressources textuelles
│   │       │       └── themes.xml         # Thème Material 3
│   │       └── AndroidManifest.xml
│   └── build.gradle.kts                   # Configuration du module app
├── gradle/
│   └── libs.versions.toml                 # Catalog des versions et dépendances
├── build.gradle.kts                       # Configuration Gradle racine
└── README.md
```

## 🚀 Compilation & Exécution

### Prérequis

- **Android Studio** (version Jellyfish ou ultérieure recommandée)
- **JDK 17**
- Un émulateur Android ou un appareil physique (Android 7.0 / API 24 minimum)

### Étapes

1. Ouvrez le projet dans **Android Studio**.
2. Synchronisez Gradle (*Sync Project with Gradle Files*).
3. Lancez la compilation et l'exécution :
   ```bash
   ./gradlew assembleDebug
   ```
4. Sélectionnez votre appareil/émulateur et cliquez sur **Run** (`Shift + F10`).

## 🧪 Tests

Pour exécuter les tests unitaires :
```bash
./gradlew test
```
