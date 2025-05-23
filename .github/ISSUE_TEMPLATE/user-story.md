**As a** [Developer/Tester/Product Owner/Stakeholder]  
**I need** [to manage the lifecycle of a task/feature/bug]  
**So that** [we can efficiently deliver value and track progress]

### Details and Assumptions
* Tasks originate as "New issues" and are moved to the "Icebox" if not immediately prioritized.
* Items in the "Icebox" are potential work that may or may not be picked up.
* The "Product Backlog" contains prioritized items ready for sprint planning.
* The "Sprint Backlog" holds items committed for the current development cycle.
* "In progress" signifies active development on a task.
* "Review /QA" indicates a task is undergoing testing or code review.
* "Done" means a task has been completed and meets all criteria.
* Each task will have an estimate (e.g., story points, hours).
* Team members will update task statuses as they progress.

### Acceptance Criteria
Given a new requirement or bug is identified
When it is added to the "New issues" column
Then it should be visible and have an initial estimate of 0

Given an item is in the "New issues" column
When a decision is made not to work on it immediately
Then it can be moved to the "Icebox" column

Given an item is in the "Icebox" or "New issues" column
When it is prioritized for future development
Then it should be moved to the "Product Backlog" column

Given an item is in the "Product Backlog"
When it is committed for the current sprint
Then it should be moved to the "Sprint Backlog" column

Given an item is in the "Sprint Backlog"
When a team member starts working on it
Then it should be moved to the "In progress" column

Given an item is in the "In progress" column
When the development work is completed
Then it should be moved to the "Review /QA" column

Given an item is in the "Review /QA" column
When it has passed all testing and reviews
Then it should be moved to the "Done" column and marked as complete
