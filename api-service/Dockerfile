# Usar imagen base ligera de Node
FROM node:18-alpine

# Crear directorio de trabajo
WORKDIR /app

# Copiar package.json y package-lock (si existe) e instalar dependencias
COPY package*.json ./
RUN npm install --production

# Copiar el resto del código
COPY . .

# Exponer puerto (coincide con PORT en server.js)
EXPOSE 3000

# Arrancar la aplicación
CMD ["npm", "start"]
