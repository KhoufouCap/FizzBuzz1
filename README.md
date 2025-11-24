# FizzBuzz Game

A Java 21 Maven project implementing the FizzBuzz game using BDD methodology with Cucumber.

## Rules

- If the number is a multiple of 3, return "Fizz"
- If the number is a multiple of 5, return "Buzz"
- If the number is a multiple of both 3 and 5, return "FizzBuzz"
- Otherwise, return the number itself as a string

## Project Structure

```
FizzBuzz1/
├── src/
│   ├── main/
│   │   └── java/
│   │       └── com/
│   │           └── fizzbuzz/
│   │               ├── FizzBuzz.java      # Main game logic
│   │               └── Main.java          # Application entry point
│   └── test/
│       ├── java/
│       │   └── com/
│       │       └── fizzbuzz/
│       │           ├── RunCucumberTest.java   # Cucumber test runner
│       │           └── FizzBuzzSteps.java     # Step definitions
│       └── resources/
│           └── features/                      # Gherkin feature files
├── pom.xml
└── README.md
```

## Building and Running

### Build the project
```bash
mvn clean install
```

### Run the application
```bash
mvn exec:java -Dexec.mainClass="com.fizzbuzz.Main"
```

### Run tests
```bash
mvn test
```

## Next Steps

- Create Gherkin feature files in `src/test/resources/features/`
- Implement the FizzBuzz logic based on BDD scenarios
