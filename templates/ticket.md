## TLDR

- in a concise way, tell your reader the story of this ticket.
- the reader should answer:
  - is this the ticket I'm looking for?



## Details

- why does this ticket exist?
- what gain do we expect from this change?
- who are the people involved or should be notified?
- how do we plan to implement, test, and confirm the changes?
- where do we plan to implement this?
- when do we plan to roll these changes out?



## Requirements

- what are the copy, assets, services you need or have to request?
- is there anything preventing you from proceeding with this ticket? 



## References

- in a clear format, list down all the details you think could help the viewer better understand your ticket
- video | [Creating a template in Microsoft word](https://www.youtube.com/watch?v=4k3FTbX7G0M)
- article | [Create a template using word](https://support.office.com/en-us/article/create-a-template-86a1d089-5ae2-4d53-9042-1191bce57deb)
- article | [Why you should wake up earlier](https://support.office.com/en-us/article/create-a-template-86a1d089-5ae2-4d53-9042-1191bce57deb)



## Current State

- what result are you getting?



## Expected State

- what is happening?
  - skip this if this is an incoming feature



## Planned State

- what would happen if you finish applying your changes?
- this could actually serve as basis for your test cases



## Rollout Plan

- update the API
- update the frontend to hide restricted links
- run a visual test
- update the DB and migrate the details to the new column
- clear the application config and cache
- run a complete cycle of the system
- run migration tests
- document new bugs related to the rollout
- create a retrospective for the rollout



## Rollback Plan

- revert updates the API
- revert frontend restrictions
- run a visual test
- recreate the deleted db column
- create duplicates of the old data to the recreated column
- confirm the changes
- clear the application config and cache
- run a complete cycle of the system
- run migration tests
- document new bugs related to the rollback
- create a retrospective for the rollback


