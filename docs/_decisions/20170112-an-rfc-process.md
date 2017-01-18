---
title: A GitHub RFC Process
---

## Summary

GitHub makes it easy for the team to collaboratively build software, but
we're still having problems communicating and recording decisions. This 
RFC outlines a GitHub based RFC (request for comments) process to help.

## Motivation

The main motivation for us needing a process is that we have **three regional 
offices** and a bunch of people who **work from home** either on a full time or part
time basis. The current way we make decisions using emails, meetings, and watercooler
conversations doesn't work because...

:email: Emails keep getting lost<br/>
:house: People from home are cut out<br/>
:earth_asia: The Singapore team tell me they feel like a satellite team<br/>
:triumph: Type A personalities dominate in-person conversations<br/>

Examples of decisions we've made in the past that could have been good RFCs:

* Changing our git workflow
* How to version APIs
* Configuration improvements
* Converting tabs to spaces

## Detailed Design

### Stealing from the open source community

Instead of inventing something new let's steal good ideas from successful open source 
projects which have found ways to engage their communities, by their very nature they 
already far more distributed than we are in the enterprise.

Two projects with excellent RFC processes:

 - [Rust](https://github.com/rust-lang/rfcs)
 - [Ember](https://github.com/emberjs/rfcs)

### Creating a place to store your RFCs

> tl;dr - create a repo to store your RFCs

1. Create a new repo
1. Create a `README.md` describing the process
1. Create an `yyyyMMdd-template.md` with lead in headers
    * Summary
    * Motivation
    * Detailed Design
    * Benefits
    * Drawbacks
    * Alternatives
    * Unresolved questions
1. Create a `/docs` folder to contain your RFCs (you may need a `.gitkeep` if it's empty) 

### Writing an RFC

> tl;dr - write down decisions in markdown and open a pull request

Writing an RFC should be as low ceremony as possible, by following the same
workflow we do for code changes teaching this will be very easy to new
and existing developers.

1. Create a branch
1. Copy the template
1. Complete template using markdown
1. Open a PR to start the conversation
1. Assign reviewers
1. Iterate as necessary
1. Merge the PR when consensus has been reached :tada: :tada:

```
git checkout -b rfc/convert-tabs-vs-spaces
cp yyyyMMdd-template.md docs/20170112-convert-tabs-vs-spaces.md
```

## Benefits

* Very low ceremony 
  * Easy setup
  * Uses the tools we know and love
  * Encourages contribution
* Builds institutional knowledge
  * Includes _context_ of decisions
  * Helps avoid the _new team rewrite_
* Encourages ownership
  * Especially for new team members

## Drawbacks

* More process?
* Decisions take longer to make?
* We have to think through our decisions more?

## Alternatives

* github issues
  * Doesn't work in a forking workflow
  * No change tracking
  * No inline comments
* Use a wiki :pencil2: :cry:
* Use email :love_letter: :boom:

## Unresolved Questions

 - [X] If you build it will they come? :baseball:
  - [X] Yes! :shipit:
  - [ ] ~~No~~