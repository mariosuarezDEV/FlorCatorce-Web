# Etapa 1: Construcción de la aplicación (si necesitas construir dentro del contenedor)
# FROM node:lts-alpine as builder
# WORKDIR /app
# COPY package*.json ./
# RUN npm ci
# COPY . .
# RUN npm run build

# Etapa 2: Servidor de producción
FROM nginx:stable-alpine

# Eliminar configuración por defecto de Nginx
RUN rm -rf /etc/nginx/conf.d/*

# Copiar configuración personalizada
COPY nginx.conf /etc/nginx/conf.d/

# Copiar archivos construidos de Vue
COPY dist /usr/share/nginx/html

# Exponer puerto 80
EXPOSE 80

# Iniciar Nginx en primer plano
CMD ["nginx", "-g", "daemon off;"]