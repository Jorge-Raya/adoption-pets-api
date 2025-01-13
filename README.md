# adoption-pets-api
API - Rest para adocion de Mascotas

spring.autoconfigure.exclude=org.springframework.boot.autoconfigure.jdbc.DataSourceAutoConfiguration


< settings xmlns="http://maven.apache.org/SETTINGS/1.0.0"
          xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
          xsi:schemaLocation="http://maven.apache.org/SETTINGS/1.0.0 https://maven.apache.org/xsd/settings-1.0.0.xsd">
    <localRepository>${user.home}/.m2/repository</localRepository>
    <interactiveMode>true</interactiveMode>
    <offline>false</offline>

    < mirrors>
        <mirror>
            <id>central</id>
            <mirrorOf>central</mirrorOf>
            <url>https://repo.maven.apache.org/maven2</url>
        </mirror>
    </mirrors>

    < proxies>
        <!-- Configura esto si estás detrás de un proxy -->
        <!--
        <proxy>
            <id>example-proxy</id>
            <active>true</active>
            <protocol>http</protocol>
            <host>proxy.example.com</host>
            <port>8080</port>
            <username>usuario</username>
            <password>contraseña</password>
            <nonProxyHosts>www.google.com|*.example.com</nonProxyHosts>
        </proxy >
        -->
    </proxies>
</setting s>

command to avoid the DB setup
* spring.autoconfigure.exclude=org.springframework.boot.autoconfigure.jdbc.DataSourceAutoConfiguration

pass for Supabase

 Db: ju66ErnauT0verwhelming7orce



-----aplication properties
spring.application.name=adoption-pets-api

#Configuracion de la Base de Datos
spring.datasource.url=jdbc:postgresql://aws-0-us-west-1.pooler.supabase.com:5432/postgres
spring.datasource.username=postgres.liliwvitbtpcmjesirpw
spring.datasource.password=${PG_SUPABASE_PASSWORD}
spring.datasource.driver-class-name=org.postgresql.Driver

# Configuracion de JPA
spring.jpa.hibernate.ddl-auto=update
spring.jpa.properties.hibernate.dialect=org.hibernate.dialect.PostgreSQLDialect
spring.jpa.show-sql=true
spring.jpa.properties.hibernate.format_sql=true

logging.level.org.hibernate.SQL=DEBUG
logging.level.org.hibernate.type.descriptor.sql=TRACE



