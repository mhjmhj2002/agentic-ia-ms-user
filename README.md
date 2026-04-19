# Agentic IA - Ms User

## 📌 Descrição

Este projeto faz parte de um ecossistema de microsserviços utilizado para estudos de automação com IA (Agentic AI).

A Web API atua como ponto de entrada das requisições e orquestra chamadas para outros microsserviços.

---

## 🧱 Arquitetura

O projeto segue uma arquitetura em camadas:

* **controller** → expõe endpoints REST
* **service** → contém a lógica de negócio
* **dto** → objetos de transporte de dados

---

## 📁 Estrutura de Pacotes

```
controller/
service/
dto/
```

---

## ⚙️ Tecnologias

* Java 21
* Spring Boot
* Maven
* Lombok

---

## 📏 Padrões de Código

### Estrutura

* Controllers devem ser responsáveis apenas por entrada/saída
* Services devem conter a lógica de negócio
* DTOs devem ser usados para comunicação externa

---

### Lombok

Este projeto utiliza Lombok para reduzir boilerplate.

Use preferencialmente:

* @Data
* @Builder
* @NoArgsConstructor
* @AllArgsConstructor

Evite criar getters/setters manualmente.

---

## 🤖 Diretrizes para IA (IMPORTANTE)

Ao gerar código para este projeto, siga as regras:

* Utilize Java + Spring Boot
* Respeite a arquitetura em camadas (controller → service → dto)
* NÃO implemente lógica de negócio no controller
* Utilize Lombok sempre que possível
* Mantenha o código simples e legível
* Não adicionar complexidade desnecessária
* Não criar integrações externas sem necessidade

---

## 🚀 Objetivo do Projeto

Este repositório é utilizado para experimentos com automação de desenvolvimento baseada em IA, incluindo:

* geração automática de código
* criação automática de PRs
* tomada de decisão baseada em contexto

---

## 📌 Observações

Este projeto é simplificado e não representa um sistema produtivo completo.
