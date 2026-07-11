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

This repository contains a modular **API Automation Framework** developed for testing the **JSONPlaceholder Posts** endpoints using **Java**, **Rest-Assured**, **TestNG**, and **Maven**.

The framework demonstrates industry-standard API automation practices, including **CRUD operations**, **Map-based payload management**, **centralized assertions**, **end-to-end workflow testing**, **logging**, and **Allure reporting**.

Using a lightweight **Map<String, Object>** payload strategy, the framework provides a flexible and maintainable approach for building dynamic request bodies while promoting **clean architecture**, **code reusability**, and **scalable test automation**.

---

# ✨ Key Features

- ✅ Complete CRUD API Automation
- ✅ Modular Framework Architecture
- ✅ Map-Based Payload Management
- ✅ Centralized Assertion Utilities
- ✅ End-to-End Workflow Testing
- ✅ TestNG Suite Execution
- ✅ Log4j2 Logging
- ✅ Rich Allure Reporting

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
├── .idea/                                                  # IntelliJ configuration
├── .mvn/                                                   # Maven wrapper files
├── allure-results/                                         # Allure execution results
├── logs/
│   └── test.log                                            # Test execution logs
│
├── pom.xml                                                 # Maven dependencies & build configuration
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
│   │   │       └── PayloadManager.java                     # Map-based payload manager
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
│       │       ├── integration/                            # End-to-end workflow tests
│       │       │   └── TestE2EFlow.java
│       │       │
│       │       └── sample/                                 # Sample test implementations
│       │           └── TestIntegrationSample.java
│
└── README.md
```

---

# 📦 Framework Components

| Component | Description |
|------------|-------------|
| **APIConstants** | Stores all API endpoint constants |
| **PayloadManager** | Generates reusable Map-based request payloads |
| **BaseTest** | Provides common test initialization and configuration |
| **AssertActions** | Contains centralized assertion utilities |
| **CRUD Tests** | Implements Create, Read, Update, Delete, and Patch API test scenarios |
| **Integration Tests** | Validates complete end-to-end API workflows |
| **Resources** | Stores Log4j2 configuration files |

---

# 🌐 API Coverage

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

Generate and launch the Allure report using:

```bash
allure serve allure-results
```

<p align="center">
<img width="1100" src="https://github.com/user-attachments/assets/a80f69c2-f0c8-4645-9493-b7db8072b528" alt="JSONPlaceholder Allure Report">
</p>

The command generates and opens an interactive **Allure dashboard** displaying execution results, logs, and test statistics.

---

# 📝 Sample Map-Based Payload

```java
Map<String, Object> payload = new LinkedHashMap<>();

payload.put("title", "API Automation Framework");
payload.put("body", "Testing JSONPlaceholder APIs");
payload.put("userId", 101);
```

---

# ⭐ Repository Highlights

- ✔ Modular API Automation Framework
- ✔ Industry-Standard Project Structure
- ✔ Complete CRUD API Testing
- ✔ Rest-Assured + TestNG
- ✔ Map-Based Payload Management
- ✔ Centralized Assertions
- ✔ End-to-End Integration Testing
- ✔ Log4j2 Logging
- ✔ Rich Allure Reporting

---

# 👨‍💻 Author

**Avinash Sinha**

If you found this repository useful, consider giving it a ⭐.

---

# 📄 License

This repository is intended for **educational** and **learning purposes**.
