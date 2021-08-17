---
title: "Quarkus Run"
date: 2021-08-17T13:53:41+02:00
draft: false
---

## Create project structure

On Windows:
```sh
mvn io.quarkus:quarkus-maven-plugin:2.1.2.Final:create -DprojectGroupId=org.acme -DprojectArtifactId=%1 -DclassName="org.acme.getting.started.GreetingResource" -Dpath="/hello"
```

## Run the app
```sh
mvn compile quarkus:dev
```


