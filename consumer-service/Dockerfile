# Imagen base ligera con Java 17
FROM eclipse-temurin:17-jre-jammy

# Argumento del JAR que será copiado
ARG JAR_FILE=target/*.jar

# Directorio de trabajo
WORKDIR /app

# Copiar el archivo JAR al contenedor
COPY ${JAR_FILE} app.jar

# Comando para ejecutar la aplicación
ENTRYPOINT ["java", "-jar", "app.jar"]
