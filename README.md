# Thymeleaf Security Project

Simple Spring Boot app using Spring Security and Thymeleaf.  
Handles login and redirects users based on roles.

## Features
- Custom login page  
- Role-based page access  
- Redirect after login  
- Logout support  

## Roles & Access
| Role     | Access           |
|----------|------------------|
| EMPLOYEE | `/`              |
| MANAGER  | `/leaders`, `/`  |
| ADMIN    | `/systems`, `/`  |

## Users (In-Memory)
- `john / test123` → EMPLOYEE  
- `mary / test123` → MANAGER -EMPLOYEE  
- `abdo / test123` → ADMIN - MANAGER -EMPLOYEE

## Run
- Open in IntelliJ  
- Java 17+, Maven  
- Run `SpringBootSecurityThymeleafApplication`

## Pages
- `/login`  
- `/logout`  
- `/access-denied`
- `/leaders`
- `/systems`  
