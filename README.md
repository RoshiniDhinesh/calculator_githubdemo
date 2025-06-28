# Automation GitHub & Jenkins Demo (Java + TestNG)

This repository demonstrates a simple flow for automation testing using Java, TestNG, GitHub, and Jenkins.

## Structure
- `src/main/java`: Source application code (Calculator example)
- `src/test/java`: TestNG-based unit tests
- `Jenkinsfile`: Jenkins pipeline for CI

## Getting Started

1. Clone the repository:
   ```
   git clone https://github.com/RoshiniDhinesh/automation-github-jenkins-demo-java.git
   cd automation-github-jenkins-demo-java
   ```

2. Build and run tests locally:
   ```
   mvn clean test
   ```

## Jenkins Integration

- On Jenkins, create a Pipeline job and point it to this repository.
- The `Jenkinsfile` will build and test automatically on each commit.