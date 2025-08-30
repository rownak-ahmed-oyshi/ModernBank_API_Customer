# API Testing Project – Modern Bank Portal

##  Overview
This project validates core features of the **Modern Bank Portal API**, including:
- Customer Registration  
- Customer Login  
- Customer Balance  

The project demonstrates:
- Manual API test cases (written in Excel)  
- Bug reporting with severity and priority  
- Validation of functional, negative, boundary, and security scenarios  

---

##  Tools & Skills Used
- **Postman** for API testing  
- **SwaggerHub** for API documentation reference  
- **Excel (.xlsx)** for structured test case documentation  
- **MySQL** (Database reference)  
- Familiarity with bug tracking workflow (Jira-style reporting)

---

##  Test Case Highlights
- **Customer Registration:** 16 test cases (12 Passed, 4 Failed)  
- **Customer Login:** 10 test cases (All Passed)  
- **Customer Balance:** 10 test cases (All Passed)  

### Covered Scenarios:
- Positive & negative test flows  
- Input validation (null, empty, boolean, boundary values)  
- Security tests (SQL Injection, XSS attempts)  
- Business rule enforcement (minimum deposit validation, password length checks)  
- Response time verification (≤ 2 seconds)

---

##  Bug Reports
4 critical bugs were identified:
1. API crashes with `NULL` deposit → returns **500 Internal Server Error**.  
2. API accepts **boolean** as deposit → bypasses validation.  
3. API accepts **deposit below minimum (9.0)**.  
4. API allows **weak passwords (<6 characters)** during registration.  

Each bug report includes:
- **Steps to reproduce**  
- **Expected vs actual results**  
- **Severity & priority classification**

##  Learning Outcomes
- API test case design  
- Boundary and edge-case testing  
- Bug tracking & reporting workflow  
- Real-world API validation experience

