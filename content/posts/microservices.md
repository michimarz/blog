---
title: "Microservices"
date: 2021-08-10T10:54:27+02:00
draft: false
---

## Microserwisy vs. Monolit

Architektura Monolitu - wdrożenie pojedynczej jednostki  
Architektura Mikroserwisów - zestaw niezależnie wdrażanych usług, gdzie *każda posiada własną bazę danych*  

* przyspiesza tempo wdrażania zmian - małe autonomiczne zespoły pracują równolegle
* wzrasta utrzymywalność, testowalność, wdrażalność (maintainability, testability, deployability)
* główna wada: wzrost złożoności (complexity)
* wymaga: DevOps, małych autonomicznych zespołów

## Dekompozycja usług

2 strategie dekompozycji:
* Decompose by business capability (według możliwości biznesowych)
* Decompose by sub-domain (według subdomen), DDD - Domain-driven design  

Przeszkody:
* opóźnienia sieci
* synchroniczna komunikacja (obniża dostępność usług)
* utrzymanie spójności danych między usługami
* uzyskanie spójnego widoku danych (wiele baz danych, ACID zapenia spójnoiść tylko w obrębie każdej z nich z osobna)
* God classes (Boskie klasy)

