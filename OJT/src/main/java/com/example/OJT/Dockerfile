From maven:3-eclipse-temurin-17 As build 
copy--
Run mvn clean package -DskipTests
From eclipse-temurin:17-alpine
copy--from=build/target/*.jar demo.jar
Expose 8080
ENTRY POINT["Java","-jar","demo.jar"]