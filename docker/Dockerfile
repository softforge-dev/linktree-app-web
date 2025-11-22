# Usando a imagem estável do Nginx
FROM nginx:alpine

# Remove configs padrão (opcional, mas deixa limpo)
RUN rm -rf /usr/share/nginx/html/*

# Copia os arquivos do seu site estático para o diretório padrão do Nginx
COPY ./src /usr/share/nginx/html

# Expondo porta tradicional do HTTP
EXPOSE 80

# Inicia o Nginx no modo foreground tradicional
CMD ["nginx", "-g", "daemon off;"]
