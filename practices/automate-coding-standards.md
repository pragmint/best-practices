# Automate Coding Standards

Automate Coding Standards is a practice about maintaining a high level of code quality through automation.
It involves using tools to enforce coding standards and conventions automatically, ensuring that code is consistently formatted and adheres to predefined quality metrics.
This practice improves code readability, reduce errors and facilitates the code review process by catching issues early without human intervention.
It's a proactive approach to code quality, making it easier for teams to manage large code bases and collaborate effectively.

## Nuance

### Misconception: One-Size-Fits-All Approach
Automated coding standards are highly configurable, allowing customization to fit specific project needs.
It's a misconception that these tools enforce a rigid, universal standard across all projects.
Team members should have the opportunity to suggest changes to the coding standards and those suggested changes should be discussed as a team.
Strict adherence to automated standards without flexibility can stifle creativity.
It's important to balance between maintaining code quality and allowing developers the freedom to innovate.

### Tool Limitations
Automated tools may not catch every type of issue, particularly those related to complex logic or architecture.
Developers should be mindful of these limitations and not solely rely on these tools for ensuring code quality.

### Legacy Code Challenges
Incorporating automated coding standards tools into existing projects, especially large or legacy code-bases, can be challenging.
Lint rules and code fixes must be introduced in an incremental way.

### Development Workflow Integration
Automatic Coding Standards tools should be incorporated as part of the development process.
There are many options to do this: build scrips, IDE/Editors, pre-commit, pre-push, during code review/pull requests or Continuous Integration (CI Pipeline).
The specific approach to incorporate automatic coding standards as part of the development workflow will very depending on team preferences and the cost of running the process.

## How to Improve

### [Start A Book Club](/practices/start-a-book-club.md)

- [Automate Your Coding Standard](https://github.com/97-things/97-things-every-programmer-should-know/tree/master/en/thing_04)

This resource provides insights into the importance of automating coding standards to maintain code quality and consistency.
It highlights how automated tools can help enforce coding conventions, making the codebase more manageable and the development process more efficient.

- [One bite at a time](https://dev.to/christiankohler/one-bite-at-a-time-how-to-introduce-new-lint-rules-in-a-large-codebase-37ph)

This resource is about introducing new lint rules in a large legacy codebase.
It recommends a gradual approach, utilizing auto-fix capabilities wherever possible and manually addressing issues otherwise.
Also proposes secondary lint configuration for new rules, applied only to modified files via a pre-commit hook.
This method, inspired by the Boy Scout Rule of leaving code better than one found it.

### [Do A Spike](/practices/do-a-spike.md)

Implement what you learned in the article [Automate Your Coding Standard](https://github.com/97-things/97-things-every-programmer-should-know/tree/master/en/thing_04) with a project or module of your codebase.

### [Host A Roundtable Discussion](/practices/host-a-roundtable-discussion.md)

* Are our automated coding standards tools customized to reflect our specific coding practices and project needs, or are we using a one-size-fits-all approach?
* Do team members understand the reasons behind certain coding rules?

## Supporting Capabilities

### [Continuous Integration](https://dora.dev/devops-capabilities/technical/continuous-integration/)
Automating Coding Standards practice improves Continuous Integration by ensuring that code committed to the repository adheres to predefined quality and style guidelines, facilitating smoother integration and fewer integration issues.

### [Code Maintainability](https://dora.dev/devops-capabilities/technical/code-maintainability/)
This practice improves code maintainability by enforcing consistent coding standards across the codebase, making it easier to understand, modify, and extend the code over time.

### [Version Control](https://dora.dev/devops-capabilities/technical/version-control/)
The practice of Automated Coding Standards requires robust version control systems to track and manage the enforcement of coding standards over time, ensuring that all code changes are compliant.

### [Streamlining change approval](https://dora.dev/devops-capabilities/process/streamlining-change-approval/)
This automation reduces the need for extensive manual code reviews and oversight for style and basic issues, allowing teams to focus on more critical aspects of code quality and functionality during the review process.
