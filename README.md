# AventuraTime_mobile

STRUCTURE DU PROJET \n
/biopointeuse-app
├── App.js
├── app.json
├── package.json
├── babel.config.js
├── /assets
│   └── sounds/ (optionnel si tu veux fichiers audio au lieu de texte)
├── /components
│   ├── FaceCamera.js          # Caméra avec détection et reconnaissance faciale
│   ├── AdminPanel.js          # Accès sécurisé (PIN) pour configuration
│   ├── AddUserForm.js         # Formulaire pour ajouter un utilisateur
│   └── FeedbackModal.js       # Fenêtre pour les messages de retour
├── /screens
│   ├── KioskScreen.js         # Écran principal (caméra, reconnaissance)
│   ├── AdminScreen.js         # Menu des fonctions admin
│   ├── AddUserScreen.js       # Page ajout utilisateur (caméra + infos)
│   └── SettingsScreen.js      # Configuration API locale, test caméra, etc.
├── /utils
│   ├── faceRecognition.js     # Libs de détection + comparaison faciale
│   ├── storage.js             # SQLite / JSON handler
│   ├── speech.js              # Synthèse vocale
│   └── apiServer.js           # Serveur HTTP local embarqué
├── /data
│   ├── users.db               # Fichier SQLite ou users.json
│   └── attendance.db          # Pointages stockés localement

