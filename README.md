# GIT

## Semantic Commits

We have very precise rules over how our git commit messages can be formatted. This leads to more readable messages that are easy to follow when looking through the project history.

**Example:**
```
WIP:FIX[consultation{#12}]>Add hat wobble
^-^ ^-^ ^----------^ ^-^   ^-------------^
 |   |   |           |     |
 |   |   |           |     +--> (Capitalised) In nutshell description in present tense.
 |   |   |           |
 |   |   |           +--> (#number,Optinal) Task or Issue id 
 |   |   |
 |   |   +--> (lowercase) Scope  OR Issue ID in case of FIX.
 |   |
 |   +--> (UPPERCASE) Type: FEAT, FIX, DOCS, REVERT, REFACTOR, STYLE or TEST. 
 |
 +--> (UPPERCASE) State: INIT, WIP, DONE.
```

### Type
- **Feat:** Feat in a new feature ( with WIP in cace)
- **Fix:** A bug fix
- **Docs:** Documentation only changes
- **Refactor:** A code change that neither fixes a bug nor adds a feature
- **Style:** Changes that do not affect the meaning of the code (white-space, formatting, missing semi-colons, etc)
- **Test:** Adding missing tests or correcting existing tests

### State
- **INIT:** Init a new feature
- **WIP:**  Work In Progress
- **WID:**  Work Is Done

### Scope
The scope could be anything specifying place of the commit change. For example: consultations, person/medical-history, etc.

### Description
!> The commit summary contains succinct description of the change.

> * Use the imperative, present tense: "Change" not "Changed" nor "Changes".
> * Capitalize first letter
> * no dot (.) at the end

### Revert
If the commit reverts a previous commit, it should begin with ``REVERT:``, followed by the header of the reverted commit. ``REVERT[<hash>]``, where the hash is the SHA of the commit being reverted.

--

### Message Body

> Commit messages are important means of communication between team members and for the lifecycle of the team: its past and its future.

[What makes a good commit message?](https://hackernoon.com/what-makes-a-good-commit-message-995d23687ad#.w6cv0f8f6)

> The seven rules of a great Git commit message:
> 
> 1. Separate subject from body with a blank line
> 2. Limit the subject line to 50 characters
> 3. Capitalize the subject line
> 4. Do not end the subject line with a period
> 5. Use the imperative mood in the subject line
> 6. Wrap the body at 72 characters
> 7. Use the body to explain what and why vs. how


[How to Write a Git Commit Message](http://chris.beams.io/posts/git-commit/)