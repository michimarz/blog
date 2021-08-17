---
title: "Managing JDK Versions"
date: 2021-08-17T11:25:59+02:00
draft: false
---

## Mac OS / Linux

### Changing JVM version 
Add aliases in ~/.zshrc for zsh  
or in ~/.bash_profile for bash:

```sh
alias j8 = 'export JAVA_HOME=$(/usr/libexec/java_home -v 1.8)'
alias j11 = 'export JAVA_HOME=$(/usr/libexec/java_home -v 11)'
alias j14 = 'export JAVA_HOME=$(/usr/libexec/java_home -v 14)'
alias j16 = 'export JAVA_HOME=$(/usr/libexec/java_home -v 16)'
```

### Listing all JVMs installed

List all JVMs installed:
```sh
% /usr/libexec/java_home -V
```

