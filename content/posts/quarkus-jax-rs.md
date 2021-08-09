---
title: "Quarkus JAX-RS"
date: 2021-08-05T09:22:21+02:00
draft: false
---

# Adnotacje JAX-RS

## Ścieżka w URL

```java
@Path("/hello") 

@Path("/hello/{username}")
// dostęp do tego parametru username:
@PathParam("username")
```

## Metody HTTP

```java
@GET
@POST
@PUT
@DELETE

@HEAD // auto support
@OPTIONS // auto support
@PATCH
```

## Dostęp do parametrów

```java
@PathParam
@QueryParam
@FormParam

@DefaultValue
```

## Media Type

```java
@Produces("text/html")
@Consumes("{text/plain, text/html}")
```


