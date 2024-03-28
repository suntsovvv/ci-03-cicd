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
![image](https://github.com/suntsovvv/ci-03-cicd/assets/154943765/024e1ad4-7de2-497f-88ae-0b7d32277d47)   

## Знакомство с Maven   
