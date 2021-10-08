## Dockerfile

Container usando Dockerfile para distribuição de uma aplicação Java.

Entrar no diretório onde se encontra o arquivo Dockerfile e criar uma imagem:

<pre>
docker build -t javapp .
</pre>

Listar as imagens:

<pre>
docker images
</pre>

Executar o container:

<pre>
docker run -p 8080:8080 javapp
</pre>
