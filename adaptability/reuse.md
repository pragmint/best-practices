# Optimize for Reuse

Typically, the more an organization can leverage someone's previous efforts, the faster they'll be able to be able to reach their goals. As such, an organization's adaptability can be greatly influenced by their ability to optimize their current efforts for future reuse. On the flip-side, the [simplicity section](https://github.com/pragmint/best-practices/blob/main/adaptability/simplicity.md) of this repo details an acronym called YAGNI (You Ain't Gonna Need It). That's what happens when an organization gets carried away with this concept. When optimizing for reuse, it's important to balance short-term constraints without losing sight of long-term goals.

## Resources

- [Boundaries](https://www.destroyallsoftware.com/talks/boundaries) - Talk - builds the case for following the imperative shell / functional core pattern

### Encapsulation

- [Code examples on how to manage complexity with encapsulation](https://8thlight.com/blog/kevin-buchanan/2014/11/04/mistaking-encapsulation-for-abstraction.html)
- [Encapsulating behavior](https://github.com/97-things/97-things-every-programmer-should-know/tree/master/en/thing_32)

#### Law of Demeter

- [Introduction of Law of Demeter](https://dzone.com/articles/the-genius-of-the-law-of-demeter)
- [What it looks like when Law of Demeter is broken](https://www.youtube.com/watch?v=IU29HF6ZEJ4)
- [Temporal coupling and the Law of Demeter](https://practicingruby.com/articles/temporal-coupling-and-the-law-of-demeter)

#### Single Responsibility Principle

- [Introductory Blog](https://blog.cleancoder.com/uncle-bob/2014/05/08/SingleReponsibilityPrinciple.html)
- [Blog that introduces some nuance](https://qualitycoding.org/single-responsibility-principle/)
- [PDF of a Case Study showing SRP at the cloud architecture level](https://azure.microsoft.com/mediahandler/files/resourcefiles/e56cf87f-eb90-49bb-b40c-5c4247b7fa7c/Cloud-SOLID-The-single-responsibility-principle.pdf)
- [How SRP relates to DDD](https://dzone.com/articles/the-most-important-rule-in-software)
- [Meme](https://1.bp.blogspot.com/-UsdrVVdzhEk/UG21yvzLCHI/AAAAAAAAHd8/GsPSmsfGMP0/s320/Single+Responsibility+Principle.jpeg)
- [Functional code example](https://spin.atomicobject.com/2017/01/09/functions-single-responsibility-principle/)
- [Sandi Metz's talk on SOLID OOO](https://vimeo.com/12350535)

### Reusability / Configurability

- Drawbacks of reuse [perspective 1](https://github.com/97-things/97-things-every-programmer-should-know/tree/master/en/thing_07) and [perspective 2](http://www.bennorthrop.com/Essays/2018/the-reality-of-reuse.php)
- [DRY](https://github.com/97-things/97-things-every-programmer-should-know/tree/master/en/thing_30)
- [DRY can uncover performance bottlenecks](https://github.com/97-things/97-things-every-programmer-should-know/tree/master/en/thing_91)
- [CUPID - How properties can be more useful than principles](https://dannorth.net/2022/02/10/cupid-for-joyful-coding/)

#### Open / Closed Principle

- [Introductory Blog](https://blog.cleancoder.com/uncle-bob/2014/05/12/TheOpenClosedPrinciple.html)

#### Dependency Inversion Principle

- [Dependency Inversion Applied](https://www.martinfowler.com/articles/dipInTheWild.html)

### Cohesion

- [Singletons create coupling](https://github.com/97-things/97-things-every-programmer-should-know/tree/master/en/thing_73)

#### Interface Segregation Principle

- [Introductory Blog](https://reflectoring.io/interface-segregation-principle/)

### Microservices

- [When to use microservices, and when not to](https://www.youtube.com/watch?v=GBTdnfD6s5Q)
- [Entity service anti-pattern](https://www.michaelnygard.com/blog/2017/12/the-entity-service-antipattern/)
- [Services by lifecycle](https://www.michaelnygard.com/blog/2018/01/services-by-lifecycle/)
