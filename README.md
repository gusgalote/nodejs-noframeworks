# Overview

I have never done a full CRUD without using any JS Frameworks, and I think it’s never too late to learn a bit more about how things work under the hood. This project is basically a "User and Address" CRUD API using a relational database (I opted for PostgreSQL),

# 💻 Technologies

- Node.js `v16.x`
- JavaScript
- PostgreSQL

# 📐 Business Logic

- Each user should have an Address
- Users’ Email must be validated with a RegEx

## Database tables

### 👤 User

| Field name | id   | name   | email  | address_id                 |
| ---------- | ---- | ------ | ------ | -------------------------- |
| Field Type | uuid | string | string | string                     |
| References |      |        |        | column id on table Address |

### 🏡Address

| Field name | id   | zip     | city   | street | neighborhood | number                          |
| ---------- | ---- | ------- | ------ | ------ | ------------ | ------------------------------- |
| Field Type | uuid | int (8) | string | string | string       | string? (maybe refactor to int) |
| Null       |      |         |        |        |              | true                            |

# 🚀Features

## Implemented

- Nice REAMDE. EYPI (Explain your project, idiot)

## To implement

- CRUD Users
- Protection against SQL Injection
- Transactions
- Field validations
- Documented endpoints
