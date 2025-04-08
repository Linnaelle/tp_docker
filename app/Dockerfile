# Utiliser une image de base Python
FROM python:3.9-slim

# Définir le répertoire de travail
WORKDIR "C:\\Users\\Clem\\Desktop\\Cours\\Docker et Kubernetes\\app"

# Copier les fichiers requirements.txt dans le conteneur
COPY requirements.txt requirements.txt

# Installer les dépendances Python
RUN pip install -r requirements.txt

# Copier le reste des fichiers de l'application dans le conteneur
COPY . .

# Indiquer le port sur lequel l'application va tourner 
EXPOSE 5000

# Commande pour exécuter l'application
CMD ["python", "app.py"]