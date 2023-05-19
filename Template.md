Project or Component Name
=========================

[![pipeline status](...img.svg)](.) and other badges go here in a line. https://docs.gitlab.com/ce/user/project/badges.html

`Mission Statement`: No more than two lines, give a context for everything
below. A good mission statement captures the essense of the component. Remember
the goals of this document:

- Get a technical person oriented in under 15 minutes.
- Describe what is unique to this component, anything that may be unexpected.
- Audience: you five years from now, someone brand new to the component.
- Pictures really help!

> Remember: This template is a guide. Use your judgement about where to add more
> information or sections and where to skip. Every component is different. If you
> are able to meet the two goals above then you've done your job regardless of
> how cloesly you've followed the template.

### Resources

The link names should be very specific so that the reader doesn't need to follow them to understand what they are. This is different than links for a customer oriented website where you want the links simple and general.

- [Project Management / Jira Board]()
- [GitHub Repo example/leaderboard]()
- [Console Admin]()
- [PHPdoc API Documentation]()
- [GitHub build artifacts]()
- [PHPUnit Coverage Reports]()

Quick Start
===========

Short instructions on making things go. A few lines of shell or a link to dev/sandbox.

Goals and Scope
===============

`Goals`

What are the aims? How do we know if they are met? Goals are often tangential
to the problems that are being solved themselves. For instance, the project is
being used as a testbed for a new technology. Or, a goal is to create a model
for future development.

Example

- Usable even under abnormal, extreme load
- Reliable processing even with bad data.
- Can stop and restart the system for a few minutes without causing undo
  stress, lost information, or obvious effect to the customers.
- Be a template for modern Perl development.

`Scope of Work`

What can the reader expect to find in this repo?

- What (major) features/solutions are included.
- What expected features/solutions are excluded.

Example

"This project is limited to what is needed for breaking down tribal knowledge,
specifically in software projects. This project does not try to be a general
solution for documenting all projects or for all documentation a project should
have."

Background
==========

This is optional. Only include things that may significantly affect the design
philosophy. Example: "This is the first project by new interns with little
guidance."

Concepts
========

`Clarification of Common Terms`

Just call out the terms that are special or confusing. For instance, "product"
has a lot of meanings. Clarify how it is used in this component.

> Link to a complete term document if it exists

`Major Components`

Just an intro to their names and how they relate.

`Links to deeper information / relevant code`

Critical Points
===============

Bulleted list of things that are essential or that should be reviewed often. Imagine an exclamation point after each.

Examples

- Maintain 100% test coverage!
- This code called 10,000 times per second!
- Keep it short!

Guiding Principles
==================

How are the goals achieved, problems solved? What is the approach taken in this component? What is the design philosophy?

`Assumptions, Guidelines, Constraints`: Not things like code-standards, things
unique to this component.

`Tech Dependencies`: Basic overview of technology, why chosen. "PHP with
relational database (MySQL) + Redis for sessions and leader board. Infra is
already available and Redis provides a good solution to leaderboards."

`Relevant Resources`: "we based the leaderboard design on this blog post"

Data Model or Flow
==================

A high-level data model or flow diagram. Pick which is appropriate.

[MermaidJS][] works well here. Try the [Live Editor](https://mermaid-js.github.io/mermaid-live-editor/).

```mermaid
graph LR
  API -->|Update| Q
  Website -->|Update| Q
  App Clients -->|Update| Q
  Q(Update Queue) -->|rows| C[queue processor]
  C -->|nats| D[Backing Service 1]
  C -->|nats| E[Backing Service 2]
  C -->|events| F(MySQL activity log)
  style C fill:#e6ffe6,stroke:#aaa,stroke-width:1px
```

[MermaidJS]: https://mermaid-js.github.io/mermaid/#/

Examples
========

These can be actual examples or contrived ones to make a point. Links to code that compiles/runs is also great.

- `Simple / Common`
- `Full, more complex`

Usage
=====

This can be longer and more involved and is generally optional, particularly if
the Quick Start is adequate and there is a good CI script or other way to
learn how the component is used.

