## TLDR

- poor requirements = project failure
  - poor requirements is #3 in IEEE as the cause of project failure
- good requirements = much better chance
  - while well drafted project requirements increase your chances significantly,
  - there are still a external factors which would affect the overall success of any propsal/feature/project

---

## Further reading

- [Karl E Wiegers - Software Requirements Third Edition](https://learning.oreilly.com/library/view/software-requirements/9780735679658/)
- [Dean Leffingwell - Agile Software Requirements: Lean Requirements Practices for Teams, Programs, and the Enterprise](https://learning.oreilly.com/library/view/agile-software-requirements/9780321685438/)

---

## Glossary

- shall = is required to
- should = is recommended that
- may = is permitted to
- can = is able to / optional
- must = unavoidable / mandatory
- will = statements of fact

---

## Characteristics of a good requirement document

- Unitary
  - addresses one and only one thing
- Complete
  - fully stated in one place with no missing information
- Consistent
  - does not contradict other requirements
- Atomic
  - does not contain conjunctions
- Traceable
  - meets all or a part of a business needs as stated by stakeholders
  - is authoritatively documented
- Current
  - is not obsolete due to age
  - has been updated within 3 months or every after update to sub components
- Unambiguous
  - concisely stated without use of jargon, acronym, or esoteric verbiage
  - all points of contention has been thoroughly discussed and finalized
- Specific Importance
  - documents the level of importance
  - may be via time, urgency, budget, financial impact, etc.
- Verifiable
  - can be determined through inspection, demonstration, test or analysis

---

## Perspectives when writing requirements

### Users perspective

- requirement = `user type` + `result type` + `object` + `qualifier`
- example. The customer shall be able to send an request to the bank within 4 steps

### System perspective

- requirement = `conditions` + `result` + `qualifier`
- example. When a request is sent by a customer the system shall send an email to the assign banker within 30 secs or next possible interaction

---

## Requirement Writing Styles

### User Stories

- one or more easily understandable sentences or business language that capture what the user/system needs to do
- as a `user` , I want `some goal` so that `some reason` + within `time or boundary`
- when `event`, the system will `some goal`, within `time or boundary`

### Traditional (text based)

- one or more sentences used to specify high level functionality for the business or stakeholders
- `stakeholder`, `shall|will|would` develop a `process|system` `some goal`
- `system` `shall|will|would` provide the ability to `process leading to a goal`

### Use Cases

- a list of actions or event steps, typically defining interactions between an actor and a system, to achieve a goal
- may include a diagram that outlines
  - a `main box with header` representing the scope
  - `actors` outside box scope
  - bubbles representing `use cases`
  - lines to the `actors` and `use case` representing `association`
  - `includes` notation `<--<<include>>-->` meaning mandatory actions
  - `extends` notation `<<extend>>` meaning optional actions

#### Outline of a use case

- Use case number
  - unique identifier, usually a sort of id
- title
  - active-verb goal phrase that names the goal of the primary actor
- description
  - description and purpose of use case
- actors
  - usually a list of actors involved in the scenario
- scope
  - name of the system/sub system
- priority
  - how important is this requirement?
  - where is this in the hierarchy of events?
- assumptions
  - any conditions presumed to be true
- preconditions
  - state the system must be in for the system to proceed
- postconditions
  - changes in the environment as a result of the use case
- trigger
  - what cases this use case to run?
- main success scenarion
  - step by step walk through of the use case
- extensions
  - alternative flows
  - may include exceptions and support

---

## Types of requirements

- Business

  - high level features of the system
  - describe what will be accomplished for the business (not how)
  - usually requires authority from stakeholders
    - style: `traditional (text based)` no actor just capability
    - example: provide an sms notification feature for customers

- User (Stakeholder)

  - describe what will be accomplished for the users/stakeholders
    - style: `traditional (text based)`
    - example: a customer shall be able to receive an sms notification when their bank account is approved
    - style: `user story`
    - example: as a customer, I want to receive an sms notification when my bank account is approved, so I could start depositing cheques

- Functional

  - define the function of the system or its components
  - behaviors, inputs, outputs
    - style: `use cases`
    - style: `user story`
    - example: as a banker I would like to update the customers phone number with their permission so that they could receive sms notifications

- Non-functional

  - criteria that define the operating environment in which the functional requirement exists
  - quality, constraints, non-behavior
    - style: `use cases`
    - style: `traditional (text based)`
    - example: the system shall send the sms notification within 20 seconds when a bank account is approved
    - style: `user story`
    - example: as a customer, I want the system to display my bank account within 5 seconds of navigating to it so that I can be quick and efficient in depositing my cheques

- Interface
  - how one system would interact with another system
  - you may include style guides for interaction specifications
  - hardware, software, communication, user interfaces
    - style: `use cases`
    - style: `traditional (text based)`
    - example: the system shall send the sms notification by consuming the sms api of twilio

---

## Software Requirements Specification

- description of a software system to be developed
- aka requirements written down so we could:
  - facilitate reviews
  - describe the scope of work
  - provide references to software designers
  - provide framework for testing primary and secondary use cases
  - links features to customer requirements
  - platform for ongoing refinement

---

## SRS template from IEEE

- table of contents
- revision history
- introduction
  - purpose
  - document conventions
  - intended audience
  - project scope
  - external references
- overall description
  - product perspective
  - product functions
  - user classes and characteristics
  - operating environment
  - design and implementation constraints
  - user documentation
  - assumption and dependencies
- external interface requirements `(use the user stories|traditional|use cases)`
  - user interfaces
  - hardware interfaces
  - software interfaces
  - communication interfaces
- functional requirements `(use the user stories|traditional|use cases)`
  - system feature 1 . . .
  - system feature 2 . . .
  - system feature 2.1 . . .
  - system feature 2.2 . . .
  - system feature 3 . . .
- non-functional requirements `(use the user stories|traditional|use cases)`
  - performance
  - safety
  - security
  - software quality
  - business rules
- other requirements
- glossary

---

## Tips for writing requirements

### DO

- user terms consistently
- define terms in a glossary
- use an active voice
- be careful of boundary values
- try to be consistent with boundary declarations (try to stick to the direction of less than / greater than)
- avoid negation (which usually leads to double negatives)

### DONT

- design the system
- use vague terms
- speculate (usually, often, typically)
- express possibilities (could, ought to, probably)
- ramble
