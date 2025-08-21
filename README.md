#  Recipe API - Spring Boot Project

This is a **Spring Boot CRUD application** for managing recipes, built as part of assignment work.  
It uses **Java 17**, **Spring Boot**, and **MySQL**.

---

##  Features
- Add new recipes  
- View all recipes  
- Update existing recipes  
- Delete recipes  

---

##  Tech Stack
- Java 17  
- Spring Boot  
- Spring Data JPA  
- MySQL Database  
- Maven  

---

##  How to Run
1. Clone the repository:
   ```bash
   git clone https://github.com/YOUR-USERNAME/recipe-api.git
   cd recipe-api
Configure your MySQL database in application.properties:

properties
Copy
Edit
spring.datasource.url=jdbc:mysql://localhost:3306/recipe_db
spring.datasource.username=root
spring.datasource.password=your_password
spring.jpa.hibernate.ddl-auto=update
Run the app:

bash
Copy
Edit
mvn spring-boot:run
## API Endpoints
Method	Endpoint	Description
GET	/api/recipes	Get all recipes
GET	/api/recipes/{id}	Get recipe by ID
POST	/api/recipes	Add new recipe
PUT	/api/recipes/{id}	Update recipe by ID
DELETE	/api/recipes/{id}	Delete recipe by ID

## Sample JSON for POST
json
Copy
Edit
{
  "cuisine": "Indian",
  "title": "Paneer Butter Masala",
  "rating": 4.7,
  "prepTime": 15,
  "cookTime": 25
}
## Example Output (GET)
json
Copy
Edit
[
{
 "id": 1,
    "cuisine": "Indian",
    "title": "Paneer Butter Masala",
    "rating": 4.7,
    "prepTime": 15,
    "cookTime": 25
  }
]
## Screen Shorts of post man output
$$ for post data
https://github.com/Akula123sri/Recipe-api/blob/main/postdata.png.png
$$ for getall data
https://github.com/Akula123sri/Recipe-api/blob/main/getall.png.png
$$ for getbyid
https://github.com/Akula123sri/Recipe-api/blob/main/getbyid.png.png
