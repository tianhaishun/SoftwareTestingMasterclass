# Software Testing Masterclass

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)

Master the skills of software testing with this comprehensive guide, designed for both beginners and experienced testers.

## Table of Contents

1. [Basics of Software Testing](#basics-of-software-testing)
    - [What is Software Testing?](#what-is-software-testing)
    - [Importance of Software Testing](#importance-of-software-testing)
    - [Types of Software Testing](#types-of-software-testing)
    - [Software Testing Life Cycle](#software-testing-life-cycle)
    - [Common Software Testing Techniques](#common-software-testing-techniques)
2. [Test Design Techniques](#test-design-techniques)
   - [Black-Box Testing Techniques](#black-box-testing-techniques)
   - [White-Box Testing Techniques](#white-box-testing-techniques)
   - [Grey-Box Testing Techniques](#grey-box-testing-techniques)
   - [Static vs Dynamic Testing](#static-vs-dynamic-testing)
   - [Manual vs Automated Testing](#manual-vs-automated-testing)
3. [Test Management](./TestManagement)
4. [Bug Tracking and Reporting](./BugTrackingAndReporting)
5. [Automation Testing](./AutomationTesting)
6. [Performance Testing](./PerformanceTesting)
7. [Security Testing](./SecurityTesting)
8. [Mobile Application Testing](./MobileApplicationTesting)
9. [Continuous Integration / Continuous Deployment](./ContinuousIntegrationContinuousDeployment)
10. [Soft Skills for Testers](./SoftSkillsForTesters)

## Introduction

This repository serves as a guide for aspiring software test engineers. It outlines the key skills and knowledge areas that are essential for a successful career in software testing. The contents are curated and regularly updated by industry experts.

## Update Plan

The contents of this repository are subject to regular updates based on the latest industry trends and advancements in software testing. The update frequency is planned as follows:

1. [Basics of Software Testing](./BasicsOfSoftwareTesting) - Updated Quarterly
2. [Test Design Techniques](./TestDesignTechniques) - Updated Bi-Annually
3. [Test Management](./TestManagement) - Updated Annually
4. [Bug Tracking and Reporting](./BugTrackingAndReporting) - Updated Bi-Annually
5. [Automation Testing](./AutomationTesting) - Updated Quarterly
6. [Performance Testing](./PerformanceTesting) - Updated Bi-Annually
7. [Security Testing](./SecurityTesting) - Updated Bi-Annually
8. [Mobile Application Testing](./MobileApplicationTesting) - Updated Annually
9. [Continuous Integration / Continuous Deployment](./ContinuousIntegrationContinuousDeployment) - Updated Quarterly
10. [Soft Skills for Testers](./SoftSkillsForTesters) - Updated Annually

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.



### Basics of Software Testing

#### What is Software Testing?

Software testing is a process that evaluates the functionality of a software application with an intent to find whether the developed software met the specified requirements or not and to identify the defects to ensure that the product is defect-free in order to produce a quality product.

##### Example

Consider a simple web form where a user needs to register by inputting their name, email, and password. Software testing in this case could involve:

- **Functional Testing**: Testing the functionality of the form, such as checking if a user can successfully register with valid inputs, or if the form correctly rejects invalid inputs (such as a malformed email or a too-short password).
- **Usability Testing**: Testing the form's user-friendliness, such as checking if the form is easy to understand and use, or if there are helpful error messages when the user makes a mistake.
- **Security Testing**: Testing the form for security vulnerabilities, such as checking if the password is being securely hashed and not just stored in plaintext.

##### Exercise

Find a web form (it could be a login form, a sign-up form, a contact form, etc.) and perform the above tests. Write down the steps you took, the test results, and any issues you found.
## Basics of Software Testing

### What is Software Testing?

Software testing is important because software bugs could be expensive or even dangerous. Software bugs can potentially cause monetary and human loss, and history is full of such examples.

##### Example

In 1996, a software bug in the Ariane 5 Flight 501 caused the rocket to self-destruct 37 seconds after launch, leading to a loss of more than $370 million. The bug was in the Inertial Reference System software, which was reused from the Ariane 4. The software tried to convert a 64-bit floating-point number to a 16-bit signed integer, but the number was too large, causing an overflow error. This incident highlights the importance of thorough software testing, especially when reusing existing software components.

##### Exercise

Research another real-world example of a costly or dangerous software bug. Write a brief report detailing what the bug was, what caused it, what the consequences were, and how it could have been prevented with better software testing.

### Importance of Software Testing

There are different stages for software testing process. The basic types of testing are: Functional Testing, Non-functional Testing, and Maintenance (Regression and Maintenance).

##### Example

Let's consider testing for a social media application like Instagram:

- **Functional Testing**: Testing the core functions of the app, like posting a picture, liking a post, or following a user.
- **Non-Functional Testing**: Testing non-functional aspects like app speed, load time, and user interface.
- **Maintenance**: After the software delivery, checking the modifications and updates in the application.

##### Exercise

Pick an application you use every day. Identify and write down at least one example for each type of testing: functional, non-functional, and maintenance.

### Software Testing Life Cycle

Software Testing Life Cycle (STLC) defines the steps/stages/phases in testing of software. However, there isn’t a fixed standard STLC in the world and it basically varies from one organization to another. The different stages in Software Testing Life Cycle are: Requirement Analysis, Test Planning, Test Case Development, Environment Setup, Test Execution, and Test Cycle Closure.

##### Example

Consider the development and testing of a new feature for a web application:

- **Requirement Analysis**: Business requirements are reviewed. Testability of the requirements is checked.
- **Test Planning**: Test strategy is defined. Estimation of testing effort is done.
- **Test Case Development**: Test cases and test scripts are created. Test data is generated.
- **Environment Setup**: Test environment setup is done.
- **Test Execution**: Test cases are executed.
- **Test Cycle Closure**: Testing is completed. Test metrics and test closure report are prepared.

##### Exercise

Think of a small feature or change you'd like to see in a software application you use regularly. Write down how you would go through each stage of the Software Testing Life Cycle for this feature or change.

### Common Software Testing Techniques

Software Testing Techniques help you design better test cases. They help identify test conditions that are otherwise hard to recognize. In this course, you will learn about the most commonly used software testing techniques.

##### Example

Suppose you're testing a simple calculator application. Some testing techniques you might use include:

- **Equivalence Partitioning**: If you're testing the calculator's addition function, you might identify "equivalence classes" of inputs to test, such as two positive numbers, a positive number and a negative number, two negative numbers, etc.
- **Boundary Value Analysis**: You might test the limits of the calculator's input range to see how it handles extremely large or small numbers.
- **Decision Table Testing**: You could create a table with different combinations of inputs and their expected outputs.

##### Exercise

Pick a simple software application or feature and write down how you would apply each of the above testing techniques.

---
## Test Design Techniques {#test-design-techniques}

### Black-Box Testing Techniques {#black-box-testing-techniques}

Black-box testing is a method of testing where the tester doesn't know the internal workings of the system. Testers only focus on the input and the output, not how the application processes data. Black-box testing primarily focuses on the functionality of the system.

Example
Let's consider a simple web form where a user needs to register by inputting their name, email, and password. In black-box testing, you would only test the functionality, such as checking if a user can successfully register with valid inputs, or if the form correctly rejects invalid inputs (such as a malformed email or a too-short password).

Exercise
Find a web form (it could be a login form, a sign-up form, a contact form, etc.) and perform black-box testing. Write down the steps you took, the test results, and any issues you found.

### White-Box Testing Techniques {#white-box-testing-techniques}

White-box testing is a method of testing where the tester knows the internal structure and implementation of the system. White-box testing primarily focuses on testing the program structure and internal paths.

Example
Consider a function in a program that calculates the factorial of a number. In white-box testing, you would test the function by providing various inputs and checking if the outputs are correct. You would also inspect the code to ensure that it correctly calculates the factorial and that there are no logical errors.

Exercise
Find a simple function or method in a program and perform white-box testing. Write down the steps you took, the test results, and any issues you found.

### Grey-Box Testing Techniques {#grey-box-testing-techniques}

Grey-box testing is a method of testing that is a blend of black-box and white-box testing. In grey-box testing, the tester has partial knowledge about the internal structure of the system.

Example
Consider a web application that you are testing. You have access to the database schema, but not the actual code of the application. You could perform grey-box testing by using the database schema to create tests that ensure data integrity, while also testing the functionality of the application as in black-box testing.

Exercise
Think of a scenario where you could perform grey-box testing. Describe the scenario, what you would test, and how you would test it.

### Static vs Dynamic Testing {#static-vs-dynamic-testing}

Static testing and dynamic testing are two different methods of testing. Static testing primarily focuses on the static structure of the program, such as code reviews or static code analysis. Dynamic testing focuses on the behavior of the program during runtime.

Example
Consider a program that you are developing. You could perform static testing by doing a code review and using a static code analysis tool like SonarQube. You could then perform dynamic testing by running the program and providing various inputs to check if the outputs are correct.

Exercise
Find a program or codebase and perform both static and dynamic testing. Write down the steps you took, the test results, and any issues you found.

### Manual vs Automated Testing {#manual-vs-automated-testing}

Manual testing and automated testing are two different methods of testing. Manual testing requires human effort, whereas automated testing uses tools or scripts to execute tests.

Example
Consider a web application that you are testing. You could perform manual testing by manually interacting with the application and checking if it behaves as expected. You could then perform automated testing by writing and running automated test scripts using a tool like Selenium.

Exercise
Think of a scenario where you could perform both manual and automated testing. Describe the scenario, what you would test, and how you would test it.

 
## Update Log

### Update 1 - 8-2-2023

Major update to the "Basics of Software Testing" module:

- Added detailed content for each of the five sub-courses: "What is Software Testing?", "Importance of Software Testing", "Types of Software Testing", "Software Testing Life Cycle", and "Common Software Testing Techniques".
- Each sub-course now includes an example and an exercise to help learners better understand the content and practice their learning.
- Added internal links in the "Table of Contents" section for easier navigation.

---
---

## Update Log

### Update 2 - 8-3-2023

Major update to the "Test Design Techniques" module:

- Added detailed content for each of the five sub-courses: "Black-Box Testing Techniques", "White-Box Testing Techniques", "Grey-Box Testing Techniques", "Static vs Dynamic Testing", and "Manual vs Automated Testing".
- Each sub-course now includes an example and an exercise to help learners better understand the content and practice their learning.
- Added internal links in the "Table of Contents" section for easier navigation.

---
