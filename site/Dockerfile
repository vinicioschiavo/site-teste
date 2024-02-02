# Use a imagem oficial do Apache
FROM httpd:2.4

# Copie o conteúdo do site para o diretório padrão do Apache
COPY ./site/ /usr/local/apache2/htdocs/

# Substitua a configuração padrão do Apache pela sua configuração personalizada
COPY ./apache-config/000-default.conf /usr/local/apache2/conf/extra/httpd-vhosts.conf