---
title: "Personal notes for optimistic locking"
author: "Chuck Boecking"
date: 2024-06-06
tags: [developer,sql]
type: blog
audience: [developer]
published: true
---
# Personal notes for optimistic locking
Here is my plan:
- add column named lock_token_uu (uuid) to each table.
- any attempt to update must include the lock_token_uu
- trigger will check to see if the old and new token match
- if match, the same trigger will create a new lock_token_uu value

Notes:
- triggers are executed in alphabetically.
- this should be one of the first triggers to execute (1000 value (of 9999 range))
- note the relationship between this effort the desire to track updated values (also set by trigger)
- note the relationship between this effort the desire to track created_by and updated_by values (also set by trigger)
