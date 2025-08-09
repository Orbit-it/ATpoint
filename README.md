# 📁 Structure du Projet ATpoint

```text
/biopointeuse-app
├── App.js                      # Point d'entrée principal de l'application
├── app.json                    # Configuration Expo (si utilisé)
├── package.json                # Dépendances et scripts NPM/Yarn
├── babel.config.js             # Configuration Babel (transpilation JS)
├── /assets                     
│   └── /sounds                 # Sons personnalisés (alertes, feedback vocal)
├── /components                 
│   ├── FaceCamera.js           # Composant caméra + détection faciale (TensorFlow.js)
│   ├── AdminPanel.js           # Interface admin sécurisée (PIN/biométrie)
│   ├── AddUserForm.js          # Formulaire d'enregistrement utilisateur
│   └── FeedbackModal.js        # Popup de confirmation/erreur
├── /screens                    
│   ├── KioskScreen.js          # Écran principal (mode kiosque plein écran)
│   ├── AdminScreen.js          # Dashboard admin (logs, export données)
│   ├── AddUserScreen.js        # Capture photo + saisie infos utilisateur
│   └── SettingsScreen.js       # Paramètres (API, réseau, calibration)
├── /utils                      
│   ├── faceRecognition.js      # Logique de reconnaissance faciale (FaceAPI/OpenCV)
│   ├── storage.js              # Gestion base SQLite (utilisateurs/pointages)
│   ├── speech.js               # TTS (Text-to-Speech pour feedback audio)
│   └── apiServer.js            # API REST locale pour synchronisation
├── /data                       
│   ├── users.db                # Base de données des employés (SQLite)
│   └── attendance.db           # Historique des pointages (SQLite)
└── /docs                       # Documentation supplémentaire (optionnel)
```

---

## 🛠 Fonctionnalités Clés par Dossier
| **Dossier**       | **Technologies/Modules**                     | **Rôle**                          |
|--------------------|---------------------------------------------|-----------------------------------|
| `components/`      | React Native, TensorFlow.js                 | UI modulaire réutilisable         |
| `screens/`         | React Navigation, Redux                     | Écrans principaux de l'application|
| `utils/`           | SQLite, Axios, Node.js (API embarquée)      | Logique métier et services        |
| `data/`            | SQLite (react-native-sqlite-storage)        | Persistance des données locales   |

---





