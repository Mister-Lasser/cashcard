## 💳 CashCard App

A simple and secure **Spring Boot REST API** for managing user cash cards — create, view, update, and delete cards with balance information.
Designed for learning, scalability, and clean code.

---

## 🚀 Features

* ✅ Create a new CashCard
* 💰 Retrieve balance and details by ID
* 🔄 Update CashCard information (e.g., balance)
* ❌ Delete a CashCard
* 🧑‍💻 Secured endpoints with user authentication
* 🧪 Comprehensive test coverage (JUnit + Spring Boot Test)
* 🌱 Built using RESTful design principles

---

## 🛠️ Tech Stack

| Layer          | Technology                               |
| -------------- | ---------------------------------------- |
| **Backend**    | Java 22, Spring Boot 3.x                 |
| **Security**   | Spring Security (Basic Auth / JWT ready) |
| **Database**   | H2 (in-memory)                           |
| **Build Tool** | Maven or Gradle                          |
| **Testing**    | JUnit 5, Spring Boot Test                |

---

## 📁 Project Structure

```
cashcard-app/
│
├── src/
│   ├── main/
│   │   ├── java/com/example/cashcard/
│   │   │   ├── CashCard.java
│   │   │   ├── CashCardController.java
│   │   │   ├── CashCardRepository.java
│   │   │   ├── SecurityConfig.java
│   │   │   └── CashCardApplication.java
│   │   └── resources/
│   │       └── schema.sql
│   └── test/
│       ├── java/com/example/cashcard/
│       |   ├── CashCardJsonTest.java
│       |   └── CashCardApplicationTests.java
│       └── resources/
|           ├── com/example/cashcard/
|           |   ├── list.json
|           |   └── single.json
│           └── data.sql
│
├── build.gradle
└── README.md
```

---

## ⚙️ Setup & Run

### Prerequisites

* Java 22
* Gradle
* Git

### Steps

```bash
# Clone the repository
git clone https://github.com/Mister-Lasser/cashcard.git

cd cashcard

# Build the project
./gradlew clean install

# Run the app
./gradlew run
```

## 🧩 Example Endpoints

| Method   | Endpoint          | Description              |
| -------- | ----------------- | ------------------------ |
| `GET`    | `/cashcards`      | Get all cash cards       |
| `GET`    | `/cashcards/{id}` | Get cash card by ID      |
| `POST`   | `/cashcards`      | Create new cash card     |
| `PUT`    | `/cashcards/{id}` | Update cash card balance |
| `DELETE` | `/cashcards/{id}` | Delete a cash card       |

### Example JSON

```json
{
  "id": 99,
  "amount": 123.45,
  "owner": "sarah1"
}
```

---

## 🧪 Running Tests

```bash
./gradlew test
```

---

## 🧠 Learning Goals

This project was created to explore:

* REST API development with Spring Boot
* CRUD operations using Spring Data JPA
* Test-driven development (TDD)
* Secure API design

---

## 👨‍💻 Author

**Mister-Lasser**
💼 Developer & Learner — Exploring Java, Spring Boot, C++, PostgreSQL, and Cybersecurity

---
