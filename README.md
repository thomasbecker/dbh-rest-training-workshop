# DBH REST API Training - Workshop Materials

This repository contains the starter code and exercise instructions for the
2-day REST API training.

## Prerequisites

- Java 8 (required)
- Gradle 6.x or higher
- Your favorite IDE (IntelliJ IDEA, Eclipse, VS Code)
- Postman or curl for API testing

## Getting Started

1. Clone this repository:

```bash
git clone https://github.com/thomasbecker/dbh-rest-training-workshop.git
cd dbh-rest-training-workshop
```

1. Navigate to the starter-project:

```bash
cd starter-project
```

1. Build the project:

```bash
./gradlew build
```

1. Run the application:

```bash
./gradlew run
```

The API will be available at `http://localhost:8080/api`

## Project Structure

```
dbh-rest-training-workshop/
├── starter-project/          # Your working directory with TODO markers
│   ├── src/main/java/       # Source code
│   ├── src/test/java/       # Test files
│   └── build.gradle         # Dependencies
└── exercises/               # Exercise instructions
    ├── 01-rest-basics/      # REST fundamentals exercise
    ├── 02-jersey-setup/     # Jersey setup exercise
    ├── 03-jersey-crud/      # CRUD implementation
    ├── 04-bean-validation/  # Validation exercise
    ├── 05-api-versioning/   # Versioning exercise
    ├── 08-security-implementation/ # Security exercise
    └── 09-comprehensive-todo/      # Final capstone exercise
```

## Exercise Instructions

Each exercise folder contains a README.md with:

- Learning objectives
- Step-by-step instructions
- Hints and tips
- Test commands
- Common pitfalls to avoid

Work through the exercises in order, as they build upon each other.

## Test-Driven Development

Tests are provided for each exercise. Run them with:

```bash
./gradlew test
```

For a specific test:

```bash
./gradlew test --tests UserResourceTest
```

## Useful Commands

```bash
# Build the project
./gradlew build

# Run the application
./gradlew run

# Run all tests
./gradlew test

# Clean build artifacts
./gradlew clean

# Check Java version
java -version
```

## API Testing

Once the server is running, test your endpoints:

```bash
# GET all users
curl http://localhost:8080/api/users

# GET specific user
curl http://localhost:8080/api/users/1

# POST new user
curl -X POST http://localhost:8080/api/users \
  -H "Content-Type: application/json" \
  -d '{"username":"john","email":"john@example.com"}'
```

## Technology Stack

- **Java 8** - Programming language
- **Jersey 2.35** - JAX-RS implementation
- **Jackson 2.14** - JSON processing
- **Jetty** - Embedded server
- **JUnit 5** - Testing framework
- **REST Assured** - API testing

## Tips for Success

1. **Read the TODOs**: Look for TODO markers in the code
2. **Run tests frequently**: Use TDD approach
3. **Check the exercise README**: Detailed instructions are provided
4. **Ask questions**: Don't hesitate to ask for help
5. **Commit often**: Save your progress regularly

## Related Repositories

- Slides:
  [dbh-rest-training-slides](https://github.com/thomasbecker/dbh-rest-training-slides)
  (Available after training) - Solutions:
  [dbh-rest-training-solutions](https://github.com/thomasbecker/dbh-rest-training-solutions)
  (Available after training)

## Support

During the training, ask your instructor for help. After the training, refer to
the solutions repository.

## License
