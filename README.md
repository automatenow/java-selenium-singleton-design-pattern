# Java Selenium Singleton Design Pattern Demo

This repository was created by [Marco A. Cruz](http://www.linkedin.com/in/marco-a-cruz) and is designed to be an introduction to using the Singleton Design Patter in a Selenium 
WebDriver test automation framework.

**Learn more about Singleton in our [Java Singleton video tutorial](https://www.youtube.com/watch?v=C_LPMGSX2rU&t)** and 
[Singleton blog post](https://testomat.io/blog/singleton-design-pattern-how-to-use-it-in-test-automation/).

## Overview

This repository demonstrates the Singleton Design Pattern specifically tailored for managing a single Selenium WebDriver instance in a Java Selenium automation framework. 
The Singleton pattern ensures that only one instance of WebDriver is created, which is particularly useful for:

- Reducing resource consumption by avoiding multiple browser sessions
- Ensuring consistent state across tests when using a shared driver
- Simplifying test setup and teardown processes

### What is the Singleton Pattern?

- **Intent**: Ensure a class (in this case, WebDriver) has only one instance, and provide a global point of access to it.
- **Use Cases in Selenium**:
    - Managing a single browser instance for all tests.
    - Centralizing WebDriver configuration and management.

### Why Use Singleton for WebDriver?

- **Resource Management**: One WebDriver instance means fewer resources are used, which is beneficial for local development or CI environments.
- **State Management**: Ensures all tests interact with the same browser state, reducing setup complexity.
- **Lazy Initialization**: The WebDriver can be initialized only when first needed, optimizing test run times.

## Implementation

This repository contains:

- **Driver.java**: A Singleton implementation for Selenium WebDriver.
- **TestBrowserNav.java**: A few sample tests showing how to use the Singleton WebDriver.

### How to Run

1. Clone the repository
Ensure you have the necessary Selenium dependencies in your `pom.xml` or `build.gradle`, then compile and run:

```
git clone https://github.com/automatenow/java-singleton-design-pattern.git
cd java-singleton-design-pattern
```

2. Build the Project<br/>
```mvn clean install```

3. Use your favorite IDE to run the tests.

## License
This project is licensed under the MIT License - see the LICENSE file for details.

## About automateNow
[automateNow](https://automatenow.io/) is a leading learning platform catering to the needs of software testers. We are dedicated to empowering testers with the necessary skills and resources to excel in test automation and beyond.
