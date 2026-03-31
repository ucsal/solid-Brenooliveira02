#  Refatoração – Sistema de Olimpíadas

##  Objetivo
Este projeto tem como objetivo realizar a refatoração de um sistema legado de aplicação de provas, melhorando a organização, legibilidade e manutenção do código, **sem alterar o comportamento funcional original**.

---

##  Principais Alterações

###  1. Encapsulamento do cálculo de nota

####  O que foi feito
O método de cálculo de nota foi removido da classe `App` e implementado diretamente na classe `Tentativa`.

####  Antes
O cálculo era feito externamente:

```java
public static int calcularNota(Tentativa tentativa)
