# SoloMate – Git Workflow

## 1. Project Repositories

- solomate-flutter
- solomate-angular
- solomate-backend
- solomate-docs

## 2. Branch Strategy

- main: Stable and approved project code.
- feat/*: Feature development.
- fix/*: Bug fixes.
- docs/*: Documentation updates.

Never push directly to the main branch.

## 3. Before Starting Development

1. Clone the assigned repository.
2. Switch to the main branch.
3. Pull the latest changes.
4. Create or switch to your assigned feature branch.
5. Start working on your assigned task.

## 4. Branch Naming Convention

Examples:

- feat/trip-planning
- feat/connect-me
- feat/helpme
- feat/authentication
- feat/profile
- feat/admin-dashboard
- feat/service-provider
- fix/login-validation
- docs/architecture-update

## 5. Commit Message Convention

- feat: Add trip planning functionality
- fix: Resolve login validation issue
- docs: Update architecture documentation
- refactor: Improve repository structure
- test: Add authentication tests
- style: Improve profile UI

## 6. Development Workflow

1. Check assigned tasks in the Master Project Tracker.
2. Update task status to In Progress.
3. Implement the assigned feature.
4. Test the implementation locally.
5. Commit the completed changes.
6. Push changes to the assigned branch.
7. Create a Pull Request targeting main.
8. Add the Pull Request link to the tracker.
9. Update task status to Submitted.

## 7. Pull Request Requirements

Every Pull Request must include:

- Task ID
- Feature or module name
- Summary of changes
- Testing results
- UI screenshots, where applicable
- Known issues, if any

## 8. Review and Approval

- The Project Lead reviews submitted Pull Requests.
- Members must resolve requested corrections.
- Only approved Pull Requests may be merged.
- The Project Lead records final approval in the tracker.

## 9. Merge Conflict Rules

- Do not overwrite another member's changes.
- Inform the Project Lead about merge conflicts.
- Resolve conflicts carefully.
- Test again before requesting approval.

## 10. Security Rules

- Never commit API keys, passwords or tokens.
- Never commit confidential environment files.
- Never force-push to shared branches.
- Never delete another member's branch without approval.
