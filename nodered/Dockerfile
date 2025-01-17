# Usar la imagen base oficial de Node-RED
FROM nodered/node-red:latest

# Establecer el directorio de trabajo
WORKDIR /usr/src/node-red

# Copiar los certificados a la carpeta `/data/certs/` dentro del contenedor
COPY certs/ /data/certs/

# Copiar el archivo settings.js al directorio de configuración de Node-RED
COPY settings.js /data/settings.js

# Exponer los puertos para HTTP y HTTPS
EXPOSE 1880 8443

# Comando para iniciar Node-RED
CMD ["npm", "start", "--", "--userDir", "/data"]
