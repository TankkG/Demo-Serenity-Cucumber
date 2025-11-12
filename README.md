# Serenity BDD with Cucumber and Java Framework

Serenity BDD (formerly known as Thucydides) is an open-source test automation framework that helps you write well-structured, maintainable acceptance criteria and automated tests. When combined with Cucumber (a BDD tool) and Java, it provides a powerful solution for behavior-driven development.

## Key Features

- **BDD Support**: Integrates with Cucumber to write tests in Gherkin syntax
- **Rich Reporting**: Generates detailed, narrative reports with screenshots
- **Web Testing**: Built-in support for Selenium WebDriver
- **Rest API Testing**: Includes support for REST-assured
- **Parallel Execution**: Supports running tests in parallel
- **Step Libraries**: Provides reusable step definitions for common actions

## Table of Contents
- [Project Overview](#project-overview)
- [Technology Stack](#technology-stack)
- [Setup Instructions](#setup-instructions)
- [Running Tests](#running-tests)
- [Reporting](#reporting)

## Project Overview
Automation framework for testing [Swag Labs](https://www.saucedemo.com/) demo e-commerce site using:
- Behavior-Driven Development (BDD) approach
- Page Object Model pattern
- Serenity's enhanced reporting capabilities

## Technology Stack
| Component      | Version |
|----------------|---------|
| Serenity BDD   | 4.2.22  |
| Cucumber       | 7.17.0  |
| JUnit          | 4.13.2  |
| Java           | 25      |
| Maven          | 3.9+    |

## Setup Instructions

### Prerequisites
1. Install JDK 25

```
choco install openjdk --version=25.0.0 -y
```

2. Install Maven 3.9.0

```
choco install maven --version=3.9.9 -y
```

3. Install Git

### Installation
```bash
git clone <repository-url>
mvn clean install
```

### Running Tests

Run all tests:
```
mvn clean verify
```

Run with specific browser:
```
mvn clean verify -Dwebdriver.driver=firefox
```

Run specific feature (Powershell):
```
mvn clean verify '-Dcucumber.filter.tags=@Login'
```

### Reporting
Serenity generates rich interactive reports located at:
```
target/site/serenity/index.html
```

Sample report includes:

-Test results dashboard
-Step-by-step screenshots
-Timing metrics
-Requirement coverage

