## Documentation de l'application

L'application **Agent Conversationnel** dédié au foncier comporte trois parties :
- **Interface utilisateur**  
- **Logique métier**  
- **API** pour communiquer avec le modèle GPT-4o d'OpenAI

---
### I – Instructions Générales

1. **Avoir une instance de PostgreSQL sur sa machine**
   1. Démarrer PostgreSQL
   2. Créer une machine virtuelle pour éviter les conflits de dépendances :
      ```bash
      python -m venv venv
      ```
    
2. **Activer l'environnement**
   - Sur Windows :
     ```bash
     ./venv/Scripts/activate
     ```
   - Sur Linux :
     ```bash
     source venv/bin/activate
     ```

3. **Cloner le dépôt**
   ```bash
   git clone https://github.com/lamtsultantpremier/Foncier-Intelligent.git

1- Installer les dépendances de chaque partie de l'application (Front, Back, API LLM) présentes dans leurs fichiers requirements.txt.

2- En fonction de l'éditeur de code utilisé, ouvrir chaque partie du programme dans une fenêtre distincte.

### II – Front-End (dans une nouvelle instance de l'éditeur)

1. Se déplacer dans le dossier frontend :
cd frontend
. Installer les dépendances :
```bash
pip install -r requirements.txt
```

2. Lancer l'application :
streamlit run main.py

### III – Backend (dans une nouvelle instance de l'éditeur)
1. Se déplacer dans le dossier backend :

cd backend

. Installer les dépendances :
```bash
pip install -r requirements.txt
```
2. Lancer le backend :

```bash
uvicorn main:app --reload
```
### IV – API LLM (dans une nouvelle instance de l'éditeur)

1. Se déplacer dans le dossier api_llm :

cd api_llm

. Installer les dépendances :
```bash
pip install -r requirements.txt
```

2. Lancer l’API LLM :
```bash
uvicorn main:app --reload --port 8001
```
