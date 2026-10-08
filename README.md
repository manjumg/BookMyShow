# BookMyShow

A movie-ticket booking application built using **Java, Spring Boot, and MySQL**.

## 🚀 Technologies Used

* Java 17
* Spring Boot 3.2.1
* Maven
* MySQL
* Spring Data JPA
* Hibernate
* Swagger UI for API documentation

## 📋 Prerequisites

Make sure you have the following installed:

* JDK 17
* MySQL Server
* Git
* IntelliJ IDEA (recommended)

## ⚙️ Configuration

The application connects to a local MySQL database named `cinemaDb`.

Configure the following environment variables before running the application:

| Variable        | Description                                |
| --------------- | ------------------------------------------ |
| `DB_USERNAME`   | MySQL username                             |
| `DB_PASSWORD`   | MySQL password                             |
| `MAIL_USERNAME` | Gmail address for email functionality      |
| `MAIL_PASSWORD` | Gmail app password for email functionality |

**Important:** Never commit real passwords or other sensitive credentials to GitHub.

## 🛠️ Installation and Setup

### 1. Clone the repository

```bash
git clone https://github.com/manjumg/BookMyShow.git
```

### 2. Navigate to the project directory

```bash
cd BookMyShow
```

### 3. Configure the environment

Set the required environment variables in IntelliJ IDEA under **Run → Edit Configurations → Environment variables**.

Ensure MySQL is running locally.

### 4. Run the application

On Windows, use PowerShell:

```powershell
.\mvnw.cmd spring-boot:run
```

Alternatively, open the project in IntelliJ IDEA and run `BookMyShowApplication`.

## 📖 API Documentation

After the application starts successfully, open Swagger UI:

http://localhost:8080/swagger-ui/index.html

Use the Swagger interface to explore the API endpoints available in the application.

## 🗄️ Database Configuration

The application uses MySQL with the following database URL:

```text
jdbc:mysql://localhost:3306/cinemaDb?createDatabaseIfNotExist=true
```

Hibernate is configured with `spring.jpa.hibernate.ddl-auto=update`.

## 📁 Project Structure

```text
BookMyShow/
├── .mvn/
├── src/
│   ├── main/
│   │   ├── java/
│   │   └── resources/
│   │       └── application.properties
│   └── test/
├── mvnw
├── mvnw.cmd
├── pom.xml
├── .gitignore
└── README.md
```

## 🔐 Security

* Store credentials in environment variables.
* Do not upload passwords, API keys, or Gmail app passwords to GitHub.
* Rotate any credentials that have been accidentally exposed.

## 👨‍💻 Author

**GitHub:** [manjumg](https://github.com/manjumg)

## 📄 License

No license has been specified for this project yet.
