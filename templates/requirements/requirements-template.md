# SRS template from IEEE

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

## Requirements Writing Style Guide

### User Stories

- one or more easily understandable sentences or business language that capture what the user/system needs to do
- as a `user` , I want `some goal` so that `some reason` + within `time or boundary`
- when `event`, the system will `some goal`, within `time or boundary`

---

### Traditional (text based)

- one or more sentences used to specify high level functionality for the business or stakeholders
- `stakeholder`, `shall|will|would` develop a `process|system` `some goal`
- `system` `shall|will|would` provide the ability to `process leading to a goal`

---

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
