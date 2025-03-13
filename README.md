# Mega City Cab Service Web Application

![GitHub](https://img.shields.io/github/license/CJHB2001/MegaCityCab)
![Java](https://img.shields.io/badge/Java-17-orange)
![Tomcat](https://img.shields.io/badge/Tomcat-9-red)
![MySQL](https://img.shields.io/badge/MySQL-Latest-blue)

This repository contains the Maven-based **MEGA CITY CAB SERVICE Web Application**, a comprehensive solution for cab service operations including user authentication, booking management, and driver coordination.

## 🚕 Application Preview

<div align="center">
  <table>
    <tr>
      <td><img src="/Documents/Images/HomePage.png" width="300" alt="Home Page"></td>
      <td><img src="/Documents/Images/AdminDriverLoin.png" width="300" alt="Admin Driver Login"></td>
      <td><img src="/Documents/Images/AdminDasboard.png" width="300" alt="Admin Dashboard"></td>
    </tr>
    <tr>
      <td><img src="/Documents/Images/DriverDashboard.png" width="300" alt="Driver Dashboard"></td>
    </tr>
  </table>
</div>

## 🛠️ Technologies Used

| Category | Technologies |
|----------|-------------|
| **Backend** | Java 17, Maven, Tomcat 9 |
| **Database** | MySQL |
| **Frontend** | Bootstrap 5, Font Awesome, Boxicon |
| **Development** | Eclipse IDE |
| **Testing** | JUnit 5 |
| **UI Components** | Toastr (for notifications) |

## 🚀 Installation and Setup

### Prerequisites
- Java 17 JDK
- Eclipse IDE
- Apache Tomcat 9
- MySQL Database
- Git

### Step-by-Step Setup Guide

#### 1. Clone the Repository

```bash
# Using Eclipse
File > Import > Git > Projects from Git > Clone URI
URI: https://github.com/CJHB2001/MegaCityCab
```

#### 2. Import the Maven Project

```bash
# In Eclipse
File > Import > Maven > Existing Maven Projects
# Select the cloned repository root folder
```

#### 3. Configure Database

- Create a MySQL database named `megacitycab`
- Update database credentials in `src/main/java/com/util/DatabaseUtil.java`:

```java
private static final String URL = "jdbc:mysql://localhost:3306/megacitycab";
private static final String USER = "Your user name";
private static final String PASSWORD = "Your password";
```

#### 4. Configure Tomcat Server

```bash
# In Eclipse
Window > Show View > Servers
Right-click > New > Server
Select Apache Tomcat v9.0
```

#### 5. Launch the Application

```bash
# Right-click on project
Run As > Run on Server
# Access at http://localhost:8080
```

## 🧪 Running Unit Tests

### Using Eclipse

```bash
# For all tests
Right-click project > Run As > JUnit Test

# For specific test class
Right-click test class > Run As > JUnit Test
```

### Using Maven

```bash
mvn test
```

## 📊 Version Control and GitHub Integration

This project uses Git and GitHub with the following practices:

- ✅ **Commit Frequency**: Regular commits with detailed messages
- 🌿 **Branching Strategy**: Structured approach for development and releases
- 🍒 **Cherry-picking**: Selective commit integration when needed
- 🏷️ **Tagging**: Version tags for key milestones (e.g., `v1.0`)
- 📦 **Releases**: Incremental feature and fix releases
- 🔒 **Security**: Dependabot integration for vulnerability detection

## Folder Structure

- **src/main/java/com/res**: Contains the Java source code
  - `controller`: Servlets for all users.
  - `service`: Business logic layer.
  - `dao`: Database interaction layer.
  - `enums`: Enums for application.
  - `model`: Entity classes representing database tables.
  - `util`: Database connection manager.
- **src/main/webapp/WEB-INF/view**: Contains views related to the project.
- **src/main/webapp/AdminArea**: Admin-related assets (images, CSS, JS, JSP files).
- **src/main/webapp/DriverArea**: Driver-related assets (images, CSS, JS, JSP files).
- **src/main/webapp/PublicArea**: Customer-related assets (images, CSS, JS, JSP files).
- **src/test/java**: Contains unit tests written with **JUnit** (available in staging/test branch only).

## Running Tests

To run tests:
- In **Eclipse**, right-click on the project or individual test class and select **Run As > JUnit Test**.
- Or use Maven from the terminal:

  ```bash
  mvn test
  ```

Test classes include:
- `CustomerDAOTest`
- `BlogDAOTest`
- `BookingDAO`
- `UserDAO`
- `CustomerModel`
- `UserModel`
- `BlogModel`
- `BookingService`
- `BlogService`
- `CustomerLoginServlet`
- `CustomerRegistrationServlet`
- `BlogServlet`

## 📄 License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for more details.
