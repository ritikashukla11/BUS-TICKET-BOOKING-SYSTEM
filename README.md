# 🚌 Bus Ticket Booking System

A web-based Bus Ticket Booking System built using **Spring Boot**. Just like RedBus but simple — users can search buses, select seats and book tickets.

---

## 🛠️ Technologies Used

| Technology | Purpose |
|---|---|
| Spring Boot | Main framework — runs the whole application |
| Hibernate | Connects Java to MySQL database (ORM tool) |
| MySQL | Database — stores buses, tickets, users, seats |
| Thymeleaf | Frontend — dynamic web pages |
| Bootstrap | Makes the website look good and responsive |
| Lombok | Reduces boilerplate Java code |
| Maven | Manages all libraries and dependencies |

---

## 🏗️ Project Structure

```
src/main/java/
├── controller/    → handles all page requests
├── model/         → Bus, Ticket, User, Seat classes
├── service/       → business logic (check seats, book ticket)
└── repository/    → talks to MySQL database
src/main/resources/
├── templates/     → Thymeleaf HTML pages
└── application.properties → database config
```

---

## ⚙️ How MVC Works in This Project

- **Browser** → User searches for a bus (Delhi to Mumbai)
- **Controller** → Receives the request, passes to Service
- **Service** → Checks seat availability, applies business logic
- **Repository** → Fetches bus data from MySQL
- **Thymeleaf View** → Shows available buses on screen

---

## 🚀 How to Run

**Step 1 — Clone the project**
```bash
git clone https://github.com/ritikashukla11/BUS-TICKET-BOOKING-SYSTEM.git
cd BUS-TICKET-BOOKING-SYSTEM
```

**Step 2 — Configure database in `application.properties`**
```properties
spring.datasource.url=jdbc:mysql://localhost:3306/busticket?createDatabaseIfNotExist=true
spring.datasource.username=root
spring.datasource.password=your_password
spring.jpa.hibernate.ddl-auto=update
```

**Step 3 — Run the project**
```bash
mvn spring-boot:run
```

**Step 4 — Open in browser**
```
http://localhost:8080/index
```

---

## 📌 Features

- Search available buses by route
- Select seats
- Book tickets
- View booking details

---

## 👩‍💻 Developed By

**Ritika Shukla**
