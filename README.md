# ONE-STOP PERSONALIZED CAREER AND EDUCATION ADVISOR

## PROJECT OVERVIEW

🔸 The One-Stop Personalized Career and Education Advisor is a web-based platform designed to assist students in making informed academic and career decisions. The system provides personalized career recommendations, educational guidance, skill development suggestions, and learning resources based on user interests, qualifications, and career goals.

## PROBLEM STATEMENT

🔸 Many students face difficulties in selecting the right career path and educational opportunities due to a lack of personalized guidance and reliable information. Career-related resources, educational options, and skill development opportunities are often scattered across multiple platforms, making decision-making challenging. This project aims to provide a centralized platform that offers personalized career recommendations and educational guidance to help students achieve their academic and professional goals.


## REQUIREMENT GATHERING

🔸 Gathered and analyzed the functional and non-functional requirements of the system.

🔸 Identified the needs of students seeking career guidance and educational recommendations.

🔸 Collected information about career paths, educational opportunities, skill development resources, and user preferences.

🔸 Defined the core features required for personalized career and education recommendations.

# OBJECTIVE

🔸 Provide personalized career recommendations based on user interests and qualifications.

🔸 Offer educational guidance and course recommendations.

🔸 Suggest skill development opportunities and learning resources.

🔸 Help students make informed academic and professional decisions.

🔸 Create a centralized platform for career and education planning.
## USER AND MODULE IDENTIFICATION

🔸 Identified the primary users of the system, including students and administrators.

🔸 Analyzed user requirements and system interactions.

🔸 Defined the major modules required for the application.

🔸 Structured the system architecture to ensure smooth communication between modules.

## MODULE LIST

🔸 User Registration and Login Module

🔸 Career Recommendation Module

🔸 Education Guidance Module

🔸 Skill Development Module

🔸 Learning Resources Module

🔸 User Profile Management Module

🔸 Dashboard Module

🔸 Admin Management Module
## Use Case Diagram

![Use Case Diagram](file_000000004d2c7208b85f6b9105f9cbc3.png)
## Database Requirement Analysis

| Table Name | Attributes | Description |
|------------|------------|-------------|
| Users | User_ID (PK), Name, Email, Password, Role | Stores user account information. |
| User_Profile | Profile_ID (PK), User_ID (FK), Qualification, Skills, Interests, Career_Goals | Stores user details and career goals. |
| Careers | Career_ID (PK), Career_Name, Description, Required_Skills | Contains career information. |
| Courses | Course_ID (PK), Course_Name, Institution, Duration | Stores course details. |
| Recommendations | Recommendation_ID (PK), User_ID (FK), Career_ID (FK), Course_ID (FK) | Stores personalized recommendations. |
## ER Diagram

![ER Diagram](file_00000000725072088862bd3e4bb61521.png)
# SQL SCHEMA

## User Table

```sql
CREATE TABLE users (
    user_id INT PRIMARY KEY,
    full_name VARCHAR(100),
    email VARCHAR(100),
    password VARCHAR(255),
    career_interest VARCHAR(100)
);
## Career Table

```sql
-- Career Table
-- Stores career information and descriptions

CREATE TABLE careers (
    career_id INT PRIMARY KEY,
    career_name VARCHAR(100),
    description TEXT
);
```
