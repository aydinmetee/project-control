# Slice Plan

## Epic
MVP Todo App

## Slice 1 - Backend Todo Read/Write Foundation
Goal:
Create the initial backend capability for creating and listing todos.

Includes:
- Todo entity/model
- Persistence structure
- Create todo API
- List todos API
- Backend validation
- Backend tests

Excludes:
- Mark as completed API
- Frontend integration
- Advanced filtering

Expected Outputs:
- Backend task issue
- Backend PR
- Backend tests

## Slice 2 - Frontend Todo List/Create Flow
Goal:
Create the initial frontend capability for listing and creating todos.

Includes:
- Todo list screen
- Create todo form
- Validation/error states
- Backend API integration for create/list
- Frontend tests

Excludes:
- Complete todo interaction
- Advanced UI polish
- Authentication

Expected Outputs:
- Frontend task issue
- Frontend PR
- Frontend tests

## Slice 3 - Todo Complete Flow End-to-End
Goal:
Allow a todo to be marked as completed through backend and frontend changes.

Includes:
- Backend complete todo API
- Frontend complete interaction
- Completed state UI
- End-to-end acceptance validation

Excludes:
- Undo flow
- Bulk actions
- Advanced filtering

Expected Outputs:
- Backend task issue
- Frontend task issue
- PRs for both repositories
- QA validation for end-to-end flow

## Slice 4 - MVP Stabilization
Goal:
Resolve review findings, QA findings, and close MVP gaps.

Includes:
- Bug fixes
- Small consistency improvements
- Acceptance criteria alignment
- Documentation alignment where needed

Excludes:
- New feature scope
- Nice-to-have improvements

Expected Outputs:
- Bug issues or stabilization tasks
- Final MVP review-ready state