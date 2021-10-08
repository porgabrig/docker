# Especifica a imagem de origem
FROM ubuntu

# Instala os pacotes
RUN apt-get update && \
	apt-get install -y default-jre && \
	apt-get install -y openjdk-17-jre-headless && \
	apt-get clean;

# Copia o arquivo jar
COPY ./application.jar start.jar

# Expõe a porta da aplicação
EXPOSE 8080

# Comando que será executado quando o container for iniciado
ENTRYPOINT ["java", "-jar", "start.jar"]