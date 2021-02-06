#  Employee REST API

The user can perform CRUD operations through this REST API.

#### Technologies used

1. Maven
2. Spring Boot
3. Spring Data REST
4. JSON
5. MySQL
6. JDBC

### Description

The user can perform CRUD operations on an 
<a href="src/main/java/com/spencer/forrest/employeerestapi/entity/Employee.java">
employee
</a> entity using HTTP methods:
1. POST "/api/employees" to create a new employee 
2. GET "/api/employees" to retrieve a list of all employees
3. GET "/api/employees/{employeeId}" to retrieve a specific employee using his id
4. PUT "/api/employees/{employeeId}" to update an employee using his id
5. DELETE "/api/employees/{employeeId}" to delete an employee using his id

### JSON format

JSON representation of the 
<a href="src/main/java/com/spencer/forrest/employeerestapi/entity/Employee.java">
employee
</a> entity
```
{
    "id": 99,
    "firstName": "John",
    "lastName": "Clayton",
    "email": "jhon@email.com"
}
```

### Spring Data REST

Use of 
<a href="src/main/java/com/spencer/forrest/employeerestapi/repository/EmployeeRepository.java">
EmployeeRepository
</a> interface that extends the 'JpaRepository' interface.<br/>
This interface enables CRUD operations on the entity 
<a href="src/main/java/com/spencer/forrest/employeerestapi/entity/Employee.java">
Employee
</a> which has an integer as 'id'.

### Configuration

The <a href="src/main/resources/application.properties">application.properties</a> file contains the information needed 
for the application to connect to a database (url, username, password).

### Database

The file <a href="sql/employee.sql">employee.sql<a/> is a script to create an employee table and insert sample data.




