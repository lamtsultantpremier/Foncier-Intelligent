## Documentation de l'application

L'application Agent Conversationnel dédié au foncier a trois partie.
Une Interface utilisateur, une logique et une API pour communiquer avec le Modele GPT 4o d'OPENAI

### I-Instruction Général
1- Avoir une une instance de POSTGRESQL sur sa machine
  1- Démarer POSTGRESQL
  1.1 Créer une machine virtuelle pour éviter les conflits de dépendance
     python -m venv venv
2- Activer l'environnement
    2.1 Sur windows ./venv/Scripts/activate
    2.2 sur linux source venv/bin/activate
  3- Cloner le Repository
    3.1 git clone https://github.com/lamtsultantpremier/Foncier-Intelligent.git

    3.2  Installer les dépendances de chaque partie de l'application (Front,Back,API LLM) contenu dans le fichier requirements.txt
    3.3  En fonction de l'éditeur de code  utilisé ouvrir chaque partie du programme dans une fenêtre de l'éditeur.
   
### - Le Front-End (dans un nouvelle instance de l'éditeur)
1- Se déplacer dans le frontend 
  1.1 -cd frontend
  1.2 installer les dépendances:   python install -r requirements.txt

2- Lancer l'application
  2.1 streamlit run main.py

## Le backend (dans un nouvelle instance de l'éditeur)
1- Se déplacer dans le backend 
1.1  cd backend
1.2  installer les dépendances:   python install -r requirements.txt

2-  Lancer une instance du backend
2.1 uvicorn main:app --reload

## L'API LLM (dans un nouvelle instance de l'éditeur)
1- Se déplacer dans l'API LLM
  1.1 cd api_llm
  1.2 installer les dépendances:   python install -r requirements.txt

2- Lancer une API LLM
  2.1 uvicorn main:app --reload --port 8001

