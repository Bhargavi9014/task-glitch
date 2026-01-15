## TaskGlitch – Bug Fix Assignment

### Bug 1 – Data loading twice
- Problem: Tasks were loading twice when the page opened.
- Fix: Ensured the data fetch runs only once.
- Result: No duplicate tasks or duplicate API calls.

### Bug 2 – Undo delete issue
- Problem: After deleting a task, the undo option could bring back old tasks even after the snackbar closed.
- Fix: Cleared the deleted task state when the snackbar closes.
- Result: Undo works only while the snackbar is visible.

### Bug 3 – Task list flickering
- Problem: Tasks with the same ROI were changing order randomly.
- Fix: Added a stable sorting rule with a clear tie-breaker.
- Result: Task order stays the same on every render.

### Bug 4 – Multiple dialogs opening
- Problem: Clicking Edit or Delete also opened the View dialog.
- Fix: Stopped event bubbling on action buttons.
- Result: Only the selected dialog opens.

### Bug 5 – Invalid ROI values
- Problem: ROI showed NaN or Infinity when time or revenue was invalid.
- Fix: Added validation to prevent invalid calculations.
- Result: ROI values are safe and UI no longer breaks.

### How I Worked on This
- Fixed one bug at a time
- Made separate commits for each bug
- Followed the acceptance criteria strictly
- Focused on clean and readable code
