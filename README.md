# TAF-1-INF222-EC1-D-veloppement-Backend-Programmation-Web
Develloement d'une api de geation d'article

# API Backend de geation d'article

## Technologies Utilisées
- **Python** : Langage serveur
- **Django** : Framework d'application web
- **SQLite3** : Base de données 
- **Swagger** : Documentation de l'API

## Prérequis
- version recente de python
- creer un repertoire et decompresser le fichier gestion_article
- dans le meme repertiore mettre le fichier requirement
- ouvrir le repertoire creer dans le terminal

## Installation et Lancement

1. **Creer un environnement virtuel** :
```bash
python -m venv venv
```

2. **Activer l'environnement et les installation necessaires** :
```bash
source venv/bin/activate
```
```bash
sudo apt update
sudo apt install python3-pip
```
```bash
pip install -r requirements.txt
```



3. **LANCEMENT DU SERVEUR** :
- `une foi activer vous verez (venv) dans le terminal `
- `Se positioner dans le dossier gestion_article dans le terminal et lancer la commande'python manage.py runserver'`
- `Aller dans votre mavigateur et taper http://localhost:8000/api/accueil/ pour realiser differentes operations`



### Endpoints Principaux

- `POST /api/articles` : Créer un article (Titre, contenu, auteur, date, tag et catégorie requis)
- `GET /api/articles` : Afficher tous les articles 
- `GET /api/articles/{id}` : Lire un article
- `PUT /api/articles/{id}` : Mettre à jour un article
- `DELETE /api/articles/{id}` : Supprimer un article
- `GET /api/articles/search?query=texte` : Chercher un "texte" dans le titre et/ou le contenu des articles

## Architecture

gestion_article/
├── api/                       
│   ├── migrations/           
│   ├── templates/
│   │   └── api/                
│   │       ├── base.html       
│   │       ├── create.html
│   │       ├── delete.html
│   │       ├── read_a.html
│   │       ├── read.html
│   │       └── search.html     
│   ├── __init__.py
│   ├── admin.py                
│   ├── apps.py
│   ├── forms.py         
│   ├── models.py               
│   ├── tests.py
│   ├── urls.py             
│   └── views.py      
├── gestion_article/  
│   ├── __init__.py
│   ├── asgi.py
│   ├── settings.py           
│   ├── urls.py              
│   └── wsgi.py
├── templates/            
├── db.sqlite3           
└── manage.py                   
