FROM nginx:alpine

# Instalar dependencias necesarias
RUN apk add --no-cache apache2-utils

# Crear directorio de datos
RUN mkdir -p /data /tmp/client_body_temp

# Copiar configuración personalizada
COPY nginx.conf /etc/nginx/nginx.conf
COPY htpasswd /etc/nginx/htpasswd
COPY index.html /data/index.html

# Dar permisos
RUN chmod 644 /etc/nginx/htpasswd

EXPOSE 8080

CMD ["nginx", "-g", "daemon off;"]

