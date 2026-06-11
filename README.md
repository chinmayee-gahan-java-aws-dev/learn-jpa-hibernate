# Spring Boot JPA Hibernate Demo

Spring Boot project comparing 3 approaches to access data: JDBC vs JPA vs Spring Data JPA. Uses H2 in-memory database and CRUD operations on `Course` entity.

## 🚀 Tech Stack
- Spring Boot 3.x
- Spring Data JPA / Hibernate 
- JDBC Template
- H2 Database
- Maven

## 📁 Project Structure

```
learn-jpa-hibernate/
├── src/main/java/com/jpahibernate/
│   ├── course/
│   │   ├── Course.java          # Entity
│   │   ├── CourseJdbcCommandLineRunner.java  # JDBC approach
│   │   ├── CourseJpaCommandLineRunner.java   # JPA approach  
│   │   └── SpringJpaRepositoryCommandLineRunner.java  # Spring Data JPA
│   └── LearnJpaHibernateApplication.java
└── src/main/resources/application.properties
```

## ▶️ Run Project
```bash
mvn spring-boot:run
```
H2 Console: http://localhost:8080/h2-console

## 📚 Key Learnings
1. `@Entity`, `@Id`, `@Table` annotations
2. JDBC Template vs JPA vs Spring Data JPA comparison
3. Repository pattern with Spring Data JPA
4. H2 in-memory DB configuration

## 🎯 SAA-C03 Relevance
Demonstrates data persistence patterns used in AWS applications. Easy to extend with AWS RDS later for cloud deployment.