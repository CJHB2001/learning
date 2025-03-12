# 🚕 Mega City Cab Service Web Application

![Mega City Cab Logo](/logoMega.png)

This repository contains the Maven-based **MEGA CITY CAB SERVICE Web Application**, which handles user authentication, booking management, cabs and driver management, and more for comprehensive cab service operations.

## 🚀 Technologies Used

- **Eclipse IDE**: Integrated development environment for Java development.
- **Maven**: Project management and dependency management tool.
- **Tomcat 9**: Servlet container to run the web application.
- **MySQL**: Database for storing customer, orders, and reservation data.
- **Bootstrap 5**: Frontend framework for building responsive UIs.
- **Font Awesome & Boxicon**: Custom fonts and icons.
- **JUnit 5**: Unit testing framework.
- **Toastr**: For displaying non-blocking notifications.

## 📷 Application Screenshots

<div style="display: flex; justify-content: space-between; flex-wrap: wrap;">
  <div style="width: 48%; margin-bottom: 20px;">
    <img src="/api/placeholder/600/400" alt="Dashboard View" style="width: 100%; border-radius: 8px; box-shadow: 0 4px 8px rgba(0,0,0,0.1);">
    <p align="center"><strong>Dashboard View</strong></p>
  </div>
  <div style="width: 48%; margin-bottom: 20px;">
    <img src="/api/placeholder/600/400" alt="Booking Interface" style="width: 100%; border-radius: 8px; box-shadow: 0 4px 8px rgba(0,0,0,0.1);">
    <p align="center"><strong>Booking Interface</strong></p>
  </div>
  <div style="width: 48%; margin-bottom: 20px;">
    <img src="/api/placeholder/600/400" alt="Driver Management" style="width: 100%; border-radius: 8px; box-shadow: 0 4px 8px rgba(0,0,0,0.1);">
    <p align="center"><strong>Driver Management</strong></p>
  </div>
  <div style="width: 48%; margin-bottom: 20px;">
    <img src="/api/placeholder/600/400" alt="Customer Portal" style="width: 100%; border-radius: 8px; box-shadow: 0 4px 8px rgba(0,0,0,0.1);">
    <p align="center"><strong>Customer Portal</strong></p>
  </div>
</div>

## 🛠️ Installation and Setup

To set up the project locally using **Eclipse IDE**, follow these steps:

### 1. Clone the repository
- Open Eclipse IDE.
- Go to **File > Import > Git > Projects from Git > Clone URI**.
- Enter the repository URL: `https://github.com/CJHB2001/MegaCityCab`.
- Click **Next** and complete the clone process.

### 2. Import the Maven Project
- After cloning, go to **File > Import > Maven > Existing Maven Projects**.
- Browse to the location where the project was cloned, select the root folder, and click **Finish**.

### 3. Set up MySQL Database
- Create a MySQL database, e.g., `megacitycab`.
- Open the file `src\main\java\com\util\DatabaseUtil.java` in Eclipse.
- Update the following properties with your MySQL credentials:
  ```java
  private static final String URL = "jdbc:mysql://localhost:3306/megacitycab";
  private static final String USER = "Your user name";
  private static final String PASSWORD = "Your password";
  ```

### 4. Configure Tomcat in Eclipse
- Go to **Window > Show View > Servers**.
- Right-click in the **Servers** tab and select **New > Server**.
- Choose **Apache Tomcat v9.0** and point to your Tomcat installation directory.
- Add the project to the server and click **Finish**.

### 5. Run the Application
- Right-click on the project, select **Run As > Run on Server**.
- The application should now be running at `http://localhost:8080`.

## 🧪 Running Unit Tests

To run the unit tests using **JUnit 5** in Eclipse:

1. **Right-click on the project folder** or individual test class (e.g., `CustomerRegistrationServlet`, `CustomerDAO`).
2. Select **Run As > JUnit Test**.
3. Eclipse will display the test results in the **JUnit** view.

You can also run all tests via Maven:
```bash
mvn test
```

## 🔄 Version Control and GitHub Integration

This project utilizes **Git** for version control and **GitHub** for repository management. Here's how version control practices are applied:

- **Multiple commits**: Frequent commits with detailed messages documenting the addition of features, bug fixes, and improvements.
- **Branching**: The project uses branches for feature development and bug fixes.
- **Cherry picking**: Selective commits are applied across branches when needed.
- **Tags**: The project uses tags to mark key milestones, such as `v1.0` for the initial release and subsequent versions.
- **Releases**: The initial release was done after the project was finalized for deployment, and further releases will continue as new features are added.
- **Dependabot Alerts**: GitHub's Dependabot was integrated to detect security vulnerabilities. Various issues related to dependencies have been identified and resolved through this.

## 📁 Folder Structure

```
project-root/
│
├── src/
│   ├── main/
│   │   ├── java/com/res/
│   │   │   ├── controller/ - Servlets for all users
│   │   │   ├── service/    - Business logic layer
│   │   │   ├── dao/        - Database interaction layer
│   │   │   ├── enums/      - Enums for application
│   │   │   ├── model/      - Entity classes representing database tables
│   │   │   └── util/       - Database connection manager
│   │   │
│   │   └── webapp/
│   │       ├── WEB-INF/view/ - Contains views related to the project
│   │       ├── AdminArea/    - Admin related images, CSS, JS and JSP files
│   │       ├── DriverArea/   - Driver related images, CSS, JS and JSP files
│   │       └── PublicArea/   - Customer related images, CSS, JS and JSP files
│   │
│   └── test/
│       └── java/ - Contains unit tests (available in staging/test branch only)
│
└── pom.xml - Maven configuration file
```

## 🧪 Test Classes

The project includes comprehensive tests for all major components:

- **DAO Tests**: `CustomerDAOTest`, `BlogDAOTest`, `BookingDAO`, `UserDAO`
- **Model Tests**: `CustomerModel`, `UserModel`, `BlogModel`
- **Service Tests**: `BookingService`, `BlogService`
- **Servlet Tests**: `CustomerLoginServlet`, `CustomerRegistrationServlet`, `BlogServlet`

## 📄 License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for more details.

---

<div align="center">
  <p>© 2025 Mega City Cab Service. All rights reserved.</p>
</div>
