# Unit Testing Asynchronous Code

## What to learn

Attendees will learn 4 practical techniques of unit testing async code, that will make unit tests more maintainable, readable and robust.

## Target audience

This is not an introductory talk. I won't convince you why unit testing is important and how to write your first unit test. I mainly target Middle / Senior / Lead Engineers with hands-one experience in unit testing. Examples will be in Swift and `XCTest` framework, however the principles apply generally to all languages and test frameworks.

## Language

- Slides: English
- Talk: Russian

## Content

- Why unit testing async code is hard
- Mocking async dependencies with sync
  - Brief overview of related techniques
    - Dependency injection
    - Mocking
  - Technique overview
  - Example
- Signaling
  - Overview
  - Signaling with `XCTestExpectation`
  - Example
    - Regular `XCTestExpectation`
    - Inverted `XCTestExpectation`
- Test before & test after
  - Overview
    - Testing preconditions
    - Testing postconditions
  - Example
- Busy assertion
  - Overview
  - Extending `XCTest` with custom expectation
  - Example
    - Regular busy assertion
    - Inverted busy assertion
- Summary
  - Overview of 4 techniques
  - When to use what
- Q&A
