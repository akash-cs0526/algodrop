FROM openjdk:17
EXPOSE 8080
ADD target/products.jar products.jar
ENTRYPOINT {"java","-jar","/products.jar"}
