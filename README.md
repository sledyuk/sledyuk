# Hi, I'm Bogdan

I build mobile applications with React Native and TypeScript, primarily using bare React Native. My background spans software development since 2011 and mobile development since 2017.

I work across application architecture, native integrations, API contracts, testing, and iOS/Android releases. When a feature needs more than a mobile client, I also build with React, Next.js, Node.js, NestJS, and PostgreSQL.

I'm interested in how software behaves beyond the happy path: authentication, loading and error states, real-time updates, platform differences, and reliable releases.

## DaySync

[DaySync](https://daysync.io) is a booking and business-management product for salons, and the side project where I try out new technologies against the needs of a real application. I build and maintain its mobile applications, web interface, and backend.

- **Mobile:** bare React Native and TypeScript, released on [iOS](https://apps.apple.com/us/app/daysync-salon-booking/id6473828297) and [Android](https://play.google.com/store/apps/details?id=io.daysync.business).
- **Web:** React and Next.js.
- **Backend:** NestJS, Prisma, and PostgreSQL.
- **Testing:** Maestro for mobile flows and Playwright for web flows.
- **Infrastructure:** Cloudflare and CI workflows.

It gives me a place to work through the complete product lifecycle – from a feature idea to a store release – and to evaluate tools and approaches on something people actually use.

## Building with AI agents

In DaySync I've set up a development workflow around Claude Code, MCP integrations, GitHub Issues, and automated checks. The workflow connects task definition, implementation, testing, and review:

1. **Define the task.** GitHub Issues hold the scope and context for the work.
2. **Implement and verify locally.** Agents work on the changes, run checks, and attach results to the issue.
3. **Review the change.** CI and automated Claude code review provide additional feedback on pull requests.
4. **Check application behavior.** Maestro through MCP supports mobile testing, alongside Playwright for the web.
5. **Decide what ships.** I review the implementation and the test evidence, resolve problems, and take responsibility for the release.

My work here includes configuring the tools and repository guidance, breaking tasks into reviewable changes, and improving the feedback agents receive when something fails. I'm particularly interested in making agent work inspectable: understanding what changed, what was tested, and what still needs human judgment.

## Open source: Redmine

I submitted an implementation of personal access tokens, scoped permissions, and structured API audit logging to Redmine's API authentication feature request. The patch covers token expiration and hashed storage, compatibility with existing API clients, permission enforcement, and tests, verified against trunk with 61 new passing tests.

Review by the core team split the submission into separate tracks:

- [Original implementation and review](https://www.redmine.org/issues/43881#note-11) – the full patch and the discussion it started.
- [API-key logging fix](https://www.redmine.org/issues/44371) – extracted from my patch by a maintainer, resolved and closed for 6.0.11.
- [Fine-grained personal access tokens](https://www.redmine.org/issues/44430) – open, with an architectural discussion about a dedicated token model versus extending the existing OAuth applications.

## Tools I work with

**Mobile:** React Native, TypeScript, React Navigation, MobX, Expo
**Web:** React, Next.js
**Backend:** Node.js, NestJS, Prisma, PostgreSQL, Redis
**Testing and delivery:** Jest, Maestro, Playwright, GitHub Actions, Docker
**AI development:** Claude Code, MCP integrations, automated review and testing workflows

---

[LinkedIn](https://www.linkedin.com/in/bogdan-egikov) · [Email](mailto:sledyuk@gmail.com)
