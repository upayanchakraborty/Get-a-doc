# 🩺✨ Get-a-Doc — Your Friendly Doctor Appointment System

Welcome to **Get-a-Doc**, a full-stack application built with 💻 **Spring Boot** to manage 🧑‍⚕️ doctors, 🧍‍♀️ patients, and 📅 appointments effortlessly!

---

## 🚀 Features

- 🧑‍⚕️ Add & manage doctors
- 🧍 Register & manage patients
- 📅 Book & track appointments
- 🔗 RESTful APIs
- ⚙️ Spring Boot + Maven powered

---

## 🧰 Tech Stack

| 🔧 Backend       | 🗄️ Database   | 🧪 Testing | 💡 Tools       |
|------------------|---------------|------------|----------------|
| Java 17+         | H2 / MySQL     | JUnit      | Spring Boot    |
| Spring Boot      | JPA / Hibernate| Mockito    | Maven          |

---

## 📁 Project Structure

get-a-doc-main/
├── backend/
│ └── getadoc/
│ ├── src/
│ │ └── main/java/com/webapp/getadoc/
│ │ ├── controller/ # API Controllers 🧩
│ │ ├── model/ # Data Models 📦
│ │ ├── repository/ # JPA Repositories 💾
│ │ └── GetadocApplication.java
│ └── resources/
│ └── application.properties # Config ⚙️
└── .vscode/ (IDE settings)

---

## 💻 Getting Started

### ✅ Prerequisites

- ☕ Java 17+
- 🧰 Maven 3.6+
- 🧠 IDE (VS Code / IntelliJ IDEA)

### ⚙️ Setup Instructions

1. 📦 Clone or unzip this repo
2. 🖱️ Navigate to the backend directory:
    ```bash
    cd backend/getadoc
    ```
3. 🛠️ Build the project:
    ```bash
    mvn clean install
    ```
4. ▶️ Run the Spring Boot application:
    ```bash
    mvn spring-boot:run
    ```

---

## 🌐 API Access

Once running, access:

- 🔍 **Swagger UI** (if integrated): `http://localhost:8080/swagger-ui.html`
- 🧪 **H2 Console** (if enabled): `http://localhost:8080/h2-console`

### 🧾 Sample Endpoints

| Method | Endpoint             | Description              |
|--------|----------------------|--------------------------|
| GET    | `/doctors`           | List all doctors         |
| POST   | `/patients`          | Register a new patient   |
| POST   | `/appointments`      | Book an appointment      |

---

## ⚙️ Configuration

Update `application.properties` as needed:

```properties
# H2 Database Configuration
spring.datasource.url=jdbc:h2:mem:testdb
spring.datasource.driverClassName=org.h2.Driver
spring.jpa.hibernate.ddl-auto=update
