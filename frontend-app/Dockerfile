# Utilisez une image de base légère Nginx
FROM nginx:alpine

# Supprimez la configuration Nginx par défaut
RUN rm /etc/nginx/conf.d/default.conf

# Copiez votre fichier de configuration Nginx personnalisé
COPY nginx.conf /etc/nginx/conf.d/

# Copiez les fichiers HTML du frontend dans le répertoire du serveur Nginx
COPY . /usr/share/nginx/html

# Exposez le port 80 pour le serveur Nginx
EXPOSE 80

# Commande pour démarrer le serveur Nginx
CMD ["nginx", "-g", "daemon off;"]


