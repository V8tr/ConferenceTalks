
# Effective Unit Testing in Swift

## What attendees will learn

- Best practices of unit testing.
- Practical tips and tricks of unit testing in Swift.

## Target audience

This is not an introductory talk: I won't convince you why unit testing is important and how to write your first unit test.

Attendees will learn best practices and guidelines to write unit tests in Swift. These practices allow to reduce efforts on development and maintainance of tests suite and increase return on investment.

## Language

- Slides: English.  
- Talk: Russian.

## Content

### Problem Statement

- Poor test practices vs good test practices: the cost-benefit trade off.

### Unit testing best practices

- Key principle
- What makes a good unit test
  - Readable
  - Maintainable
  - Trustworthy
    
### Real-world unit testing in Swift

- Tech stack
  - Assertions: XCTest
  - Code generation: Sourcery
  - Network stubs: OHHTTPStub
- CI/CD
  - Never merge code with failing tests
  - Commit queue
  - Test reports
    - Detailed failure messages: use specialized assertions
    - Quality gate: maintain minimal code coverage of 85%. Reference to [Google approach](https://docs.google.com/presentation/d/1god5fDDd1aP6PwhPodOnAZSPpD80lqYDrHhuhyD7Tvg/edit#slide=id.g3f5c82004_99_130). 
- Controlling the world
  - Isolate system under test
    - Inject dependencies
    - Mock everything
    - Stub network
  - Control side effects
    - Identify warning flags
    - Cleanup in `setUp`, `tearDown`
  - Use patterns when testing concurrent code. (Wrote about them in [Unit Testing Asynchronous Code in Swift](https://www.vadimbulavin.com/unit-testing-async-code-in-swift/)).
    - Mocking
    - Signaling
    - Test before/test after
    - Busy assertion
- Test data
  - Use simplest possible input
  - Rotate data
  - Fixtures
- Avoid leaking test code into production
  - Do not weaken encapsulation
  - Do not put logic which is there only to support testing
