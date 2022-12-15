FROM bitnami/java
COPY app/PingPong.java /opt
WORKDIR /opt
CMD ["javac", "PingPong.java"]
CMD ["java", "PingPong.java"]
EXPOSE 8080
