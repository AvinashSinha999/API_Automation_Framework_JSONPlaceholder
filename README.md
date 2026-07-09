# 🚀 API Automation Framework | JSONPlaceholder

> A modular **API Automation Framework** built using **Java**, **Rest-Assured**, **TestNG**, **Maven**, **AssertJ**, and **Allure Reports** to automate testing of the **JSONPlaceholder Posts** endpoints.

<p align="center">

![Java](https://img.shields.io/badge/Java-11+-blue?logo=openjdk)
![Maven](https://img.shields.io/badge/Maven-Build%20Tool-C71A36?logo=apachemaven&logoColor=white)
![RestAssured](https://img.shields.io/badge/RestAssured-API--Testing-yellowgreen)
![TestNG](https://img.shields.io/badge/TestNG-Framework-brightgreen)
![AssertJ](https://img.shields.io/badge/AssertJ-Assertions-orange)
![Allure](https://img.shields.io/badge/Allure-Reports-ff69b4)
![Log4j2](https://img.shields.io/badge/Log4j2-Logging-yellow)

</p>

---

# 🗂️ Overview

This repository contains a modular **API Automation Framework** for testing the **JSONPlaceholder Posts** endpoints.

Built with **Java**, **Rest-Assured**, **TestNG**, and **Maven**, the framework demonstrates industry-standard API automation practices, including reusable payload management, centralized assertions, CRUD operations, end-to-end workflow testing, logging, and rich Allure reporting.

The framework uses **Map-based payload creation**, providing a lightweight and flexible approach for building dynamic request bodies while maintaining clean and reusable test code.

---

# ✨ Features

- ✅ Complete CRUD API Automation
- ✅ Modular Framework Design
- ✅ Map-Based Payload Management
- ✅ Centralized Assertion Utilities
- ✅ End-to-End Integration Testing
- ✅ TestNG Suite Execution
- ✅ Log4j2 Logging
- ✅ Allure Reporting

---

# 🛠️ Tech Stack

| Technology | Usage |
|------------|-------|
| Java 11+ | Programming Language |
| Maven | Dependency & Build Management |
| Rest-Assured | API Automation |
| TestNG | Test Framework |
| AssertJ | Fluent Assertions |
| Log4j2 | Logging |
| Allure Reports | Test Reporting |
| IntelliJ IDEA | Development IDE |

---

# 🏗️ Project Structure

```text
API_Automation_Framework_JSONPlaceholder/
│
├── .idea/                                                  # IntelliJ config
├── .mvn/                                                   # Maven wrapper files
├── allure-results/                                         # Allure results (auto-generated)
├── logs/
│   └── test.log                                            # Execution logs
│
├── pom.xml                                                 # Project dependencies & build config
├── .gitignore
│
├── testng_*.xml                                            # TestNG suite files
│
├── src/
│   ├── main/
│   │   ├── java/com.avinashsinha/
│   │   │   ├── endpoints/
│   │   │   │   └── APIConstants.java                       # API endpoint constants
│   │   │   │
│   │   │   └── modules/
│   │   │       └── PayloadManager.java                     # Payload Manager (Map-based)
│   │   │
│   │   └── resources/
│   │       └── log4j2.xml                                  # Logging configuration
│   │
│   └── test/
│       ├── java/com.avinashsinha/
│       │   ├── asserts/
│       │   │   └── AssertActions.java                      # Assertion utilities
│       │   │
│       │   ├── base/
│       │   │   └── BaseTest.java                           # Base test configuration
│       │   │
│       │   └── tests/
│       │       ├── crud/                                   # CRUD test cases
│       │       │   ├── TestPostsCreate.java
│       │       │   ├── TestPostsDelete.java
│       │       │   ├── TestPostsDetails.java
│       │       │   ├── TestPostsDetailsById.java
│       │       │   ├── TestPostsFullUpdate.java
│       │       │   └── TestPostsPartialUpdate.java
│       │       │
│       │       ├── integration/                            # End-to-end tests
│       │       │   └── TestE2EFlow.java
│       │       │
│       │       └── sample/                                 # Sample Tests
│       │           └── TestIntegrationSample.java
│
└── README.md
```

---

# 📦 Framework Components

| Component | Description |
|------------|-------------|
| **APIConstants** | Stores all API endpoint constants |
| **PayloadManager** | Builds reusable Map-based request payloads |
| **BaseTest** | Provides common test setup and configuration |
| **AssertActions** | Centralized assertion utilities |
| **CRUD Tests** | Individual API CRUD test scenarios |
| **Integration Tests** | End-to-end workflow validation |
| **Resources** | Log4j2 configuration files |

---

# ✅ Test Coverage

| Endpoint | Test Scenario |
|-----------|---------------|
| **POST** `/posts` | Create Post |
| **GET** `/posts` | Retrieve All Posts |
| **GET** `/posts/{id}` | Retrieve Post by ID |
| **PUT** `/posts/{id}` | Full Update Post |
| **PATCH** `/posts/{id}` | Partial Update Post |
| **DELETE** `/posts/{id}` | Delete Post |
| Workflow | End-to-End Integration Testing |

---

# ▶️ Running Tests

Execute any TestNG suite using Maven.

### Example

```bash
mvn clean test -DsuiteXmlFile=testng_integration.xml
```

### Available Test Suites

| Suite | XML File |
|--------|----------|
| Create Post | `testng_createPosts.xml` |
| Delete Post | `testng_deletePosts.xml` |
| Post Details | `testng_detailsPostById.xml` |
| Full Update | `testng_fullUpdate.xml` |
| Partial Update | `testng_partialUpdate.xml` |
| Sample Tests | `testng_sample.xml` |
| End-to-End Flow | `testng_integration.xml` |

---

# 📊 Allure Reports

Generate the report using:

```bash
allure serve allure-results
```

<p align="center">
<img width="1100" src="https://github.com/user-attachments/assets/a80f69c2-f0c8-4645-9493-b7db8072b528" alt="JSONPlaceholder Allure Report">
</p>

The command launches an interactive Allure dashboard in your default browser.

---

# 📝 Sample Map-Based Payload

```java
Map<String, Object> payload = new LinkedHashMap<>();

payload.put("title", "API Automation Framework");
payload.put("body", "Testing JSONPlaceholder APIs");
payload.put("userId", 101);
```

---

# 👨‍💻 Author

**Avinash Sinha**

If you found this repository helpful, consider giving it a ⭐ on GitHub.

---

# 📄 License

This project is intended for **educational** and **learning purposes**.
