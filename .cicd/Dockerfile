# Need to create a Dockerfile for java based applications
# Dockerfile for Eureka

FROM openjdk:18.0.2.1-jdk
ARG JAR_SOURCE
ENV JAR_SOURCE ${JAR_SOURCE}
ARG JAR_DEST
ENV JAR_DEST ${JAR_DEST}
RUN mkdir -p /opt/i27/
WORKDIR /opt/i27/
COPY ["${JAR_SOURCE}", "/opt/i27/i27cart-user.jar"]
RUN chmod 777 /opt/i27/
EXPOSE 8232
CMD ["java", "-jar", "/opt/i27/i27cart-user.jar"]