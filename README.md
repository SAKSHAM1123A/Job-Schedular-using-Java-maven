# Chronos — Job Scheduler

A Java-based desktop job scheduler with a graphical user interface, priority-based execution, delayed jobs, and persistent storage using SQLite.

## Overview

Chronos is a desktop application designed to schedule and manage jobs with different priorities and execution delays.

The application provides a dashboard to monitor jobs, manage pending tasks, and track completed or failed executions.

## Features

- Create and schedule jobs with configurable delays.
- Assign job priorities: LOW, NORMAL, HIGH, and URGENT.
- Execute jobs using a priority-aware scheduling queue.
- Run jobs immediately.
- Cancel pending jobs.
- Delete selected jobs.
- Search and filter jobs.
- View job statuses and activity logs.
- Store jobs locally using SQLite.
- Restore pending jobs after restarting the application.

## Tech Stack

| Technology | Purpose |
|---|---|
| Java 21 | Core application |
| Java Swing | Desktop GUI |
| Maven | Build and dependency management |
| SQLite | Persistent local storage |
| JUnit 5 | Unit testing |

## Requirements

- JDK 21 or later
- Maven 3.8 or later

Check your installed versions:

```bash
java -version
mvn -version
```

## Getting Started

### 1. Clone the repository

```bash
git clone https://github.com/YOUR_USERNAME/Chronos.git
```

### 2. Open the project

```bash
cd Chronos
cd "Java project job schedular"
```

### 3. Build the application

```bash
mvn clean compile
```

### 4. Run the application

```bash
mvn exec:java
```

## Database

Chronos uses SQLite for local persistence.

The database stores job information and activity logs. It is created automatically when the application runs.

The database schema is available in:

`src/main/resources/schema.sql`

No external database server is required.

## Testing

Run the test suite using:

```bash
mvn test
```

## Project Structure

```text
Chronos/
├── .gitignore
├── README.md
└── Java project job schedular/
    ├── pom.xml
    └── src/
        ├── main/
        │   ├── java/
        │   └── resources/
        └── test/
            └── java/
```

## Future Improvements

- Support for recurring jobs.
- Configurable execution threads.
- Job execution history and analytics.
- Export and import scheduled jobs.
- More advanced scheduling options.

## Author

Developed as a Java desktop application project.

## License

This project is licensed under the MIT License.
