# Utilisez une image de base légère Python
FROM python:3.8-slim

# Répertoire de travail à l'intérieur du conteneur
WORKDIR /app

# Copiez le fichier de dépendances dans le conteneur
COPY requirements.txt .

# Installez les dépendances Python
RUN pip install --no-cache-dir -r requirements.txt

# Copiez le reste des fichiers dans le conteneur
COPY . .

# Commande pour démarrer le serveur
CMD ["python", "app.py"]