# Usar a imagem base do Nginx
FROM nginx:alpine

# Copiar o arquivo de configuração do Nginx
COPY nginx.conf /etc/nginx/nginx.conf

# Copiar os arquivos do site para o diretório padrão do Nginx
COPY index.html /usr/share/nginx/html/

# Copiar os certificados SSL
COPY ssl/selfsigned.crt /etc/ssl/certs/cert.pem
COPY ssl/selfsigned.key /etc/ssl/private/key.pem

# Expôr as portas 80 e 443 para HTTP e HTTPS
EXPOSE 80 443
