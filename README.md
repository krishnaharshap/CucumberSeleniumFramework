# Cucumber Selenium Framework

A robust Test Automation Framework built with **Java**, **Cucumber**, and **Selenium WebDriver** for efficient and maintainable web UI testing.

---

## Table of Contents

- [Overview](#overview)
- [Features](#features)
- [Tech Stack](#tech-stack)
- [Project Structure](#project-structure)
- [Getting Started](#getting-started)
- [Running the Tests](#running-the-tests)
- [Reporting](#reporting)
- [Contributing](#contributing)
- [License](#license)

---

## Overview

This framework leverages [Cucumber](https://cucumber.io/) for behavior-driven development, [Selenium WebDriver](https://www.selenium.dev/) for browser automation, and is designed for easy scalability, readability, and reusability. The project supports cross-browser testing and Gherkin-based feature files.

---

## Features

- **Behavior-Driven Development (BDD) with Cucumber**
- **Web Automation with Selenium WebDriver**
- **Gherkin Syntax for Test Scenarios**
- **Page Object Model (POM) Design Pattern**
- **Detailed HTML Test Reports**
- **Easy Configuration and Extensibility**
- **Support for Multiple Browsers**
- **CI/CD Friendly (GitHub Actions/Other CI tools)**

---

## Tech Stack

- **Java**
- **Cucumber**
- **Selenium WebDriver**
- **JUnit/TestNG** (specify which is used)
- **Gherkin**
- **Maven/Gradle** (specify which is used for build management)
- **JavaScript, CSS, HTML** (for reporting or test resources)

---

## Project Structure
. ├── src │ ├── main │ │ └── java │ └── test │ ├── java │ └── resources │ └── features ├── pom.xml / build.gradle ├── README.md └── ...


- `features/` — Gherkin feature files describing test scenarios
- `stepdefinitions/` — Step definitions mapping Gherkin steps to Java code
- `pages/` — Page Object Model classes
- `utils/` — Utility classes (helpers, drivers, etc.)
- `reports/` — Generated test reports

---

## Getting Started

### Prerequisites

- [Java JDK 8+](https://adoptopenjdk.net/)
- [Maven](https://maven.apache.org/) or [Gradle](https://gradle.org/) (as per project)
- [Git](https://git-scm.com/)
- A supported browser (Chrome, Firefox, etc.)

### Installation

1. **Clone the repository:**
   ```bash
   git clone https://github.com/krishnaharshap/CucumberSeleniumFramework.git
   cd CucumberSeleniumFramework
   ```

2.   **Install dependencies:**

## Running the Tests

**For Maven:**
`bash
mvn test`

**For Gradle:**
`bash
gradle test`

You can specify browser or environment via system properties (if supported):
```
bash
mvn test -Dbrowser=chrome
```

### Reporting
After execution, test reports (HTML/JSON) can be found in the target/cucumber-reports or build/reports directory. Open the HTML report in your browser to view detailed results.

## Contributing

Contributions are welcome! Please open an issue or submit a pull request.

1. Fork the repo
2. Create a new branch (`git checkout -b feature/your-feature`)
3. Commit your changes (`git commit -am 'Add new feature'`)
4. Push to the branch (`git push origin feature/your-feature`)
5. Create a new Pull Request

---

## License

This project is licensed under the [MIT License](LICENSE).

**Happy Testing!**

