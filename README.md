# Assistant — Task Management Application

## Overview

**Assistant** is a desktop task management application developed in Java using JavaFX and FXML. It allows users to organize and manage their tasks, categorize them, set priorities and deadlines, create reminders, and monitor their progress through a graphical user interface.

The application was developed as an academic project using IntelliJ IDEA and Maven.

## Features

### Task Management
- Create, edit, and delete tasks.
- Store task details, including title, description, category, priority, deadline, and completion status.
- View and manage tasks through data tables.
- Edit table cells by double-clicking a cell, modifying its value, and pressing Enter.
- Delete a selected task using the corresponding button.

### Categories and Priorities
- Organize tasks into categories.
- Assign priority levels to tasks.
- Use categories and priorities to organize and search for tasks.

### Search and Filtering
- Search for tasks by title, category, or priority.
- Combine search criteria to find specific tasks more easily.

### Reminders
- Create and manage reminders.
- Store reminder titles, dates, and activation status.

### Dashboard
- View an overview of task-related information.
- Display a pop-up notification showing the exact number of overdue tasks that have not been completed.

### Graphical User Interface
- Built with JavaFX and FXML.
- Provides separate screens for the application's main functions.
- Supports navigation between screens and interaction through buttons and editable tables.

## Technologies Used

- **Java 23** — Core programming language.
- **JavaFX 23.0.1** — Graphical user interface.
- **FXML** — User interface layout and structure.
- **Maven** — Dependency management and project build configuration.
- **JSON** — Data storage.
- **Gson** — JSON processing.
- **Jackson Databind** — JSON serialization and deserialization.
- **Jackson JSR310** — Support for Java date and time types.
- **org.json** — JSON manipulation.
- **JUnit 5** — Unit testing.

## Project Structure

The project follows a Maven-based structure.

```text
Assistant/
├── pom.xml
├── README.md
└── src/
    └── main/
        ├── java/
        │   └── ece/
        │       └── medialabassistant/
        │           └── assistant/
        │               ├── Controllers/
        │               ├── myObjects/
        │               ├── Loaders/
        │               ├── medialab/
        │               │   ├── tasks.json
        │               │   ├── categories.json
        │               │   ├── priorities.json
        │               │   └── reminders.json
        │               ├── DataManager.java
        │               └── Main.java
        └── resources/
            └── *.fxml
```

*Note: The structure above is illustrative. The actual contents may vary depending on the files included in the project.*

## Data Storage

The application uses JSON files to store task-related information.

The JSON files are located in:

```text
src/main/java/ece/medialabassistant/assistant/medialab/
```

The data files include:

- `tasks.json` — Task information.
- `categories.json` — Available task categories.
- `priorities.json` — Priority information.
- `reminders.json` — Reminder information.

The application uses its data management and loading classes to handle stored information.

## Getting Started

### Prerequisites

Make sure the following are installed:

- Java Development Kit (JDK) 23.
- Apache Maven.
- IntelliJ IDEA or another Java-compatible IDE.

### Running the Application in IntelliJ IDEA

1. Open the project in IntelliJ IDEA.
2. Make sure the project uses JDK 23.
3. Load or reload the Maven configuration.
4. Locate the `Main.java` class.
5. Run the application's main method.

### Running the Application with Maven

1. Open a terminal in the project's root directory, where the `pom.xml` file is located.
2. Execute:

```bash
mvn javafx:run
```

Maven will resolve the configured dependencies and launch the JavaFX application.

## Documentation

Javadoc documentation was prepared for the `Category` class to describe its purpose and implementation.

## Author

Developed as an academic project.
