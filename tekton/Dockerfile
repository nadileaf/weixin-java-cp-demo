FROM cr.mesoor.com/dev-dependencies/openjdk:11-alpine-slim
WORKDIR /app
COPY target/weixin-java-cp-demo-1.0.0.jar app.jar
#COPY conf conf
EXPOSE 8080
CMD ["java", "-jar", "-Xms256m", "-XX:MaxRAMPercentage=75.0", "-Duser.timezone=GMT+8", "app.jar","application.env=prod"]
