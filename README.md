

```markdown
# 🧪 API Testing with Rest Assured - ReqRes API

This project demonstrates basic **API testing** using the [ReqRes](https://reqres.in/) public API. The tests are written in **Java** using the **Rest Assured** library and **TestNG** framework.

It covers the full CRUD operations:
- `GET`: Retrieve user list
- `POST`: Create a user
- `PUT`: Update a user
- `DELETE`: Remove a user

---

## 📁 Project Structure

```

src/
└── test/
└── java/
└── day1/
└── HTTPRequests.java
pom.xml
README.md

````

---

## 🔧 Tools & Technologies

| Tool              | Purpose                        |
|------------------|---------------------------------|
| Java              | Programming Language            |
| Rest Assured      | API Testing Framework           |
| TestNG            | Test Runner                     |
| Maven             | Build & Dependency Management   |
| ReqRes API        | Public Dummy REST API for Testing |

---

## 🚀 How to Run

### 🖥 Prerequisites

- Java JDK 8+
- Maven installed
- IDE (e.g., IntelliJ, Eclipse)

### 🧪 Steps to Execute

1. Clone this repo:

```bash
git clone https://github.com/yourusername/RestAssuredAPI-Testing.git
cd RestAssuredAPI-Testing
````

2. Run tests using Maven:

```bash
mvn test
```

Or, from your IDE: right-click `HTTPRequests.java` and run as TestNG Test.

---

## 🧪 API Test Summary

### ✅ `getUsers()`

* Sends a `GET` request to retrieve users from page 2
* Asserts status code = 200
* Validates `page` field value = 2

### 🆕 `createUser()`

* Sends a `POST` request to create a new user
* Request body includes `name` and `job`
* Extracts and stores the `id` for use in later tests

### ✏️ `updateUser()`

* Sends a `PUT` request using the previously generated user `id`
* Updates the user's `name` and `job`
* Asserts status code = 200

### ❌ `deleteUser()`

* Sends a `DELETE` request using the stored `id`
* Asserts status code = 204 (successful deletion)

---

## 🧠 Key Concepts Demonstrated

* Fluent API pattern: `given() → when() → then()`
* Using **HashMap** for request payload
* Extracting response data with `.jsonPath()`
* Logging full request/response
* Method dependency using TestNG
* Reusable test structure for REST APIs

---

## 📌 Note

* The project uses the `https://reqres.in` public API which **does not actually persist data** — it's a mock API used for demonstration purposes.
* The `id` received after user creation is simulated.

---

## 🙋‍♀️ Author

**Feona Donnal**
📧 [feonadonnal@gmail.com](mailto:feonadonnal@gmail.com)
🔗 [LinkedIn](https://www.linkedin.com/in/yourprofile)

---

> ⚠️ This project is for **educational/demo purposes** only and is not affiliated with ReqRes or its maintainers.

```


