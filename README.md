# Employee Management System

## Project Overview
The Employee Management System is a web-based application developed using **Spring Boot, Spring MVC, Spring Data JPA, Thymeleaf, and MySQL**. The system allows users to perform CRUD (Create, Read, Update, Delete) operations on employee records efficiently.

## Technologies Used
- **Backend:** Spring Boot, Spring MVC, Spring Data JPA
- **Frontend:** Thymeleaf, HTML, CSS, Bootstrap
- **Database:** MySQL
- **Build Tool:** Maven

## Features
- Add a new employee
- View all employees
- Update employee details
- Delete an employee record
- Flash messages for successful operations
- User-friendly UI with Bootstrap

## Project Structure
```
in.sp.main
│── controller
│   ├── EmpController.java
│
│── entity
│   ├── Employee.java
│
│── repository
│   ├── EmpRepository.java
│
│── service
│   ├── EmployeeService.java
│   ├── EmployeeServiceImpl.java
│
│── resources
│   ├── templates
│   │   ├── index.html
│   │   ├── add_emp.html
│   │   ├── edit.html
│
│── application.properties
│
│── main
│   ├── Application.java
```

## Installation & Setup
### Prerequisites:
- JDK 17+
- MySQL Server
- Maven
- IDE (Eclipse, IntelliJ IDEA, or VS Code)

### Steps to Run:
1. Clone the repository:
   ```sh
   git clone <repository-url>
   ```
2. Navigate to the project folder:
   ```sh
   cd employee-management-system
   ```
3. Configure the database in `application.properties`:
   ```properties
   spring.datasource.url=jdbc:mysql://localhost:3306/emp_db
   spring.datasource.username=root
   spring.datasource.password=yourpassword
   spring.jpa.hibernate.ddl-auto=update
   ```
4. Build and run the project:
   ```sh
   mvn spring-boot:run
   ```
5. Open the browser and access:
   ```
   http://localhost:8080/
   ```

## API Endpoints
| Method | Endpoint       | Description             |
|--------|--------------|-------------------------|
| GET    | `/`          | View all employees      |
| GET    | `/addemp`    | Show add employee form  |
| POST   | `/register`  | Save new employee       |
| GET    | `/edit/{id}` | Edit an employee        |
| POST   | `/update`    | Update an employee      |
| GET    | `/delete/{id}` | Delete an employee    |

## Future Enhancements
- Implement user authentication and authorization
- Add pagination and filtering options
- Integrate REST API for better scalability

## Contributors
- **Nandlal Sakle** - Developer


