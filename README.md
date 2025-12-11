# Employee Payroll System (OOP)

## 📖 Description
A scalable backend application designed to model workforce data and calculate compensation based on employee classification. This project demonstrates core Object-Oriented Programming (OOP) principles, specifically **Inheritance** and **Polymorphism**, to handle different payment structures within a single system.

The application distinguishes between standard hourly employees (eligible for overtime) and salaried staff (fixed annual compensation), processing payroll over multiple weeks through a unified interface.

## 🛠 Technologies Used
* **Language:** Java
* **IDE:** IntelliJ IDEA
* **Concepts:** Inheritance, Polymorphism, Encapsulation, Method Overriding
* **Architecture:** UML Class Design

## ✨ Key Features

### 🏗 Class Hierarchy
* **`Person` (Base Class):** Manages fundamental demographic data (ID, Name, Title, YOB).
* **`Worker` (Subclass):** Extends `Person` to include hourly wage logic. Implements algorithms to calculate weekly pay, including:
    * **Regular Pay:** Standard hours at base rate.
    * **Overtime Pay:** Hours exceeding 40/week calculated at 1.5x rate.
* **`SalaryWorker` (Subclass):** Extends `Worker` to handle fixed annual salaries.
    * Overrides pay calculation methods to distribute annual salary evenly across 52 weeks, ignoring hourly variations.

### ⚙️ Simulation Driver
* The main driver program simulates a 3-week payroll cycle.
* Iterates through a polymorphic list of employees (both `Worker` and `SalaryWorker`).
* Generates a formatted payroll report to the console, demonstrating the difference in calculation logic between employee types.

## 🏗 System Architecture

### Inheritance Model
The system uses a linear inheritance model to maximize code reuse:
`Person` → `Worker` → `SalaryWorker`

### UML Design
<img width="444" height="663" alt="Lab2UML" src="https://github.com/user-attachments/assets/7b520417-71bf-4acd-9942-af926725e23b" />


## 🚀 How to Run
1. Clone the repository.
2. Open the project in **IntelliJ IDEA**.
3. Navigate to the `Main` (Driver) class.
4. Run the program to view the simulated payroll report in the console.
