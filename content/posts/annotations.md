---
title: "Annotations"
date: 2021-08-19T13:10:34+02:00
draft: false
---

## Adnotacje vs. pliki konfiguracyjne

Zasada stosowania:
Adnotacje - Jeżeli metadane są związane z elementem Javy (metoda, klasa, pole, zmienna, pakiet, itd.)
Pliki konfiguracyjne - w innych przypadkach (deployment info, DB connection params, runtime/launch params)

## Ważne adnotacje

* @Nullable, @Nonnull -> mniej Null Pointer Exceptions
* @Override - obowiązkowe od J6
* @FunctionalInterface - od J8, interfejs z dokładnie 1 metodą abstrakcyjną
* @SupressWarnings - lokalnie można wyłączyć warningi, kiedy wiemy lepiej niż kompilator
