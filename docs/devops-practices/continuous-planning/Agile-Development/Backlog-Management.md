# Backlog Management

## What is Backlog Management

Backlog management is the process by which the product owner (often in collaboration with others) adds, adjusts, grooms, and prioritizes backlog items within the backlog to make sure the most valuable product is shipped to customers. An oversized product backlog is a problem that indicates the team have either taken on too much work or they have other challenges that need addressing.

Backlog management can be broken down into the following sub-sections:

- [Backlog Refinement](#backlog-refinement)
- [Minimal Slices](#minimalism-slices)
- [External Feedback](#external-feedback)

------

## Backlog Refinement

### Goals

_What are the intended outcomes of the ceremonies?_

[Backlog refinement](https://www.agilealliance.org/glossary/backlog-refinement) is when the [product owner](https://www.agilealliance.org/glossary/product-owner/) and some, or all, of the rest of the team review items on the backlog to ensure the backlog contains the appropriate items, that they are prioritized, and that the items at the top of the backlog are ready for development. This activity occurs on a regular basis and may be an officially scheduled meeting or an ongoing activity.

### Participation

_What members of the team should participate?_

Ideally all the team members could participate. This is an ongoing process in which the Product Owner and the Development Team collaborate on the details of Product Backlog items.

### Impact

_What positive impact has been observed as a result of this practice?_

The intent of backlog refinement is to ensure that the backlog keeps updating with items that are appropriate to their priority, i.e. higher priority items are with more details than lower priority ones. Also, it is important that at any time there are enough user stories ready for planning in the next or even, where reasonable, the next two or three iterations but not too much further.

### Measures

_How might one measure the impact of this ceremony positive or negative?_

The expected outcome from the backlog refinement is all the team members are on the same page of what they are going to implement in the next or next few iterations with priority. A positive outcome of refinement is one where each backlog item can reasonably be “done” within the sprint time. Product backlog items that can be “done” by the development team within one sprint are deemed “ready” for selection in a sprint planning.

### Facilitation Guidance

_How might one go about running the ceremony? Is there a general pattern that the ceremony should follow?_

- Product Owner: presents the ordered backlog and backlog list they'd like in the next iteration.
- Process Lead: ensure the timebox.
- Team members: ask questions and request additional details on the backlog if needed.

Make sure that the team does not focus on how to implement the items. Instead, the Product Owner and Team discuss the goals and context for these high - priority items on the Product Backlog, providing the Team with insight into the Product Owner’s thinking.

------

## Minimalism Slices

Minimalism Slices, simply refers to the practice of breaking down pieces of work so they can be ackomlished in a reasonable time frame.

- Split your work item into small chunks that are contributed in incremental commits.

- Contribute your chunks frequently. Follow an iterative approach by regularly providing updates and changes to the team. This allows for instant feedback and early issue discovery and ensures you are developing in the right direction, both technically and functionally.

- Do NOT work independently on your task without providing any updates to your team.

### Example of a Bad approach

After six weeks of work you created PR with all required functionality, including portal UI (build settings), backend REST API (UWP build functionality), telemetry, unit and integration tests, etc.

### Example of a Good approach

You divided your feature into smaller user stories (which in turn were divided into multiple tasks) and started working on them one by one:

- As a user I can successfully build UWP apps using current service
- As a user I can see telemetry when building the apps
- As a user I have the ability to select build configuration (debug, release)
- As a user I have the ability to select target platform (arm, x86, x64)
- ...

You also divided your stories into smaller tasks and sent PRs based on those tasks.
E.g. you have the following tasks for the first user story above:

- Enable UWP platform on backend
- Add `build` button to the UI (build first solution file found)
- Add `select solution file` dropdown to the UI
- Implement unit tests
- Implement integration tests to verify build succeeded
- Update documentation
- ...

------

## External Feedback

Various stakeholders can provide feedback to the working product during a project, beyond any formal
review and feedback sessions required by the organization. The frequency and method of collecting
feedback through reviews varies depending on the case, but a couple of good practices are:

### Best Practices for External Feedback

- Capture each review in the backlog as a separate user story.
- Standardize the tasks that implement this user story.
- Plan for a review user story per Epic / Feature in your backlog proactively.

### Tips on giving feedback

- **Give feedback after it’s asked for**. Chiming in during the developmental phase with suggestions and ideas will irritate the developers and collaborators.
- **Ask questions first**. Try to understand why things are this way and the thought process or the justification behind it.
- **Only relay the things under the receiver’s control**. Giving design feedback to the developer will not help in any way. In general, feedback is usually received by one person who classifies the received reviews and forwards them to the right collaborators.
- **Be concise and specific with examples**. While suggesting something, give proper reasoning and provide some examples for the same.
- **Give feedback that will improve the product**. Any feedback that you provide should be aimed at that.
- **End with a request for opinions**. It’s important to know how the receiver of the feedback feels about your ideas and suggestions.

_Example:_ Feedback like “the homepage doesn’t feel good” will not help the dev team. Instead say something like “the homepage doesn’t show information that’s relevant to me as a user.” The latter helps isolate the issue that the problem lies with the content or the way content is presented.

### Tips on receiving feedback

- **Listen to understand and not to reply**. Figure out the intent behind the feedback.
- **Be honest and open** while providing justifications for your decisions regarding the design.
- **A good reason** provided to the reviewer should precede refuting suggestions as to why their opinion and feedback will not work well.
- **Try to figure out why particular feedback is given**. Ask detailed questions in regard to that element of the product.
- **Propose off-the-top alternatives** and see if the reviewer is inclined to accept any of all them. It will help understand what is desired.
- **Follow up**. If there are a few suggestions that require a bit of research on your part, hit pause on that conversation and get back to that later.

------

### Useful Links

- Always try and deliver in [Minimal Slices](./Minimal-Slices.md)
- [Backlog Refinement: Who Should Attend and How to Maximize Value](https://www.mountaingoatsoftware.com/blog/backlog-grooming-who-should-attend-and-how-to-maximize-value#:~:text=A%20good%20rule%20of%20thumb,may%20be%20able%20to%20participate)
- [You're doing backlog refinement wrong. Here's how to do it less wrong](https://clubhouse.io/blog/how-to-do-backlog-refinement-less-wrong/)
- [multi team backlog refinement](https://www.scrum.org/resources/blog/multi-team-backlog-refinement)
- [Product Backlog Refinement explained](https://www.scrum.org/resources/blog/product-backlog-refinement-explained-13)
