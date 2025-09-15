# Cucumber Selenium Framework

A robust, scalable, and modular automation framework leveraging **Cucumber** for BDD and **Selenium WebDriver** for browser automation. This project is designed for rapid test development, easy maintenance, and seamless integration into CI/CD pipelines.

## Features

- **Behavior-Driven Development (BDD)**: Write human-readable test scenarios using Gherkin syntax.
- **Modular Page Object Model (POM)**: Clean separation of test logic and UI interactions.
- **Cross-Browser Testing**: Easily extendable to run tests on Chrome, Firefox, Edge, etc.
- **Test Data Management**: Supports external test data sources (Excel, CSV, JSON).
- **Advanced Reporting**: Integrated with reporting tools (ExtentReports, Allure, etc.).
- **Parallel Execution**: Supports running tests in parallel using TestNG/JUnit.
- **CI/CD Integration**: Ready for GitHub Actions, Jenkins, Azure DevOps, etc.

## Project Structure

```
CucumberSeleniumFramework/
├── src/
│   ├── main/
│   │   └── java/
│   │       └── com/
│   │           └── yourcompany/
│   │               └── pages/
│   │               └── utils/
│   ├── test/
│   │   └── java/
│   │       └── stepdefinitions/
│   └── resources/
│       └── features/
│       └── config/
├── pom.xml
├── README.md
```

- **features/**: Contains `.feature` files written in Gherkin.
- **stepdefinitions/**: Glue code to connect Gherkin steps with Selenium actions.
- **pages/**: Page Object classes for different web pages.
- **utils/**: Utilities, hooks, drivers, data providers, etc.

## Setup & Installation

### Prerequisites

- Java 8+
- Maven or Gradle
- Chrome/Firefox/Edge browsers
- IDE (IntelliJ, Eclipse, VS Code)

### Cloning the Repository

```bash
git clone https://github.com/krishnaharshap/CucumberSeleniumFramework.git
cd CucumberSeleniumFramework
```

### Installing Dependencies

```bash
mvn clean install
```
_or_
```bash
gradle build
```

### Configuration

- Update browser and environment settings in `/src/test/resources/config/config.properties`.
- Add/modify feature files in `/src/test/resources/features/`.

## Running Tests

### Using Maven

```bash
mvn test
```

### Using Gradle

```bash
gradle test
```

### Running Specific Feature

```bash
mvn test -Dcucumber.options="src/test/resources/features/Login.feature"
```

## Reporting

- After test execution, reports are generated in the `/target` folder.
- For Allure reports:
  ```bash
  allure serve target/allure-results
  ```

## Contribution Guidelines

1. Fork the repository.
2. Create a feature branch.
3. Make changes and commit.
4. Push to your fork.
5. Open a Pull Request describing your changes.

## Best Practices

- Follow the Page Object Model for maintainability.
- Write reusable step definitions.
- Keep feature files concise and descriptive.
- Use hooks for setup and teardown logic.
- Document new features and utilities.

## Troubleshooting

- Ensure browser drivers are up to date and compatible with your browser version.
- Check `config.properties` for correct environment URLs and credentials.
- Review logs in `/target` for error details.

## Credits

- [SeleniumHQ](https://www.selenium.dev/)
- [Cucumber](https://cucumber.io/)
- [Original Author - naveenanimation20](https://github.com/naveenanimation20/CucumberSeleniumFramework)
