# CRUD API Back-end

## Initialisation du projet en local

Fonctionne principalement sous bash. (certaines commandes doivent être adaptées pour un environnement windows)

Dabord vous avez besoin de récupérer le projet via un clone du git ou via le zip envoyé par mail

https://github.com/ROMAIN

Installer python
_(sur windows bien penser à ajouter python dans le PATH et
à fermer et rouvrir votre shell pour interagir avec python nouvellement installé)_
 
https://www.python.org/downloads/

Installer pip :
```bash
curl https://bootstrap.pypa.io/get-pip.py -o get-pip.py
python get-pip.py
```

Installer virutalenv via pip 
```bash
pip install virtualenv
```

Creer votre environement virtuel via pip
```bash
cd chemin_du_repo/crud-api
python -m venv ../crud-api_env 
```

Démarer l'env virtuel
```bash
source ../crud-api_env/Scripts/activate
```

Installer les requirements
```bash
cd chemin_du_repo/crud_api
pip install -r requirements.txt
```

Lancer le calcul de la base de donnée
```bash
python manage.py db upgrade
```

Lancer l'API
```bash
python manage.py run
```

L'API est désormais accesible à cette adresse : http://127.0.0.1:5000/ 
