## Documentation de l'application

L'application Agent Conversationnel dédié au foncier a trois partie.
Une Interface utilisateur, une logique et une API pour communiquer avec le Modele GPT 4o d'OPENAI

### I-Instruction Général
-- Avoir une une instance de POSTGRESQL sur sa machine
-- Démarer POSTGRESQL
-- Créer une machine virtuelle pour éviter les conflits de dépendance
    python -m venv venv
-- Activer l'environnement
    Sur windows ./venv/Scripts/activate
    sur linux source venv/bin/activate
-- Cloner le Repository
git clone https://github.com/lamtsultantpremier/Foncier-Intelligent.git

-- Installer les dépendances de chaque partie de l'application (Front,Back,API LLM) contenu dans le fichier requirements.txt
-- En fonction de l'éditeur de code  utilisé ouvrir chaque partie du programme dans une fenêtre de l'éditeur.
   
### - Le Front-End (dans un nouvelle instance de l'éditeur)
1- Se déplacer dans le frontend 
-cd frontend
installer les dépendances:   python install -r requirements.txt

2- Lancer l'application
streamlit run main.py

## Le backend (dans un nouvelle instance de l'éditeur)
1- Se déplacer dans le backend 
-cd backend
installer les dépendances:   python install -r requirements.txt

2- Lancer une instance du backend
uvicorn main:app --reload

## L'API LLM (dans un nouvelle instance de l'éditeur)
1- Se déplacer dans l'API LLM
-cd api_llm
installer les dépendances:   python install -r requirements.txt

2- Lancer une API LLM

uvicorn main:app --reload --port 8001

