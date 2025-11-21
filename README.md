# 🎵 Speech Emotion Recognition (SER)
### 🔊 Détection des émotions dans la voix avec RAVDESS + EmoDB + ResNet50

Ce projet implémente un système complet de **reconnaissance des émotions à partir de fichiers audio**, utilisant :

✔ RAVDESS et EmoDB  
✔ Extraction de mél-spectrogrammes  
✔ Vision par ordinateur avec ResNet50 (transfer learning)  
✔ Entraînement, validation, visualisation, prédictions  
✔ Sauvegarde & chargement du modèle final  

---

## 📌 Objectifs

- Combiner deux datasets audio (RAVDESS + EmoDB)  
- Extraire les features audio (mel-spectrogrammes)  
- Convertir les audios en images pour ResNet50  
- Entraîner un modèle Deep Learning robuste  
- Évaluer les performances sur validation  
- Prédire l’émotion d’un fichier audio externe  
- Sauvegarder le modèle + LabelEncoder  

---

## 📂 Structure du projet

```
📁 SpeechEmotionRecognition
 ├── RAVDESS/                   
 ├── EmoDB/                    
 ├── savefinal/
 │    ├── emotion_model.h5      
 │    ├── label_encoder.joblib  
 ├── emotional_speech_dataset2.csv  
 ├── nouvlab.ipynb              
 ├── README.md
 └── test/
      └── sad.wav               
```

---

## 🗂️ Datasets utilisés

### 🎙️ RAVDESS
- Audios émotionnels d'acteurs  
- Étiquettes extraites via le nom du fichier  
- Emotions utilisées : neutral, happy, sad, anger, fear, disgust  

### 🎤 EmoDB
- Corpus allemand  
- Étiquettes extraites via le 5ᵉ caractère du nom du fichier  
- Emotions utilisées : anger, disgust, fear, happy, sad, neutral  

---

## 🔧 Prétraitement des données

### 1. Calcul des durées
### 2. Extraction des mél-spectrogrammes
### 3. Conversion des spectrogrammes en images pour ResNet50

---

## 🧠 Modélisation – ResNet50
- Transfer learning  
- GlobalAveragePooling2D  
- Dense + Dropout  
- Softmax final  

---

## 📈 Évaluation
- Classification Report  
- Matrice de confusion  

---

## 🔍 Prédiction sur un fichier audio

---

## 💾 Sauvegarde & chargement
- emotion_model.h5  
- label_encoder.joblib  

---

## 🔮 Améliorations possibles
- Ajouter d’autres classes  
- Tester EfficientNet  
- API Flask / FastAPI  
- Version mobile  

---

## 🧑‍💻 Auteur
**Hamza NASR**
