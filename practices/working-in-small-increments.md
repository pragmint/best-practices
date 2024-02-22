# Working in Small Increments

The practice of working in small increments involves making frequent, manageable changes to the codebase, facilitating easier tracking, quicker issue detection, and straightforward integration. It promotes continuous improvement, minimizes risks from large updates, and enhances collaboration. By breaking tasks into smaller pieces, development teams can ensure higher quality, consistent progress, and efficient adaptability.

## Nuance

### Misconception: More Commits Equals More Productivity
The belief that a higher frequency of commits directly correlates with increased productivity can be misleading. While working in small increments encourages regular updates, the focus should be on meaningful, self-contained changes that contribute to the project's progression. Simply pushing a high volume of minor changes without clear intent can lead to clutter in the version history and complicate project tracking.

### Overemphasis on Size Over Substance
Prioritizing the size of increments over the quality and relevance of the contribution can detract from the project's overall goals. It's crucial to ensure that each increment adds value and aligns with the project's objectives. Small, trivial changes that don't drive the project forward or improve its quality can waste valuable time and resources.

### Integration Challenges
While small increments facilitate easier integration and testing, they also require a robust continuous integration (CI) system to manage the frequent updates. Without efficient CI practices and tools in place, the benefits of working in small increments can be negated by integration delays and bottlenecks.

### Underestimating the Importance of Clear Commit Messages
Each small increment should be accompanied by a clear, descriptive commit message. This becomes even more critical when working in small increments, as the project history will contain a higher volume of updates. Neglecting this can lead to confusion and difficulties in understanding the purpose and impact of changes.

### Risk of Fragmentation
Working in excessively small increments can lead to fragmentation, where the codebase is peppered with incomplete features or changes that don't function well independently. This can make it difficult to maintain a clear direction for the project and may hinder the team's ability to deliver cohesive updates.

### Neglecting Long-Term Planning
Focusing too narrowly on small, immediate tasks can sometimes distract from the bigger picture and long-term objectives of the project. It's important to balance the benefits of incremental work with strategic planning to ensure that all efforts contribute meaningfully towards the project's overarching goals.

## Introspective Questions

### How Often Do You Commit?
How often do you commit changes to your codebase, and do you believe your current frequency optimally supports your project's goals and workflow?

### Are Your Increments Meaningful?
Are the increments you work on truly meaningful and contributing to the project, or are they simply small for the sake of being manageable?

### How Effective Is Your CI System?
How effectively does your current continuous integration (CI) system handle the frequency of updates from working in small increments, and where can improvements be made?

### How Clear Are Your Commit Messages?
Do your commit messages accurately and clearly convey the purpose and impact of each change, facilitating easier tracking and understanding of the project's evolution?

### Do You Maintain Project Cohesion?
Have you experienced any fragmentation in your project due to working in very small increments, and how do you ensure that each piece contributes to a coherent whole?

### Is Your Work Aligned With Long-Term Goals?
How do you maintain a balance between focusing on small, immediate tasks and ensuring that every effort aligns with and contributes to the long-term objectives of your project?

## Exercises

### Implement a Daily Commit Challenge
* **Objective:** Encourage developers to commit at least once a day with meaningful changes to foster the habit of working in small increments.
* **Outcome:** Increased familiarity with the practice, leading to a more consistent and manageable development process.

### Track and Analyze Commit Sizes
* **Objective:** Review the size and scope of commits over a period to assess whether the team is effectively balancing between too small and too large increments.
* **Outcome:** Insights into the optimal size for commits that balance manageability with meaningful contribution to the project.

### Continuous Integration (CI) Workflow Optimization
* **Objective:** Evaluate and improve the CI process to handle frequent updates more efficiently, including automating tests and deployment where possible.
* **Outcome:** A smoother, faster CI process that supports the practice without becoming a bottleneck.

### Commit Message Workshop
* **Objective:** Host a session to discuss and practice writing clear, descriptive commit messages that effectively communicate the intent and scope of changes.
* **Outcome:** Improved commit messages that facilitate better project tracking, understanding, and collaboration.

### Fragmentation Review
* **Objective:** Conduct a review of recent features or changes to identify instances of fragmentation due to excessively small increments.
* **Outcome:** Recommendations for combining or restructuring work to maintain project cohesion without sacrificing the benefits of small increments.

### Strategic Increment Planning Session
* **Objective:** Organize a planning session to align small increment work with long-term project goals, ensuring that each small task contributes to the bigger picture.
* **Outcome:** A clearer understanding of how daily work fits into long-term objectives, potentially leading to more strategic task allocation and prioritization.

## Resources

### [Know Your Next Commit](https://github.com/97-things/97-things-every-programmer-should-know/tree/master/en/thing_47#know-your-next-commit)
A guideline advocating for clarity and foresight in planning commits, emphasizing the practice of keeping changes small and manageable for streamlined development and easier troubleshooting.

### [An Argument Against PRs](https://www.youtube.com/watch?v=ZlLZEQQBcFg)
A video discussion that critiques the standard use of pull requests, arguing for a workflow that favors smaller, frequent updates to foster better collaboration and efficiency in software development.

### [Boy Scout Rule](https://github.com/97-things/97-things-every-programmer-should-know/tree/master/en/thing_08)
An approach to coding that urges developers to continually improve and clean up the codebase, making small, incremental enhancements with each commit, in line with the adage of leaving the code better than you found it.


## Related Practices

<!-- TODO: insert a list of [linked practices](/practices) that relate to this practice. For each item, give a brief explanation of how the linked practice supports / relates to this practice. Also categorize each linked practices as one of the following: Enables, Requires, Improves -->

## Supporting Capabilities

### [Continuous Integration](https://dora.dev/devops-capabilities/technical/continuous-integration/) #core
**Relationship:** Enables  
Working in small increments is foundational for effective continuous integration, allowing teams to integrate changes frequently, detect errors early, and maintain high quality and velocity.

### [Database Change Management](https://dora.dev/devops-capabilities/technical/database-change-management/) #core
**Relationship:** Improves  
Small, incremental changes facilitate smoother database updates and migrations, reducing the risk of disruptive errors and ensuring that database evolution aligns with application development.

### [Deployment Automation](https://dora.dev/devops-capabilities/technical/deployment-automation/) #core
**Relationship:** Enables  
The practice of working in small increments complements deployment automation by ensuring that changes are small enough to be deployed rapidly and reliably, enabling a continuous delivery pipeline.

### [Test Automation](https://dora.dev/devops-capabilities/technical/test-automation/) #core
**Relationship:** Improves  
Small, frequent commits make it easier to maintain a comprehensive suite of automated tests, as each change can be tested in isolation, improving test coverage and confidence in the codebase.

### [Trunk-Based Development](https://dora.dev/devops-capabilities/technical/trunk-based-development/) #core
**Relationship:** Requires  
Trunk-based development relies on developers working in small increments and merging their changes into the main branch frequently, minimizing divergence and promoting a more cohesive and stable codebase.

### [Streamlining Change Approval](https://dora.dev/devops-capabilities/process/streamlining-change-approval/) #core
**Relationship:** Enables  
By breaking work into smaller increments, teams can streamline the change approval process, as smaller changes are easier to review, understand, and validate, leading to quicker and more efficient approval cycles.

### [Working in Small Batches](https://dora.dev/devops-capabilities/process/working-in-small-batches/)
**Relationship:** Is synonymous with  
This capability is essentially what working in small increments is about—managing work in small batches to improve flow, reduce cycle times, and enhance feedback loops for continuous improvement.

### [Learning Culture](https://dora.dev/devops-capabilities/cultural/learning-culture/)
**Relationship:** Improves  
The practice of working in small increments fosters a learning culture by encouraging experimentation and rapid feedback on small changes, which supports continuous learning and adaptation within the team.

### [Generative Organizational Culture](https://dora.dev/devops-capabilities/cultural/generative-organizational-culture/) #core
**Relationship:** Improves  
Working in small increments can contribute to a generative culture by promoting transparency, collaboration, and high trust, as teams work closely together, share knowledge freely, and support each other in continuous improvement efforts.