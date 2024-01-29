# [Code Maintainability](https://dora.dev/devops-capabilities/technical/code-maintainability/)

Each time we write, edit, or read a line of code it costs an organization time and money. In the lifespan of a line of code, it will be written once, edited at least a handful of times, and read many times. As such, it makes sense to write code in a way that reduces the time required to comprehend it. Ideally, the software is built such that the reader can avoid needing to know how the whole system functions in order to make a local change. Furthermore, bugs are easier to spot when the surrounding code is easy to comprehend. The result of building code that's easy to maintain is more efficient delivery and better stability.

When difficult to maintain code is written, it can have a snowball effect. It requires an advanced set of skills to write maintainable code in a sea of hard to maintain code. Often, developers follow the path of least resistance by adding to the mess to get their new functionality added. There may be good reasons to follow such a path, however doing so further degrades the maintainability of the system. There is a delay between difficult to maintain code being introduced and the team experiencing a performance degradation. This delay makes it harder for non-technical team members to understand the consequences of implementing too many short-term solutions.

Following the practices below should yield software systems that are easier to maintain:

## SOLID Principles

The SOLID Principles are an acronym for the following:

- Single Responsibility
- Open / Closed
- Liskov Substitution
- Interface Segregation
- Dependency Inversion

Teams that understand and apply the SOLID Principles tend to write many small and focused abstractions that are skim-able, highly configurable, and easy to test. When new code gets written there tend to be fewer edits and more greenfield additions.

### Nuance

It is not always valuable to have fully SOLID compliant code. While most "violations" of SOLID point to worthy design problems, sometimes other factors are at play.

While originally designed for object oriented software, the SOLID Principles have adapted to other paradigms.

### Introspective Questions

- Does your codebase have large methods/functions?
- Assuming your codebase makes use of a framework, is there a lot of branching logic in your

### Resources

- [Dependency Inversion Applied](https://www.martinfowler.com/articles/dipInTheWild.html)
- [Blog that introduces some nuance](https://qualitycoding.org/single-responsibility-principle/)
- [PDF of a Case Study showing SRP at the cloud architecture level](https://azure.microsoft.com/mediahandler/files/resourcefiles/e56cf87f-eb90-49bb-b40c-5c4247b7fa7c/Cloud-SOLID-The-single-responsibility-principle.pdf)
- [How SRP relates to DDD](https://dzone.com/articles/the-most-important-rule-in-software)
- [Meme](https://1.bp.blogspot.com/-UsdrVVdzhEk/UG21yvzLCHI/AAAAAAAAHd8/GsPSmsfGMP0/s320/Single+Responsibility+Principle.jpeg)
- [Functional code example](https://spin.atomicobject.com/2017/01/09/functions-single-responsibility-principle/)
- [Sandi Metz's talk on SOLID OOO](https://vimeo.com/12350535)
- [CUPID](https://dannorth.net/cupid-for-joyful-coding/): An alternative to SOLID that focuses on foundational properties of well formed software instead of guiding principles. The author of CUPID was frustrated by some of the dogma that SOLID created and wanted a better way to articulate the nuance that each unique situation calls for.

### Exercises

## Imperative Shell / Functional Core

An imperative shell should read like a book. It should explicitly cover the high-level flow of an application and not get bogged down in the details.

A functional core should provide the complete context of how a low-level part of the system functions. It should be very detailed and focused in one area.

It's good practice to minimize the number of layers. Code gets complicated when there are a bunch of nested abstractions.

## Encapsulate Ideas

Don't scatter the logic for a thing across multiple abstractions.
"Email test" can you copy/paste a file and email it to someone, such that they can understand what's going on.
co-locate data and the behavior that modifies it

- [Code examples on how to manage complexity with encapsulation](https://8thlight.com/blog/kevin-buchanan/2014/11/04/mistaking-encapsulation-for-abstraction.html)
- [Encapsulating behavior](https://github.com/97-things/97-things-every-programmer-should-know/tree/master/en/thing_32)
- Drawbacks of reuse [perspective 1](https://github.com/97-things/97-things-every-programmer-should-know/tree/master/en/thing_07) and [perspective 2](http://www.bennorthrop.com/Essays/2018/the-reality-of-reuse.php)
- [DRY](https://github.com/97-things/97-things-every-programmer-should-know/tree/master/en/thing_30)
- [DRY can uncover performance bottlenecks](https://github.com/97-things/97-things-every-programmer-should-know/tree/master/en/thing_91)

## Measure & Manage Cyclomatic Complexity

https://jellyfish.co/library/cyclomatic-complexity/

## 4 Rules of Simple Design

## Transformation Priority Premise

Do the absolute simplest thing possible over and over again. Only introduce necessary complexity.
YAGNI

## Incremental Refactoring

Aka the boy scout rule. Leave the campsite cleaner than you found it.

## Enforce Coding Standard

Use linting to make style concerns consistent.
Use a resource like this to outline coding standards to get everyone on the same page. Build onboarding docs, training programs, community of practice, co-dev coaching playbooks, etc all off of a resource like this.

## Bookmarking

Use a placeholder name, mark a todo, add a pre-commit hook to search for todos so nothing slips, will be easier to name after you build the thing a bit. https://stackoverflow.com/questions/7291186/git-warn-before-committing-if-string-appears-in-source-or-diff/7292992#7292992

## Related Capabilities

- [Documentation Quality](/process/documentation-quality.md): Well documented code helps readers understand the high level concepts at play in the codebase.
- [Test Automation](/tech/test-automation.md): When code is well covered in automated tests, it reduces the risk of making a change. Developers can refactor with confidence when there is a high quality suite of automated tests covering the code they're altering. Furthermore, techniques like test-driven development and the transformation priority premise can increase the simplicity of code, thus making it easier to maintain.
- [Monitoring and Observability](/tech/monitoring-and-observability.md): For reasons similar to test automation, having great monitoring and observability creates a safety net that gives developers confidence to make changes to a codebase.
- [Version Control](/tech/version-control.md): When it's really easy to rollback changes to a previous version of code, state, infrastructure, etc, the time required to fix issues gets reduced to almost zero.
- [Loosely Coupled Architecture](/tech/loosely-coupled-architecture.md): Just like in code, when architectural abstractions are well-formed, it becomes easier to alter the system.
- [Streamline Change Approval](/process/streamline-change-approval.md): Following practices that streamline change approval, like pair programming, reduces the friction on incorporating new changes. Thus, it's less costly to refactor the code, which can lead to higher code maintainability.
- [How to Empower Software Delivery Teams as a Business Leader](/culture/how-to-empower-software-delivery-teams-as-a-business-leader.md): Code is a reflection of the conversations a team is having. If teams are well formed and having productive conversations, the code will likely reflect that and be easier to maintain as a result.








### Nuance

### Introspective Questions

### Resources

### Exercises
