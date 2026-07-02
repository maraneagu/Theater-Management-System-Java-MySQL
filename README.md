# Theater Management System

A Java-based theater management and ticket booking application developed for the **Advanced Object-Oriented Programming** course during my fourth semester at FMI.

The project models two main parts of a theater system:

1. **Theater administration**, where an admin user can manage theater-related components such as spectacles, artists, events, and categories.
2. **Ticket shop functionality**, where users can buy, cancel, and list tickets for events from the theater’s repertoire.

The application uses **Java** for the core logic and **MySQL** for data storage, with SQL scripts written and managed through **MySQL Workbench**.

---

## Features

- User sign-up and login flow
- Admin and regular user functionality
- Theater management section
- Ticket shop section
- Add, remove, and list theater components
- Buy, cancel, and list event tickets
- MySQL database integration
- Audit logging with timestamps for important application actions

---

## Tech Stack

- **Language:** Java
- **Database:** MySQL
- **Database Tool:** MySQL Workbench
- **Core Concepts:** Object-Oriented Programming, JDBC/database interaction, CRUD operations, authentication flow, audit logging

---

## Database / MySQL Workbench

The application stores its data in a MySQL database. The SQL commands used to create the required tables are available here:

[MySQL Theater Commands](https://github.com/maraneagu/Theater-Java/blob/main/MySQLTheaterCommands.txt)

The database supports the main entities of the application, including users, spectacles, categories, directors, artists, events, and tickets.

---

## Sign Up / Log In

The first step when starting the application is authentication. Users can either sign up or log into an existing account.

In the example below, the application is accessed using the `@admin` account, which has permission to add and remove components from the system.

![2023-05-21 (9)](https://github.com/maraneagu/Theater-Java/assets/93272424/9b71e0ff-dde8-4fa3-8496-c63ecf67e778)

---

## Main Menu

After a successful login, users can choose between the main parts of the application:

- Visit the theater
- Visit the theater’s ticket shop
- Log out of the current account

![2023-05-21 (10)](https://github.com/maraneagu/Theater-Java/assets/93272424/51d0cf35-e683-46e2-a955-b28f35384ac7)

---

## Theater Administration

The theater section allows an admin user to manage the structure and content of the theater system.

When logged in as `@admin`, the user can create and manage theater-related components, including:

- Spectacles
- Actors
- Dancers
- Singers
- Directors
- Categories
- Events

This part of the application focuses on administrative CRUD operations and object-oriented modeling of the theater domain.

![2023-05-21 (2)](https://github.com/maraneagu/Theater-Java/assets/93272424/585f331f-ddbf-4070-908e-96b48c3a99dd)

![2023-05-21 (6)](https://github.com/maraneagu/Theater-Java/assets/93272424/cf253792-943b-4e7a-87b7-eec94fb364a9)

---

## Ticket Shop

The ticket shop is available to both admin users and regular users.

From this section, users can:

- Buy tickets for available events
- Cancel existing tickets
- List tickets associated with the theater’s events

This part of the application models the user-facing ticket booking flow.

![2023-05-21 (11)](https://github.com/maraneagu/Theater-Java/assets/93272424/3c3966fd-d047-4708-943c-55a7e5e08ef6)

---

## Audit Logging

The application includes an audit system that records important actions with the current date and time.

Separate audit files are maintained for different parts of the application, including:

- Users
- Spectacles
- Categories
- Directors
- Artists
- Events
- Tickets

The example below shows the `theaterUsers.csv` audit file after logging in as `@admin`, switching to the user `@maraneagu`, and updating the user’s name.

![2023-05-21 (15)](https://github.com/maraneagu/Theater-Java/assets/93272424/4a673f8e-b235-4bfa-868f-dbbe2e795d51)

---

## Project Focus

This project focuses on applying object-oriented programming principles in Java to model a real-world management system.

The main learning goals included:

- Designing domain entities using Java classes
- Implementing CRUD operations
- Connecting application logic to a MySQL database
- Managing different user flows and permissions
- Structuring a larger Java application
- Using audit files to track system activity

---

## Repository

This repository contains the implementation of a Java and MySQL theater management system, including theater administration, ticket booking functionality, authentication, database scripts, and audit logging.
