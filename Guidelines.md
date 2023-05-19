Guidelines
==========

The most important things to remember while writing your document:

- Get a technical person oriented in under 15 minutes.
- Describe what is unique to this project, anything that may be unexpected.
- The audience: you five years from now, someone brand new to this component.
- Pictures really help!

The template is a guide. Use your judgment about where to add more information
or sections and where to skip. Every project is different. If you are able to
meet the two goals above then you've done your job regardless of how closely
you've followed the template. Perhaps you have discovered a more general truth.
Open an MR for this repo!

Using these Guidelines
----------------------

Getting familiar: First, read this whole document. Then look through the
template and compare what is here with each section.

When it comes time to use the template, think about the "important things"
above as you go. If you are ever unsure, considering skipping a section, or a
section grows too long, re-read the relevant sections from this document.

This template and guidelines can be used at any level of documentation, from
the top level of a web project to a single component like a PHP namespace.

Mission Statement
=================

A mission statement isn't just a short description of what this thing does but
an expression of what this component is about. Don't hesitate to incorporate
intangibles or purpose beyond solving a specific problem.

> HELP! Good examples of mission statements are needed!

Resources
=========

These links serve two functions

- Indicate where all relevant stuff is, suggesting a map of the whole project.
- Quick access from the project to these places

This means that the link names are not standardized and should be as specific
as possible. For instance, a link to the project in jira should be "Jira
Project WebDev" as opposed to "Issues". You can assume the reader knows what
jira is. The reader won't have to click to the link to know this project is
part of the WebDev Jira project. This is different than links for a customer
oriented website where you want the links simple and general.

Quick Start
===========

These instructions should be short, short enough that one could glance at them
to get the idea. If there isn't a fast way to get going just skip this section.
At the end is a Usage section that can be any length.

Goals and Scope
===============

### Goals

What are the aims? How do we know if they are met?

There is no need to list every possible goal. Everyone knows you're here to
solve a problem. List the goals that are unique to this project.

Goals are often tangential to the problems that are being solved themselves.
For instance, the project is being used as a test bed for a new technology. Or,
a goal is to create a model for future development. Good goals give more
specifics to the mission statement.

### Scope of Work

What (major) features/solutions are included. What expected features/solutions
are excluded.

The scope is a very important section. This helps the reader know to expect. If
they are looking for credit card processing in the Billing package but it only
covers invoices and subscriptions, the reader should be alerted to that.

Background
==========

Often it is helpful to know the environment within which the project was
conceived. This should be very brief and probably often excluded. Definitely an
optional section but if you need/want to write some history this is the place
to do it.

You may wonder why this section isn't more prominent. It is because ultimately
the background shouldn't matter too much. It is only needed to aid in context
if everything else isn't easily understood.

Concepts
========

### Clarification of Common Terms

This should not attempt to be a complete glossary. Only define terms that are
vague and give them very concrete meanings. Think about RFC 2181,
"Clarifications to the DNS Specification". There is a complete spec elsewhere,
this just pins down the confusing and vague stuff.

This section can also reinforce terms correct usage of common terms. Call out
terms that have a specific meaning within the code that are perhaps more
loosely used in conversation. For instance, "service" is often thrown around
when talking about what a company offers, but in a provisioning system it
likely refers to specific aspect or unit of deployment.

### Major Components

Just an intro to their names and how they relate. For instance, the overall
architecture of a large e-commerce website can be shown in a diagram with five
or so boxes.

This is a good place for diagrams.

### Deep Information

Links to code documentation that further explains the components, their
architecture, and any specifics of using them.

Critical Points
===============

Critical Points are things that you would like the reader to keep in mind at
all times. This could be anything from performance to code clarity. What do you
want your reader to remember once they've moved on from the documentation?

Design Principles
=================

### Assumptions, Guidelines, Constraints

Not things like code-standards, things unique to this project.

Assumptions are things that you are going to do that haven't been tested but
are expected to work. For instance, "We assume this project will be deprecated
when we finish project X."

Guidelines are ideas or patterns that are used in the code. For instance,
"There is a lot of date/time manipulations in this code so _always_ use our
Carbon wrapper so that convenience methods are available." Or, "Follows
laravel's flavor of Manager pattern for all pluggable classes." Play
particularly close attention to any convention that is developed. E.g. "All
non-psr4 code goes under lib-legacy with the namespace Legacy."

### Tech Dependencies

Basic overview of technology and why it was chosen. E.g. "PHP with relational
database (MySQL) + Redis for sessions and leader board. Infra is already
available and Redis provides a good solution to leaderboards." Always include
this section even if it is really boring, "PHP/MySQL". But be serious about it
and think about what the tech dependencies really are. "This code uses Guzzle
Service Descriptions for API client." "Routes generated from OpenAPI document
with JanePHP."

### Relevant Resources

Links to any information that will help understand how things were done. E.g.
"We based the leaderboard design on this blog post." "Follows DNS terminology
from RFC 7719, except that we also use the term "label" for unique ids in
rdata."

Data Model or Flow
==================

A high-level data model or flow diagram. Pick which is appropriate.

General, no need for specifics. Just point out any peculiarities. For instance,
a simple PHP/MySQL CRUD API may best show its novelty with its database design.
Just show how the pattern used when the API doesn't exactly match the tables.

This can be hard to make short and simple. Think about what makes this
application unique or how it fits into a larger picture.

Examples
========

These can be actual examples or contrived ones to make a point. Links to
example code that is compiled or run during tests is even better.

Include a simple one that helps get a feel of things and then a more complex
one that illuminates the details.

Usage
=====

Most of the time we all scan a readme for the usage instruction to get an idea
of what a program does and how it works. So this is another opportunity to
convey that information. Unfortunately, usage for projects like web apps
doesn't indicate anything helpful. In those cases make sure to show how to
develop on the project and how to run its test suite.
