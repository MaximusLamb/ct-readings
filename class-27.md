## setState()
*  It is the only legitimate way to update state after the initial state setup. Let’s say we have a search component and want to display the search term a user submits.
### Reconciliation
* The reconciliation process is the way React updates the DOM, by making changes to the component based on the change in state.
## Snapshot Testing
* A typical snapshot test case for a mobile app renders a UI component, takes a snapshot, then compares it to a reference snapshot file stored alongside the test. The test will fail if the two snapshots do not match: either the change is unexpected, or the reference snapshot needs to be updated to the new version of the UI component.
## Snapshot FACTS
* Treat snapshots as code
* Tests should be deterministic
* Use descriptive snapshot names
