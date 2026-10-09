# Unified Portfolio Experience: Executive Strategy

Oct 9, 2026 · @Adam

## Executive summary

We will turn a collection of independently built applications into one coherent portfolio that users experience as a single, trusted product family, in the way people experience Google Workspace rather than a set of unrelated tools.

Today our users pay a hidden tax: duplicate tools for the same job, inconsistent interfaces that must each be relearned, data re-entered across systems, and no single place to find release notes, roadmaps, or help. Every new application added without discipline increases that tax and the cost to sustain it.

The strategy rests on six mutually reinforcing workstreams:

1. **Convergence and integration:** reduce redundancy and connect what remains so work flows across apps.
2. **Feature vs. application discipline:** a clear taxonomy and a deliberately high bar for adding any new application.
3. **Brand cohesion:** one master brand with a shared family identity across every product.
4. **Interface inventory and standardization:** a single visual and interaction language (color, iconography, type, layout, components, patterns) delivered through the design system.
5. **Standardized user portals:** one consistent home for release notes, roadmaps, feedback, and help.
6. **In-app guided tutorials:** learning delivered in the flow of work, built on shared tooling.

This effort is the user-facing expression of Project MACH1. MACH1 builds the capability platforms and orchestration layer underneath; this strategy defines how users meet those capabilities: through a small number of SuperApps that look, behave, and feel like one family.

## Vision, goals, and success measures

**Vision:** One portfolio, one experience. A user who has learned one of our applications already knows how to use all of them, can move work between them without friction, and always knows where to go to learn what changed, what is coming, and how to be heard.

The five strategic goals below each carry a measurable outcome. Baselines are set during the first quarter from the interface inventory, usage telemetry, and help desk data; targets are proposed for leadership approval once baselines exist.

| Goal | What it means | Leading indicator | Outcome measure |
| --- | --- | --- | --- |
| G1. Simplify the portfolio | Fewer apps doing overlapping jobs; every app has a clear, distinct purpose | Convergence candidates identified and dispositioned | Net application count; % of capabilities with a single authoritative app |
| G2. Connect the work | Users complete end-to-end workflows without re-entering data or switching context manually | Integrations delivered against prioritized workflows | Context switches and duplicate entries per key workflow; task completion time |
| G3. Unify the experience | Every app speaks one visual and interaction language | Design system and token adoption per app | % of apps conformant to the standard; cross-app usability (SUS) scores |
| G4. Earn trust through transparency | Users always know what changed, what is next, and that feedback goes somewhere | Apps publishing through the standard portals | Portal coverage; feedback-to-response time; user awareness of changes |
| G5. Reduce time to proficiency | New users become productive quickly; existing users absorb change easily | Apps with guided tutorials for top tasks | Time to first successful task; Tier 1 tickets per active user |

Together these goals should show up in one executive number: **reduced cost of ownership per user**, combining lower sustainment cost from fewer, shared components with lower support and training cost from a consistent experience.

## Guiding principles

These principles settle disputes before they reach leadership. When teams disagree, the decision that better honors these principles wins.

1. **Mission outcomes lead.** We organize around the work users must accomplish, not around the org chart or the history of how a tool was funded.
2. **Extend before you build.** The default answer to a new need is a feature in an existing app or a capability on an existing platform. A new application is the exception and must earn its place.
3. **One way to do a common thing.** Navigation, search, notifications, sharing, settings, and help behave identically everywhere.
4. **Shared by default, unique by exception.** Teams differentiate on mission value, not on buttons, colors, or login screens.
5. **The user sees one product family.** Brand, identity, and transitions between apps should feel like moving between rooms in the same building.
6. **Standards are a product, not a policy.** The design system, portals, and tutorial tooling are funded, maintained, and made easier to adopt than to ignore.
7. **Measure what users experience.** Conformance is a means; reduced friction, faster proficiency, and user trust are the ends.

## Definitions

A shared vocabulary is the first deliverable: most portfolio sprawl starts when a feature is funded, staffed, and branded as if it were an application. The terms nest: capabilities power features, features compose workflows, workflows are delivered by applications, and related applications converge into SuperApps.

### The building blocks

| Term | Definition | Test question | Example |
| --- | --- | --- | --- |
| **Capability** | A reusable business or technical function exposed as a service by a capability platform, with no user interface of its own. | Could multiple apps consume this through an API? | Identity, search, notifications, document storage, geospatial rendering |
| **Feature** | A discrete, user-facing function that helps a user complete a task within an application. A feature has no independent identity, navigation, or audience. | Does it only make sense in the context of a larger job? | Export to PDF, bulk edit, saved filters, a map layer |
| **Workflow** | An ordered sequence of tasks, often spanning roles and features, that produces a defined mission or business outcome. Workflows are what users actually care about. | Does it have a start trigger, a hand-off, and a finished outcome? | Request, review, approve, and publish a product |
| **Application** | A distinct, branded, user-facing product with its own entry point, primary audience, and core job to be done, delivering one or more complete workflows and governed with its own lifecycle. | Would a user name it, launch it, and live in it to do a primary job? | A case management app; an analytic workbench |
| **SuperApp** | A unified application shell that hosts multiple related workflows (often from formerly separate apps) as modules behind one entry point, one navigation model, one identity, and one data context. | Does it serve a whole user role or mission domain end to end? | An analyst SuperApp hosting search, analysis, collaboration, and reporting modules |
| **Module** | A workflow area hosted inside a SuperApp. It may have been an app before convergence, but it shares the shell, navigation, and brand. | Does it live under a SuperApp's navigation rather than its own? | The "Reports" area within the analyst SuperApp |
| **Capability platform** | A product team's service layer (per MACH1) that owns one or more capabilities and serves them to many apps. | Is its customer another product team rather than an end user? | The search platform; the identity platform |

### The two ways apps come together

| Term | Definition | What changes for the user | What changes underneath |
| --- | --- | --- | --- |
| **Integration** | Connecting separate applications so data, context, and actions flow between them while each remains a distinct product. | Fewer manual hand-offs; deep links, shared data, single sign-on, actions triggered across apps. | APIs, events, shared identity and data contracts. Apps keep their own lifecycles. |
| **Convergence** | Consolidating two or more applications (or overlapping features) into a single product, retiring the redundant ones. | One place to do the job; fewer apps to learn and launch. | Code, data, and teams consolidate; at least one product is decommissioned. |

Integration is the right answer when apps serve genuinely different jobs or audiences that occasionally intersect. Convergence is the right answer when apps serve the same job, the same audience, or the same data, so that users are forced to choose between them or use both. Integration is cheaper and faster; convergence produces the larger, more durable gain. Integration is frequently the first step toward convergence.

## Feature vs. application: the high bar

Every new need walks down a ladder and stops at the first rung that satisfies it. A new standalone application is the last rung, and reaching it requires a documented case that every rung above it was tried and failed.

1. **Configure:** Can an existing app meet the need through settings, permissions, or configuration?
2. **Extend:** Can it be delivered as a feature in an existing app that serves the same users?
3. **Compose:** Can it be delivered as a new module inside an existing SuperApp?
4. **Integrate:** Can existing apps meet it if they are connected (shared data, deep links, events)?
5. **Platform:** Is it really a reusable capability that belongs on a capability platform, surfaced through existing apps?
6. **New application:** Only if all five answers are no, and the criteria below are met.

### Criteria for a new application (all must be true)

| Criterion | The bar |
| --- | --- |
| Distinct primary audience | Serves a user role or population not well served by any existing app or SuperApp. |
| Distinct core job | Owns a complete workflow, with its own start and finished outcome, that does not fit an existing app's purpose. |
| Daily-use gravity | Users would launch it and spend meaningful time in it, not visit it as a side trip from another app. |
| No credible home | The owning teams of the closest SuperApps formally agree it would degrade their product's coherence. |
| Built on shared foundations | Commits to the design system, shared identity, capability platforms, standard portals, and the master brand from day one. |
| Sustainment funded | A named product owner and a funded team for at least the full lifecycle, not just the build. |
| Exit plan | Defined success measures and the conditions under which it would be converged or retired. |

### Signals that something is a feature, not an app

- It is requested by the same users who already use an existing app.
- It reads or writes the same data as an existing app.
- Its primary entry point would be a button or link inside another app.
- It would be used weekly or less, or only as one step in someone else's workflow.
- Its justification is speed of delivery ("we can build it faster on our own") rather than user need.

The decision authority for a new application sits with the architecture review board (see Governance), not with the requesting team.

## Criteria for creating a new SuperApp

A SuperApp is justified when a coherent user role or mission domain is currently fragmented across several applications, and unifying it would remove more friction than it adds. The portfolio should hold only a few SuperApps; each one is a long-term commitment.

### Entry criteria (all must be met)

| # | Criterion | Evidence required |
| --- | --- | --- |
| 1 | **Coherent audience or mission domain.** It serves an identifiable role or mission thread end to end. | Persona and mission thread definitions; user research. |
| 2 | **Demonstrated fragmentation.** That audience today relies on three or more apps for related work. | Usage and journey data showing app switching and overlap. |
| 3 | **Shared data and context.** The candidate modules operate on substantially the same entities, so one data context reduces re-entry. | Data and entity mapping across candidate apps. |
| 4 | **Workflow continuity.** Users regularly move work between candidate apps within a single task or session. | Journey maps; cross-app hand-off counts. |
| 5 | **No existing SuperApp home.** The workflows cannot reasonably become modules of an existing SuperApp. | Fit assessment signed by existing SuperApp owners. |
| 6 | **Platform readiness.** The supporting capabilities exist or are funded on MACH1 capability platforms, so the SuperApp is a composition, not a rebuild. | Capability map; platform roadmap commitments. |
| 7 | **Convergence commitment.** A decommission plan exists for the apps it replaces, with dates. A SuperApp that adds an app without retiring others has failed its purpose. | Signed retirement and migration plan. |
| 8 | **Single accountable owner.** One product leader owns the shell, navigation, and module integration, with authority over contributing teams. | Named owner and operating model (e.g., platform and stream-aligned teams). |

### Design obligations once approved

- One entry point, one global navigation model, one search, one notification center, one settings area.
- Modules plug into the shell through a defined contract (micro-frontend or equivalent) so teams ship independently without fragmenting the experience.
- Shared identity and permissions: users never re-authenticate or re-select context when moving between modules.
- Built entirely on the design system and master brand; modules do not carry their own sub-brands.
- Release notes, roadmap, feedback, and tutorials surface through the standard portals at the SuperApp level.

### Warning signs a SuperApp is the wrong answer

- The proposed modules share a funding line or organization but not users or data.
- It is a portal of links rather than a unified shell.
- No existing application would be retired.
- The audience is so broad that navigation would become a menu of everything.

## Brand cohesion

The Google Workspace model is a **branded house**: one master brand carries the trust, and each product is a clearly named member of the family rather than a brand of its own. Users recognize a Google app before they read its name, and they know how it will behave before they use it. Brand cohesion is as much about shared behavior as shared appearance.

### Brand architecture decision

| Model | Description | Fit for us |
| --- | --- | --- |
| Branded house (recommended) | Master brand + descriptive product name ("Google Docs", "Google Drive"). | Maximizes recognition and trust; makes convergence easy because products are not attached to independent identities. |
| Endorsed brands | Distinct product brands with a visible master endorsement ("by X"). | A transitional option for well-established legacy products during migration. |
| House of brands | Independent product brands with no visible link. | The current state for many apps; the pattern this strategy retires. |

### Considerations

1. **Master brand definition.** Name, mark, mission statement, and brand promise for the portfolio as a whole. Decide whether the master brand is the organization, a platform name, or a new portfolio name.
2. **Product naming convention.** A single pattern: master brand + plain descriptor of the job (e.g., "\[Brand\] Analysis", "\[Brand\] Reports"). Descriptive names tell users what a product does and make convergence painless. Evocative or mythological names remain valuable for internal platforms, programs, and engineering systems, but user-facing products should use descriptors. Retire acronym-only names.
3. **Icon family.** One construction system for all app icons: shared grid, shape language, corner radius, stroke weight, and master palette, with each app distinguished by a single glyph. Google's icon set is the reference: every icon is unmistakably related.
4. **Color system.** One master palette expressed as design tokens, with semantic colors (success, warning, error, info) identical everywhere. Allow at most one per-product accent, drawn from the master palette. Light and dark modes are defined once, centrally.
5. **Typography.** One type family (open-licensed and self-hostable for our environment) and one type scale across all products.
6. **Universal chrome.** A shared global header containing the app switcher (the "waffle"), universal search, notifications, help, and the account/profile menu, in the same place with the same behavior in every app. This single element does more for perceived cohesion than any visual refresh.
7. **Voice, tone, and terminology.** A content style guide and a shared glossary so the same action has the same word everywhere ("Share", not "Distribute" in one app and "Send" in another), including error messages and empty states.
8. **Entry and exit moments.** Consistent sign-in, loading and splash screens, email and notification templates, and help/documentation styling, since these are where users form first impressions.
9. **Motion and sound.** A small shared vocabulary of transitions and feedback so interactions feel related (addressed in Phase 3 of the interface inventory).
10. **Accessibility as brand.** WCAG 2.2 AA conformance is part of the brand promise, not a separate compliance item.
11. **Transition plan for legacy brands.** Sequence renaming with convergence so users are not asked to learn a new name for a product that will be retired soon. Communicate changes through the release notes portal.
12. **Brand stewardship.** A small brand council (UX, product, communications) owns the guidelines, approves product names and icons, and maintains brand assets inside the design system so teams consume them rather than recreate them.

## Workstreams

Each workstream has an executive objective, a primary deliverable, and a link to the goals above.

| Workstream | Objective | Key deliverables | Goals |
| --- | --- | --- | --- |
| 1. Convergence and integration | Remove redundancy and connect what remains. | Portfolio capability map; overlap analysis; disposition for every app (retain, integrate, converge, retire); prioritized integration backlog tied to key workflows. | G1, G2 |
| 2. Feature vs. application | Stop sprawl at the source. | Ratified definitions; decision ladder; new-app and SuperApp criteria embedded in architecture review. | G1 |
| 3. Brand cohesion | One recognizable product family. | Brand architecture decision; naming convention; icon family; universal header and app switcher; content style guide. | G3, G4 |
| 4. Interface inventory | One visual and interaction language. | Phase 1 (framework, iconography, typography, color, spacing); Phase 2 (component inventory); Phase 3 (motion, content, data visualization, interaction and form patterns); gap analysis feeding the design system and token roadmap. | G3 |
| 5. Standardized portals | One trusted place to learn and be heard. | Common release notes, roadmap, feedback, and help center patterns per app, reachable from the universal header; a standard for writing release notes users can understand. | G4, G5 |
| 6. In-app guided tutorials | Learning in the flow of work. | Tutorial standards on shared tooling; top-task tours for every app; tutorials updated with each major release; support for disconnected video creation. | G5 |

**How they connect:** the inventory (4) supplies the evidence for brand decisions (3) and for spotting duplicate apps (1). The decision ladder (2) prevents new sprawl while convergence (1) reduces existing sprawl. Portals (5) and tutorials (6) carry every change to users, so convergence and rebranding land as improvements rather than disruptions. These two also anchor the broader user enablement strategy.

## Governance and phasing

Standards without decision rights become suggestions. This strategy embeds its decisions in the existing architecture review process so that portfolio choices are made once, by the right people, and enforced at the points where teams already seek approval.

| Decision | Decides | Consulted | Where enforced |
| --- | --- | --- | --- |
| New application or SuperApp | Architecture review board | UX, product owners of nearest apps, mission stakeholders | Architecture review; funding requests |
| Convergence or retirement of an app | Technical Director, with leadership approval | Product owners, affected users, enablement | Portfolio roadmap |
| Brand, naming, and icons | Brand council | Communications, product owners | Design system release |
| Design system standards and tokens | Design system team | App teams, accessibility | Pipeline conformance checks; design reviews |
| Portal and tutorial standards | UX and user enablement | App teams, help desk | Release readiness checklist |

**Enforcement through paved roads:** the most effective governance makes the standard the easiest path. Shared components, the universal header, portal templates, and tutorial tooling should be available through the internal developer platform so adopting them takes less effort than building alternatives. Conformance checks run in the centralized CI/CD pipeline where possible.

### Proposed phasing

&#91;embedded content: proposed phasing · 4 phases, 3 gates\]

Phasing aligns with MACH1: the October to December foundation period sets definitions and evidence, and user-visible changes begin in January. Dates are proposed for leadership review.

## Risks and open decisions

### Key risks

| Risk | Mitigation |
| --- | --- |
| App teams see convergence as a loss of identity or funding. | Frame convergence around user outcomes; protect team continuity by moving teams into stream-aligned roles within SuperApps or onto capability platforms. |
| Standards are published but not adopted. | Deliver standards as paved-road components; enforce at architecture review and in the pipeline; publish conformance openly. |
| Rebranding outpaces convergence, so users learn names that soon disappear. | Sequence naming changes with convergence decisions. |
| A SuperApp becomes a portal of links rather than a unified shell. | Hold SuperApps to the design obligations; require a module contract and shared navigation before launch. |
| Users experience the changes as disruption. | Announce every change through the release notes portal and ship guided tutorials with each major change. |

### Decisions needed from leadership

- [ ] Ratify the definitions and the decision ladder as portfolio policy.
- [ ] Adopt the branded house model and select the master brand.
- [ ] Grant the architecture review board authority over new applications and SuperApps.
- [ ] Approve the proposed phasing and the first SuperApp candidate for evaluation.
- [ ] Fund the design system, portals, and tutorial tooling as products with dedicated teams.
