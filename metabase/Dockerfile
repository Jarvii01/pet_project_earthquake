#FROM openjdk:20-jdk

FROM eclipse-temurin:17-jdk-jammy

ENV MB_PLUGINS_DIR=/home/plugins/

#ADD https://downloads.metabase.com/v0.52.13/metabase.jar /home
COPY metabase.jar /home/metabase.jar

COPY metabase.jar /home/metabase.jar
ADD https://github.com/MotherDuck-Open-Source/metabase_duckdb_driver/releases/download/0.2.12-b/duckdb.metabase-driver.jar /home/plugins/

RUN chmod 744 /home/plugins/duckdb.metabase-driver.jar

CMD ["java", "-jar", "/home/metabase.jar"]









#FROM eclipse-temurin:17-jdk-jammy
#
#ENV MB_PLUGINS_DIR=/home/plugins/
#
#ADD https://downloads.metabase.com/v0.57.5/metabase.jar /app
#ADD https://github.com/MotherDuck-Open-Source/metabase_duckdb_driver/releases/download/0.2.12-b/duckdb.metabase-driver.jar /app/plugins/
#
#RUN chmod 744 /home/plugins/duckdb.metabase-driver.jar
#
#CMD ["java", "-jar", "/app/metabase.jar"]
