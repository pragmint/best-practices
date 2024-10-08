# Build a Consistent Testing Strategy

Building a consistent testing strategy involves matching your approach to the specific needs of your project and considering the influence of your technology stack.
Prioritize testing critical and complex code areas, and select appropriate types of tests, such as unit, integration, and end-to-end tests.
Balance the proportion of each test type, favoring more unit tests and fewer high-cost tests like end-to-end tests.
Ensure comprehensive test coverage for new and modified code by including tests in the definition of done and verifying them during code reviews.
Manage expensive tests by regularly reviewing, deleting, and replacing them with more efficient alternatives.
Integrate tests into the continuous integration pipeline and spread knowledge of the testing strategy and best practices among the development team.

## Nuance

### One-Size-Fits-All Testing Strategy

A common misconception is that a single testing strategy can be applied to all projects.
In reality, each project has unique requirements and constraints, which means that the testing strategy must be customized accordingly.
Factors such as project size, complexity, technology stack, and team expertise influence the choice of testing tools, frameworks, and the balance of different test types.

### Balancing Test Coverage and Maintenance

While comprehensive test coverage is important, it is equally important to balance it with the maintainability of tests.
Over-ambitious coverage goals can lead to a large test suite that is difficult to maintain and slows down the development process.
Focus on covering critical paths and high-risk areas thoroughly, and ensure that tests are easy to update as the codebase evolves.
Regularly refactor tests to keep them relevant and maintainable.

### Excessive End-to-End Testing

End-to-end tests are important for verifying the complete functionality of an application, but they are also resource-intensive and time-consuming.
Relying too heavily on end-to-end tests can slow down the continuous integration pipeline and make the testing process less efficient.
Additionally, end-to-end tests are prone to flakiness due to their reliance on multiple integrated components and external dependencies.
When these tests fail intermittently, it can be challenging to pinpoint the exact cause, leading to wasted time investigating false negatives or non-reproducible issues.
To mitigate these challenges, it's advisable to tests with more targeted unit and integration tests that provide faster feedback on specific code functionalities, reducing the overall dependency on end-to-end testing.

### Manual Testing is Obsolete

With the rise of automation, there is a misconception that manual testing is no longer necessary. However, manual exploratory testing plays a critical role in identifying unexpected issues and usability problems that automated tests might miss. Manual testers bring human intuition and creativity to the testing process, uncovering edge cases and user experience issues that automated scripts cannot replicate.

## How to Improve

### [Host A Roundtable Discussion](/practices/host-a-roundtable-discussion.md)

#### Evaluate Current Testing Strategy

Schedule a team meeting to review your current testing strategy.
Analyze your existing practices, tools, and processes.
Document the strengths, weaknesses, and any gaps in your approach.
Discuss potential improvements and prioritize them based on impact and feasibility.
After implementing changes, reassess after a few sprints to measure improvements in bug detection and code quality.

<!-- workshop  -->

### [Lead a Workshop](/practices/lead-a-workshop.md)

#### Develop a Testing Strategy Document

Create a detailed testing strategy document that outlines your project's specific testing needs. Include information on test types, coverage goals, and maintenance practices.
Share this document with your team and solicit feedback.
Implement the strategy and monitor its impact on your testing process and overall code quality.

#### Balance Your Test Pyramid

Analyze your current distribution of unit, integration, and end-to-end tests.
Compare it to the ideal test pyramid, which suggests having more unit tests, fewer integration tests, and even fewer end-to-end tests.
Adjust your test suite to better align with this model, and observe changes in test execution times and reliability.

#### Integrate Tests into Continuous Integration (CI) Pipeline

If not already done, integrate your tests into the CI pipeline.
Ensure that all tests run automatically on each code commit.

#### Conduct Manual Exploratory Testing Sessions

Schedule regular manual exploratory testing sessions where team members test the application without predefined scripts.
Focus on uncovering usability issues and edge cases.
Compare the issues found through these sessions with those found through automated testing to understand the value added by manual exploration.

### [Run Pair Programming Sessions](/practices/run-pair-programming-sessions.md)

### Share and Educate Testing Best Practices

Organize workshops or knowledge-sharing sessions where team members can learn about and discuss testing best practices.
Encourage the team to share their experiences and tips.
Track how this knowledge transfer impacts the quality and consistency of your testing efforts.

### [Host A Roundtable Discussion](/practices/host-a-roundtable-discussion.md)

#### Tailoring Your Testing Strategy

* How well does your current testing strategy align with the specific needs and constraints of your project?
* What unique aspects of your project (e.g., technology stack, team expertise) might require a different testing approach?

#### Balancing Test Coverage and Maintenance

* How often do you refactor your tests to ensure they remain relevant and maintainable as your codebase evolves?
* How do you currently handle resource-intensive and time-consuming tests, such as end-to-end tests?
* Are there opportunities to replace some of these expensive tests with more efficient alternatives?

#### Integrating Manual Testing

* Have you considered the role of manual exploratory testing in your overall strategy?
* How can you use the creativity and intuition of manual testers to uncover issues automated tests might miss?

#### Continuous Integration and Testing

* How well integrated are your tests into your continuous integration pipeline?
* Are your tests providing timely and reliable feedback during the development process?

#### Spreading Testing Knowledge

* How effectively is your testing strategy and best practices communicated and shared within your development team?
* What steps can you take to ensure everyone on the team understands and follows the testing strategy?

## Supporting Capabilities

### [Test Automation](/capabilities/test-automation.md)

Building a Consistent Testing Strategy supports the Test Automation capability by providing a structured approach to testing that aligns with project needs.
It emphasizes balanced test coverage, integrates tests into CI pipelines for fast feedback, and combines automated and manual testing to ensure comprehensive quality and stability of software delivery.