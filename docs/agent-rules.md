# 🤖 Agent Rules - Hard Constraints

## 🎯 Objective

These rules define how AI agents must behave when generating or modifying code in this repository.

They are mandatory and must always be followed.

---

## 🧱 Architecture Rules

* Follow the layered architecture strictly:

  * controller → service → dto

* DO NOT:

  * Put business logic inside controllers
  * Skip layers
  * Create unnecessary abstractions

---

## 📦 Code Placement Rules

* Controllers:

  * Handle HTTP requests and responses only
  * No business logic

* Services:

  * Contain all business logic

* DTOs:

  * Used for input/output only
  * No logic inside DTOs

---

## 🧩 Code Style Rules

* Use Lombok whenever possible:

  * @Data
  * @Builder
  * @NoArgsConstructor
  * @AllArgsConstructor

* DO NOT:

  * Manually implement getters/setters (unless necessary)
  * Add unnecessary comments
  * Over-engineer solutions

---

## ⚙️ Technology Constraints

* Language: Java

* Framework: Spring Boot

* Build tool: Maven

* Do not introduce new frameworks or libraries unless explicitly required.

---

## 🧪 Simplicity Rule (VERY IMPORTANT)

* Always choose the simplest working solution.

* DO NOT:

  * Add validations unless explicitly required
  * Add database integration unless explicitly required
  * Add security, authentication, or authorization
  * Add external API integrations

---

## 🔍 Scope Control

* Only implement what is explicitly requested in the issue.

* DO NOT:

  * Anticipate future features
  * Refactor unrelated code
  * Modify files outside the scope

---

## 🧠 Naming Conventions

* Classes:

  * Controller → *Name*Controller
  * Service → *Name*Service
  * DTO → *Name*DTO

* Endpoints:

  * Use REST conventions
  * Keep naming consistent and simple

---

## 🔁 Idempotency Rule

* Before creating new files:

  * Check if similar structure already exists
  * Reuse existing patterns

---

## 🚫 Forbidden Actions

* Do not delete existing code unless explicitly required
* Do not rename existing classes without reason
* Do not change project structure

---

## ✅ Output Expectations

Every generated feature should include:

* Controller
* Service
* DTO (if applicable)

Keep everything minimal and functional.

---

## 📌 Final Rule

When in doubt:
→ choose simplicity
→ follow existing patterns
→ do not invent complexity
