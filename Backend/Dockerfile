# Usar una imagen base de Node.js
FROM node:20

# Establecer el directorio de trabajo dentro del contenedor
WORKDIR /usr/src/app

# Copiar package.json y package-lock.json al contenedor
COPY package*.json ./

# Instalar dependencias
RUN npm install

# Copiar el resto de los archivos al contenedor
COPY . .

# Exponer el puerto en el que tu aplicación se ejecuta
EXPOSE 22174

# Comando para iniciar la aplicación
CMD ["npm", "run", "dev"]