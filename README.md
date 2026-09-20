# TDD — Pizza Ordering System

A small Java project developed as an academic exercise in **Test-Driven Development (TDD)** and **unit testing**.

The project models a simple pizzeria domain and uses **JUnit 4** tests to verify the behavior of ingredients, pizzas, customers, and orders.

> Academic project developed in 2020 for the **Técnicas de Programação 2** course at **IFSP**.

## Overview

The exercise starts from a partially specified pizzeria system and focuses on implementing and validating the required behavior through automated tests.

The main domain objects are:

- **Ingrediente** — represents an ingredient with a name, quantity, and price.
- **Pizza** — manages ingredients, profit margin, and the resulting pizza price.
- **Cliente** — stores customer information such as name, address, phone, and reference.
- **Pedido** — manages pizzas in an order and calculates totals and taxes.

The test suite covers object creation, calculations, collection management, profit margins, order totals, and tax calculations.

## Project Structure

```text
.
├── PizzaTDD/
│   ├── src/
│   │   └── edu/ifsp/tdd/test/Pizzaria/
│   │       ├── Cliente.java
│   │       ├── Ingrediente.java
│   │       ├── Pedido.java
│   │       └── Pizza.java
│   │
│   ├── test/
│   │   └── edu/ifsp/tdd/test/Pizzaria/
│   │       ├── ClienteTest.java
│   │       ├── IngredienteTest.java
│   │       ├── PedidoTest.java
│   │       └── PizzaTest.java
│   │
│   └── nbproject/
│       └── ...
│
└── README.md
```

The project follows the conventional separation between production code (`src/`) and automated tests (`test/`).

## Test Coverage

The repository contains **21 JUnit test cases** covering the main requirements of the assignment:

| Test Class | Focus | Tests |
|---|---|---:|
| `IngredienteTest` | Object creation and ingredient value calculation | 3 |
| `PizzaTest` | Ingredient management and pizza price calculation | 7 |
| `PedidoTest` | Order totals and tax calculations | 7 |
| `ClienteTest` | Customer data setters | 4 |
| **Total** | | **21** |

### Examples of Tested Behavior

- Creating ingredients and calculating their values from quantity and unit price.
- Adding and removing ingredients from a pizza.
- Calculating the total ingredient cost of a pizza.
- Applying different profit margins to a pizza.
- Creating customers and storing their contact information.
- Adding multiple pizzas to an order.
- Calculating order totals with different tax rates.
- Verifying order totals both with and without taxes.

Floating-point calculations use JUnit's delta-based assertions where appropriate.

## Technologies

- **Java 14**
- **JUnit 4**
- **Apache Ant**
- **NetBeans project structure**
- **Hamcrest**

The project configuration is maintained through NetBeans' `nbproject/` files and the Ant `build.xml`.

## Running the Tests

This is a NetBeans/Ant project, so it can be opened directly in **Apache NetBeans**.

### Using NetBeans

1. Clone the repository.
2. Open the `PizzaTDD` directory as a NetBeans project.
3. Build the project.
4. Run the project's test suite.

NetBeans will execute the JUnit tests and display the results in its test runner.

### Using Apache Ant

From the `PizzaTDD` directory, run:

```bash
ant test
```

The project is configured to compile against **Java 14** and uses JUnit 4 for automated testing.

## What This Project Demonstrates

Although this is a small academic project, it demonstrates several practical software development concepts:

- Writing automated unit tests with JUnit.
- Translating functional requirements into test cases.
- Testing calculations and business rules.
- Testing object state and behavior.
- Working with collections of domain objects.
- Using assertions to validate expected behavior.
- Organizing Java production code and tests separately.
- Using automated tests as a safety net for refactoring and implementation changes.

## Academic Context

This repository contains coursework from the second semester of **2020**, created as part of an assessment for the **Técnicas de Programação 2** course at **Instituto Federal de São Paulo (IFSP)**.

The original assignment provided a set of requirements and test-related tasks around a simple pizza-ordering domain. The implementation in this repository represents the completed exercise and its accompanying test suite.

## Repository

**GitHub:**  
https://github.com/Maxwel-Araujo-Costa/pizza-ordering-tdd

---

*This project is preserved as part of my academic development history and as an example of early experience with automated testing and TDD-oriented development.*
