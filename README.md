# Домашнее задание к занятию 9 «Процессы CI/CD»
## Знакомоство с SonarQube

```bash
user@study:~/home_work/cicd/ci-03-cicd/example$ sonar-scanner \
  -Dsonar.projectKey=cicd03 \
  -Dsonar.sources=. \
  -Dsonar.host.url=http://158.160.155.139:9000 \
  -Dsonar.login=23dc5320d6daafcbbe79a862e85e90cd44cc7290 \
> -Dsonar.coverage.exclusions=fail.py
INFO: Scanner configuration file: /home/user/sonar-scanner-5.0.1.3006-linux/conf/sonar-scanner.properties
...
INFO: ------------------------------------------------------------------------
INFO: EXECUTION SUCCESS
INFO: ------------------------------------------------------------------------
INFO: Total time: 1:13.304s
INFO: Final Memory: 8M/34M
INFO: ------------------------------------------------------------------------
```
![image](https://github.com/suntsovvv/ci-03-cicd/assets/154943765/0c76681b-fba6-49ea-aeef-3e8612b0b0c2)
![image](https://github.com/suntsovvv/ci-03-cicd/assets/154943765/8f55ec47-69a9-4b6f-95b9-0a6a7d5c0b9d)

## Знакомство с Nexus   
![image](https://github.com/suntsovvv/ci-03-cicd/assets/154943765/f4fd0ab3-15b6-4b15-a576-a8da9d2164fe)

https://github.com/suntsovvv/ci-03-cicd/blob/main/maven-metadata.xml   

## Знакомство с Maven   
```bash
[WARNING] JAR will be empty - no content was marked for inclusion!
[INFO] Building jar: /home/user/home_work/cicd/ci-03-cicd/mvn/target/simple-app-1.0-SNAPSHOT.jar
[INFO] ------------------------------------------------------------------------
[INFO] BUILD SUCCESS
[INFO] ------------------------------------------------------------------------
[INFO] Total time:  18.008 s
[INFO] Finished at: 2024-03-28T07:07:21Z
[INFO] ------------------------------------------------------------------------
```
```bash
user@study:~/.m2/repository/netology/java/8_282$ ls
java-8_282-distrib.jar  java-8_282-distrib.jar.sha1  java-8_282.pom.lastUpdated  _remote.repositories
```
pom.xml :   
```xml
<project xmlns="http://maven.apache.org/POM/4.0.0" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
  xsi:schemaLocation="http://maven.apache.org/POM/4.0.0 http://maven.apache.org/xsd/maven-4.0.0.xsd">
  <modelVersion>4.0.0</modelVersion>
 
  <groupId>com.netology.app</groupId>
  <artifactId>simple-app</artifactId>
  <version>1.0-SNAPSHOT</version>
   <repositories>
    <repository>
      <id>my-repo</id>
      <name>maven-public</name>
      <url>http://158.160.156.220:8081/repository/maven-public/</url>
    </repository>
  </repositories>
  <dependencies>
     <dependency>
      <groupId>netology</groupId>
      <artifactId>java</artifactId>
      <version>8_282</version>
      <classifier>distrib</classifier>
      <type>jar</type>
    </dependency> 
  </dependencies>
</project>
```
