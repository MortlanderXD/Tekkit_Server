# Tekkit Server 3.21 / Minecraft 1.25

# 🎮 Comment lancer ton serveur Tekkit ???

## Salut toi ! 👋

Tu veux jouer à **Tekkit** avec tes amis sur ton propre serveur ? Trop cool ! 😎  
Voici un petit guide super simple pour t'aider à tout lancer tout seul comme un pro. 🧑‍💻

---

## 🧰 Ce qu'il te faut :

1. **Une vieille version de Java** (Java 7 exactement)
   - Le fichier est ici :  
     `C:\Program Files\Java\jdk1.7.0_80\bin\java.exe`

2. **Le fichier de Tekkit** (il s'appelle `Tekkit.jar`)
   - Mets-le dans un dossier que tu connais, par exemple sur ton **Bureau**.

3. **Un terminal Windows** (on va t’expliquer 👇)

---

## 🧑‍🚀 Étape par étape

### 1. Ouvre ton terminal
- Clique sur le bouton **Démarrer** 🔍
- Tape **PowerShell**
- Clique **droit** dessus et choisis **"Exécuter en tant qu'administrateur"**
  > C'est super important ! Sinon ton serveur ne pourra pas ouvrir les ports nécessaires pour que tes amis se connectent.

---

### 2. Va dans le dossier où tu as mis Tekkit
Par exemple, si tu l’as mis sur ton **Bureau**, tape :

```powershell
cd "$env:USERPROFILE\Desktop"
```

👉 Appuie sur Entrée

### 3. Lance le serveur avec la vieille version de Java

Maintenant, tape cette commande magique :
```powershell
& 'C:\Program Files\Java\jdk1.7.0_80\bin\java.exe' -jar .\Tekkit.jar
```
👉 Appuie encore sur Entrée

💥 BOOM ! Le serveur démarre ! Tu vas voir plein de lignes qui bougent, c’est normal. C’est le serveur qui se réveille !

