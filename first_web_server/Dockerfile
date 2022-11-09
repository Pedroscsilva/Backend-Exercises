FROM httpd:2.4
# COPY copia um arquivo do computador e coloca ele dentro da imagem, no caminho especificado à frente.
COPY index.html /usr/local/apache2/htdocs/
# EXPOSE indica que a imagem poderá receber conexões pelo número da porta informado. Aqui a imagem poderá receber conexões na porta 80, padrão do httpd.
EXPOSE 80
CMD ["httpd-foreground"]
# um docker build -t <name> <context> agora faz a imagem.
# para executar a imagem, use docker run --rm -d -p 1234:80 --name meu-container meu-servidor
# a flag -p indica a porta
# se entrar no localhost:1234 você irá ser redirecionado para o html passado. Massa demais...