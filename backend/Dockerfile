# Étape 1 : choisir une image Node légère
FROM node:18-alpine

# Étape 2 : définir le répertoire de travail
WORKDIR /app

# Étape 3 : copier les fichiers de dépendances
COPY package*.json ./

# Étape 4 : installer les dépendances
RUN npm install --production

# Étape 5 : copier le reste du code
COPY . .

# Étape 6 : documenter le port utilisé
EXPOSE 5000

# Étape 7 : lancer l'application
CMD ["npm", "start"]
