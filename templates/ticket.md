## tldr

- in a concise way, tell your reader the storey of this ticket.
- the reader should answer:
  - is this the ticket I'm looking for?

## details

- why does this ticket exist?
- what gain do we expect from this change?
- who are the people involved or should be notified?
- how do we plan to implement, test, and validate the changes?
- where do we plan to implement this?
- when do we plan to roll these changes out?

## links, references, related

- in a clear format, list down all the details you think could help the viewer better understand your ticket
- video | [Creating a template in microsoft word](https://www.youtube.com/watch?v=4k3FTbX7G0M)
- article | [Create a template using word](https://support.office.com/en-us/article/create-a-template-86a1d089-5ae2-4d53-9042-1191bce57deb)
- article | [Why you should wake up earlier](https://support.office.com/en-us/article/create-a-template-86a1d089-5ae2-4d53-9042-1191bce57deb)

## current state

- what result are you currently getting?

## expected state

- what should be really happening?
  - skip this if this is an incoming feature

## planned state

- what would happen if you finish applying your changes?
- this could actually serve as basis for your test cases

## rollout plan
- update the API
- update the frontend to hide restricted links
- run a visual test
- update the DB and migrate the details to the new column
- clear the application config and cache
- run a complete cycle of the system
- run migration tests
- document new bugs related to the rollout
- create a retrospective for the rollout

## rollback plan
- revert updates the API
- revert frontend restrictions
- run a visual test
- re-create the deleted db column
- create duplicates of the old data to the recreated column
- validate the changes
- clear the application config and cache
- run a complete cycle of the system
- run migration tests
- document new bugs related to the rollback
- create a retrospective for the rollback
