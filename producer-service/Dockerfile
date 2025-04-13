# Imagen base con Java JDK
FROM openjdk:17-jdk-slim

# Argumento que usaremos para copiar el .jar
ARG JAR_FILE=target/*.jar

# Directorio de trabajo en el contenedor
WORKDIR /app

# Copiar el archivo JAR al contenedor
COPY ${JAR_FILE} app.jar

# Exponer el puerto del servicio
EXPOSE 8080

# Comando para ejecutar la app
ENTRYPOINT ["java", "-jar", "app.jar"]
